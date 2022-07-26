# Receive Port Binding

> **Downloads** The code samples used in this user guide have been made available in the [Be.Stateless.BizTalk.Factory.Samples][github.samples] GitHub repository.

Growing our `Application` binding [sample](./Application.md), let us add receive ports to handle the interactions with our `Billing` department and our external `Bank of Evil` banking company. The developer can choose between 2 alternate syntaxes to declare new receive ports: he can use fluent syntactic helpers or separate types.

## Fluent Declaration

Using the fluent API, we can add the `Billing` receive port to our `Accounting` application as follows:

```csharp
public Application()
{
  ...
  ReceivePorts.Add(ReceivePort(rp => rp.Name = "Billing Receive Port"));
  ...
}
```

## Separate Type Declaration

If we prefer to declare a separate type for the `Bank of Evil Receive Port` we can define the following class:

```csharp
using Be.Stateless.BizTalk.Dsl.Binding;

namespace Org.Anization.Accounting.ReceivePorts
{
  public class EvilBankReceivePort : ReceivePort
  {
    public EvilBankReceivePort()
    {
      Name = "Evil Bank Receive Port";
    }
  }
}
```

And add it to the collection of receive ports of our `Accounting` application as follows:

```csharp
public Application()
{
  ...
  ReceivePorts.Add(
    ReceivePort(rp => rp.Name = "Billing Receive Port"),
    new EvilBankReceivePort()
  );
  ...
}
```

Notice that since we have already written the `ApplicationFixture` test class, there is no need to define any additional test methods to validate our application bindings; all aspects of the entire application bindings are validated by this single test.

Now, if we were to execute this test, it would quite naturally fail complaining that it _Did not expect any exception, but found `Be.Stateless.BizTalk.Dsl.Binding.BindingException` with message "[Billing Receive Port] Receive Port's Receive Locations are not defined."_

Let us then have a look at how as a developer we can configure the [Receive Locations](./ReceiveLocation.md).

<!-- links -->

[github.samples]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Samples

<!--
cSpell:ignore Anization
-->
