# Transport Binding

> **Downloads** The code samples used in this user guide have been made available in the [Be.Stateless.BizTalk.Factory.Samples][github.samples] GitHub repository.

Let us configure the transport of our sample Microsoft BizTalk Server® [Receive Locations](./ReceiveLocation.md) and [Send Ports](./SendPort.md). Depending on whether this is a receive location or a send port, the developer will have to configure either an inbound or an outbound adapter.

## Transport Adapter

> **Important** There is much more to be said about the configuration of transport adapters and the developer is invited to read the dedicated section about the [Adapter](./Adapter.md)s for more information.

API wise, configuring the transport adapter of either a receive location or a send port is almost identical. There is however no risk that a developer could inadvertently configure an outbound adapter for a receive location &mdash;or, conversely, an inbound adapter for a send port&mdash; as this is prevented by the `Binding DSL` at its core, i.e. the `C#` would not even compile.

For the illustration's sake, let us configure the transport adapter of our [`Bribe Receive Location`][bribe-receive-location]. You should notice a familiar `Binding DSL` pattern right now: the constructor is given a configuration lambda.

```csharp
Transport.Adapter = new FileAdapter.Inbound(
  a => {
    a.ReceiveFolder = @"c:\file\evil\bribes";
    a.FileMask = "*.xml";
    a.RenameReceivedFiles = true;
  });
```

The configuration of the transport adapter of our inline [`Credit Note Receive Location`][credit-note-receive-location] is very similar:

```csharp
rl.Transport.Adapter = new FileAdapter.Inbound(
  a => {
    a.ReceiveFolder = @"c:\file\billing\credits";
  }
);
```

> **Remark** We can rely on the configuration properties' default values and don't have to configure all of them for any given adapter. Anyway, should we forget to configure a mandatory property, this would be caught by the [`ApplicationFixture`][application-fixture]'s `GenerateApplicationBinding` test. Let us suppose we forget to configure the `ReceiveFolder`, then the test would fail complaining that it _Did not expect any exception, but found Be.Stateless.BizTalk.Dsl.Binding.BindingException with message "[Credit Note Receive Location] Receive Location's Transport is not valid: Inbound file adapter has no source folder."_

As illustrated by the following code excerpt, configuring the outbound adapter is unsurprisingly very similar too:

```csharp
Transport.Adapter = new FileAdapter.Outbound(
  a => {
    a.DestinationFolder = @"c:\file\tax-evasion";
  }
);
```

## Transport Host

Configuring the transport host of any receive location or send port really is a no brainer. For our inline [`Credit Note Receive Location`][credit-note-receive-location] this would look like:

```csharp
rl.Transport.Host = "BizTalkServerApplication";
```

While for our separate [`Bribe Receive Location`][bribe-receive-location] that would be:

```csharp
Transport.Host = "BizTalkServerApplication";
```

## Receive Location's Transport Specifics

### Schedules and Service Windows

`BizTalk.Factory`'s `Binding DSL` exposes a rich `API` to configure all the aspects of receive location's [`Schedule`][schedule] and [`ServiceWindow`][service-window], as illustrated by the following examples.

With a non recurring service window:

```csharp
Transport.Schedule = new Schedule {
  AutomaticallyAdjustForDaylightSavingTime = true,
  StartDate = new DateTime(2022, 1, 20),
  StopDate = new DateTime(2022, 2, 14),
  TimeZone = TimeZoneInfo.Utc,
  ServiceWindow = RecurringServiceWindow.None
}
```

With a **daily** recurring service window:

```csharp
Transport.Schedule = new Schedule {
  ...
  ServiceWindow = new DailyServiceWindow {
    StartTime = new Time(8, 0),
    StopTime = new Time(20, 0),
    From = new DateTime(2022, 1, 20),
    Interval = 4
  }
}
```

With a **weekly** recurring service window:

```csharp
Transport.Schedule = new Schedule {
  ...
  ServiceWindow = new WeeklyServiceWindow {
    StartTime = new Time(8, 0),
    StopTime = new Time(20, 0),
    From = new DateTime(2022, 1, 20),
    Interval = 2,
    WeekDays = BtsDayOfWeek.Monday | BtsDayOfWeek.Friday
  }
}
```

With a **monthly** recurring service window based on **calendar** days:

```csharp
Transport.Schedule = new Schedule {
  ...
  ServiceWindow = new CalendricalMonthlyServiceWindow {
    StartTime = new Time(8, 0),
    StopTime = new Time(20, 0),
    Months = Month.January | Month.April | Month.July | Month.October,
    Days = MonthDay.Day01 | MonthDay.Day08 | MonthDay.Day15 | MonthDay.Day22 | MonthDay.Day29,
    OnLastDay = true
  }
}
```

With a **monthly** recurring service window based on **ordinal** days:

```csharp
Transport.Schedule = new Schedule {
  ...
  ServiceWindow = new OrdinalMonthlyServiceWindow {
    StartTime = new Time(8, 0),
    StopTime = new Time(20, 0),
    Months = Month.January | Month.March | Month.June,
    Ordinality = OrdinalType.First,
    WeekDays = BtsDayOfWeek.Monday | BtsDayOfWeek.Friday
  }
}
```

> **Remark** Custom [`Schedule`][schedule] and [`ServiceWindow`][service-window] classes could be written in an environment sensitive way &mdash;see [Environment Overrides](./EnvironmentOverrides.md)&mdash; and will be given the opportunity to provide different configurations according to the target environments for which the application bindings are generated.

> **Remark** When trying to compile some of the previous samples, the compiler might complain that _The type 'BtsDayOfWeek' is defined in an assembly that is not referenced. You must add a reference to assembly 'Microsoft.BizTalk.ExplorerOM, Version=3.0.1.0, Culture=neutral, PublicKeyToken=31bf3856ad364e35'._ In this case, the developer should reference the `BizTalk.Server.2020.Utilities` `NuGet` package.
>
> In doing so the developer might causes another compilation to arise, namely, _The type 'BtsDayOfWeek' exists in both 'Microsoft.BizTalk.ExplorerOM, Version=3.0.1.0, Culture=neutral, PublicKeyToken=31bf3856ad364e35' and 'Microsoft.BizTalk.Messaging, Version=3 .0.1.0, Culture=neutral, PublicKeyToken=31bf3856ad364e35'_.
>
> Fixing this problem is more involved and requires the developer to define a `C#` [`extern alias`][extern-alias]. Assigning an alias to a specific assembly that is part of a multi-assembly `NuGet` package is not supported by Visual Studio user interface. It is however fairly easy to edit the project file, i.e. `Org.Anization.Accounting.Bindings.csproj`, and add the following excerpt:
>
> ```XML
> <ItemGroup>
>   <Reference Include="Microsoft.BizTalk.ExplorerOM">
>      <Aliases>ExplorerOM</Aliases>
>   </Reference>
> </ItemGroup>
> ```
>
> and rewrite the source file's using directive as follows &mdash;notice the `Explorer::` prefix:
>
> ```c#
> using ExplorerOM::Microsoft.BizTalk.BtsScheduleHelper;
> ```

## Send Port's Transport Specifics

### Retry Policies

A send port's transport expose a configurable _retry_ feature. The `BizTalk.Factory`'s `Binding DSL` API surfaces it as a [`RetryPolicy`][retry-policy] class, which exposes 2 properties:

- a `Retry count` whose type is integer;
- a `Retry interval` whose type is a `TimeSpan`, this way freeing the developer of having to remember the time unit in which to express the interval duration before the next attempt to send the message.

```csharp
Transport.RetryPolicy = new RetryPolicy {
  Count = 3,
  Interval = TimeSpan.FromHours(2)
};
```

Every seasoned Microsoft BizTalk Server® developer knows that there is a _default_ retry policy that every send port inherits. Faithful to this principle, every send port declared and configured through `BizTalk.Factory`'s `Binding DSL` will have the same default retry policy unless otherwise specified. This _default_ policy is explicitly available through the static `Default` property of the [`RetryPolicy`][retry-policy] class.

```csharp
using Be.Stateless.BizTalk.Dsl.Binding;

Transport.RetryPolicy = RetryPolicy.Default;
```

> **Remark** For the record, the `RetryPolicy.Default` does not have hardcoded `Count` and `Interval` values but rather fetches them from the configuration classes being part of the native Microsoft BizTalk Server® API.

### Environment Sensitive Retry Policies

Recall that a custom [`RetryPolicy`][retry-policy] class could be written in an environment sensitive way &mdash;see [Environment Overrides](./EnvironmentOverrides.md)&mdash; so as to be given the opportunity to provide different configurations according to the target environments for which the application bindings are generated.

`BizTalk.Factory`'s `Binding DSL` has done precisely that and comes with a predefined set of environment sensitive [`RetryPolicies`][environment-sensitive-retry-policy] made available together with its [Naming Convention](./NamingConvention.md) &mdash;see [Be.Stateless.BizTalk.Dsl.Binding.Conventions][nuget.conventions] `NuGet` package. `BizTalk.Factory` defines three _not so arbitrary_ retry policies:

- a `RealTime` one, which features no retry at all;
- a `ShortRunning` one, which features 6 retries, one every 5 minutes, thus attempting to deliver a message for a total period of 30 minutes;
- a `LongRunning` one, which features 72 retries, one every hour, thus attempting to deliver a message for a total period of 3 days.

Each of these policies is environment sensitive in its own way:

- the `RealTime` one will always be the one actually configured. not matter what the target deployment environment;

- the `ShortRunning` one will be replaced by the `RealTime` one in every target deployment environment but the `PREPRODUCTION` and `PRODUCTION` ones;

- the `LongRunning` one will be replaced by the `RealTime` one in the `DEVELOPMENT` or `BUILD` target deployment environments, and by the `ShortRunning` one in the `ACCEPTANCE` target deployment environment.

The whole idea behind these policies is that the developer expresses his actual intent in the code, but the configuration is smart enough to avoid long periods of message delivery attempts in non production environments, therefore speeding up the tests that can rapidly became operationally painful otherwise.

### Service Windows

A service window restricts the send port to work during certain hours of the day. It is exposed by the send port's [`ServiceWindow`][service-window] property, which is a class exposing 2 properties:

- a `StartTime` whose type is a [`Time`][time];
- a `StopTime` whose type is a [`Time`][time].

Should you wonder how to configure a service window and instantiate a [`Time`][time] type, the intellisense will guide you through.

```csharp
Transport.ServiceWindow = new ServiceWindow {
  StartTime = new Time(11, 12, 13),
  StopTime = new Time(23, 22, 21)
};
```

> **Remark** A custom [`ServiceWindow`][service-window] could be written in an environment sensitive way &mdash;see [Environment Overrides](./EnvironmentOverrides.md)&mdash; and will be given the opportunity to provide different configurations according to the target environments for which the application bindings are generated.

<!-- links -->

[github.samples]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Samples
[nuget.conventions]: https://www.nuget.org/packages/Be.Stateless.BizTalk.Dsl.Binding.Conventions

<!--  -->

[application-fixture]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Samples/blob/master/src/Org.Anization.Accounting.Bindings.Tests/ApplicationFixture.cs
[bribe-receive-location]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Samples/blob/master/src/Org.Anization.Accounting.Bindings/ReceiveLocations/BribeReceiveLocation.
[credit-note-receive-location]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Samples/blob/master/src/Org.Anization.Accounting.Bindings/Application.cs#L45
[environment-sensitive-retry-policy]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding.Conventions/Dsl/Binding/Convention/RetryPolicy.cs
[extern-alias]: https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/extern-alias
[retry-policy]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/RetryPolicy.cs
[schedule]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/Scheduling/Schedule.cs
[service-window]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/Scheduling/ServiceWindow.cs
[time]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/Scheduling/Time.cs

<!--
cSpell:ignore Anization brainer ordinality PREPRODUCTION
-->
