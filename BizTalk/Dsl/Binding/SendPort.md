# Send Port Binding

> **Downloads** The code samples used in this user guide have been made available in the [Be.Stateless.BizTalk.Factory.Samples][github.samples] GitHub repository.

Growing our `Application` binding [sample](./Application.md), let us add send ports to handle the interactions with our `Embezzlement` subsidiary and our external `Tax-Evading Shell Company`. The developer can choose between 2 alternate syntaxes to declare new send ports: he can use fluent syntactic helpers or separate types.

## Fluent Declaration

Using the fluent API, we can add the `Embezzlement` send port to our `Accounting` application as follows:

```csharp
public Application()
{
  ...
  SendPorts.Add(
    SendPort(
      sp => {
        sp.Name = "Embezzlement Send Port";
        sp.SendPipeline = new SendPipeline<XmlTransmit>();
        sp.Transport.Adapter = new FileAdapter.Outbound(a => { a.DestinationFolder = @"c:\file\embezzlement"; });
        sp.Transport.Host = "BizTalkServerApplication";
      }));
  ...
}
```

## Separate Type Declaration

If we prefer to declare a separate type for the `Tax-Evading Shell` we can define the following class:

```csharp
using Be.Stateless.BizTalk.Dsl.Binding;
using Be.Stateless.BizTalk.Dsl.Binding.Adapter;
using Be.Stateless.BizTalk.MicroPipelines;

namespace Org.Anization.Accounting
{
  public class TaxEvadingShellCompanySendPort : SendPort
  {
    public TaxEvadingShellCompanySendPort()
    {
      Name = "TaxEvadingShellCompany";
      SendPipeline = new SendPipeline<XmlTransmit>();
      OrderedDelivery = true;
      Priority = Priority.Normal;
      Transport.Adapter = new FileAdapter.Outbound(a => { a.DestinationFolder = @"c:\file\tax-evasion"; });
      Transport.Host = "BizTalkServerApplication";
    }
  }
}
```

> **Remark** As illustrated, _ordered delivery_ and _priority_ can be configured too.

## Filters

Configuring [subscription filters][send-port-filters] thanks to the BizTalk Server Administration Console can rapidly become tedious; even more so if directly written as `XML` configuration binding.

`BizTalk.Factory`'s `Binding DSL` tremendously streamlines and alleviates theses burdens. No more magic strings when configuring filters against, for instances, message types or port names. No more struggle when combining predicates through `or` and `and` operators.

Let us illustrate some of the main advantages of writing subscription through `BizTalk.Factory`'s `Binding DSL`.

1. It uses the same context property accelerators that are used by the [Message Context Abstraction](../../Abstractions/README.md#message-context-abstractions) `API` and are type safe &mdash;`C#` will prevent the developer from comparing a property of type `bool` with a `string` for instance:

   ```csharp
   Filter = new Filter(
     () => BtsProperties.AckRequired == true
   );
   ```

2. It frees the developer from using magic strings for message types or port names &mdash;though it should be discouraged to write filter directly against port names as they can easily be altered through the administration console:

   ```csharp
   Filter = new Filter(
     () => BtsProperties.MessageType == SchemaMetadata.For<Any>().MessageType
       && BtsProperties.ReceivePortName == ApplicationBinding.ReceivePorts.Find<EvilBankReceivePort>().Name
   );
   ```

   This will produce the following `XML` configuration binding:

   ```xml
   <Filter>
     <Filter>
       <Group>
         <Statement Property="BTS.MessageType" Operator="0" Value="http://schemas.microsoft.com/BizTalk/2003/Any#Root" />
         <Statement Property="BTS.ReceivePortName" Operator="0" Value="Bank of Evil ReceivePort" />
       </Group>
     </Filter>
   </Filter>
   ```

3. It is intuitive to combine predicates through `or` and `and` logical operators as the `Binding DSL` will take care of redistributing these operators correctly so as to produce valid subscription filters in all cases:

   ```csharp
   Filter = new Filter(
     () =>
       (BtsProperties.MessageType == SchemaMetadata.For<Any>().MessageType || BtsProperties.ReceivePortName == ApplicationBinding.ReceivePorts.Find<EvilBankReceivePort>().Name)
       && BizTalkFactoryProperties.EnvironmentTag == TargetEnvironment.ACCEPTANCE
   );
   ```

   This will produce the following `XML` configuration binding:

   ```xml
   <Filter>
     <Filter>
       <Group>
         <Statement Property="BTS.MessageType" Operator="0" Value="http://schemas.microsoft.com/BizTalk/2003/Any#Root" />
         <Statement Property="Be.Stateless.BizTalk.Schemas.BizTalkFactory.EnvironmentTag" Operator="0" Value="ACC" />
       </Group>
       <Group>
         <Statement Property="BTS.ReceivePortName" Operator="0" Value="Bank of Evil ReceivePort" />
         <Statement Property="Be.Stateless.BizTalk.Schemas.BizTalkFactory.EnvironmentTag" Operator="0" Value="ACC" />
       </Group>
     </Filter>
   </Filter>
   ```

   4. It is impossible to write invalid subscription filters even though they can be written in `C#`:

   ```csharp
   Filter = new Filter(
     () => BtsProperties.MessageType == null
   );
   ```

   This will throw the following exception when the `GenerateApplicationBinding` test method is executed:

   ```csharp
   System.NotSupportedException with message "Cannot translate FilterPredicate "() => (BtsProperties.MessageType == null)" because filter value can be null only if the operator is exists."
   ```

   By opposition, the following subscription filter is therefore valid:

   ```csharp
   Filter = new Filter(
     () => BtsProperties.MessageType != null
   );
   ```

   and would produce the following `XML` configuration bindings, making use of the `Exists` operator:

   ```xml
   <Filter>
     <Filter>
       <Group>
         <Statement Property="BTS.MessageType" Operator="6" />
       </Group>
     </Filter>
   </Filter>
   ```

   For a thorough coverage, the developer is invited to take a look at all the various ways one can write `C#` type-safe subscription filters in the [FilterFixture][filter-fixture] unit testing class, as well as how they translate to binding configuration's `XML`.

## Backup Transport

Because a send port's backup transport is optional, it is exposed as a [`Lazy<T>`][lazy-of-t] type through the `BackupTransport` property, which can be configured as follows &mdash;in a very similar way to how a send port's primary transport is configured:

```csharp
BackupTransport.Value.Adapter = new FileAdapter.Outbound(a => { a.DestinationFolder = @"c:\file\tax-evasion-backup-plan"; });
BackupTransport.Value.Host = "BizTalkServerApplication";
BackupTransport.Value.RetryPolicy = RetryPolicy.Default;
BackupTransport.Value.ServiceWindow = new ServiceWindow { StartTime = new Time(1, 0), StopTime = new Time(23, 0) };
```

<!-- links -->

[github.samples]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Samples

<!--  -->

[filter-fixture]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/master/src/Be.Stateless.BizTalk.Dsl.Binding.Tests/Dsl/Binding/Subscription/FilterFixture.cs
[lazy-of-t]: https://docs.microsoft.com/en-us/dotnet/api/system.lazy-1?view=netframework-4.8
[send-port-filters]: ./../../../assets/images/SendPort.Filters.png

<!--
cSpell:ignore anization
-->
