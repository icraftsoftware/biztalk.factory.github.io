# Receive Location Binding

> **Downloads** The code samples used in this user guide have been made available in the [Be.Stateless.BizTalk.Factory.Samples][github.samples] GitHub repository.

Growing our `ReceivePort` binding [sample](./ReceivePort.md), let us add receive locations to handle the interactions with our `Billing` department and our external `Bank of Evil` banking company. Once again, the developer can choose between 2 alternate syntaxes to declare new receive locations: he can use fluent syntactic helpers or separate types.

## Fluent Declaration

Using the fluent API, we can add the `Credit Note Receive Location` to our `Billing Receive Port` as follows:

```csharp
public Application()
{
  ...
  ReceivePorts.Add(
    ReceivePort(
      rp => {
        rp.Name = "Billing Receive Port";
        rp.ReceiveLocations.Add(
          ReceiveLocation(
            rl => {
              rl.Name = "Credit Note Receive Location";
          })
        );
      })
    ...
  );
  ...
}
```

## Separate Type Declaration

If we prefer to declare a separate type for the `Bribe Receive Location` of our `Bank of Evil Receive Port` we can define the following class:

```csharp
using Be.Stateless.BizTalk.Dsl.Binding;

namespace Org.Anization.Accounting
{
  public class BribeReceiveLocation : ReceiveLocation
  {
    public BribeReceiveLocation()
    {
      Name = "Bribe Receive Location";
    }
  }
}
```

And add it to our `Bank of Evil Receive Port`'s collection of receive locations as follows:

```csharp
public class EvilBankReceivePort : ReceivePort
{
  public EvilBankReceivePort()
  {
    ...
    ReceiveLocations.Add(new BribeReceiveLocation());
    ...
  }
}
```

At this point, if we were to run the `ApplicationFixture`'s `GenerateApplicationBinding` test, it would fail complaining that it _Did not expect any exception, but found `Be.Stateless.BizTalk.Dsl.Binding.BindingException` with message "[...] Receive Location's Receive Pipeline is not defined."_

Let us configure a [receive pipeline](./Pipeline.md) for each of our receive locations.

The `ApplicationFixture` unit test however would still fail complaining now that it _Did not expect any exception, but found Be.Stateless.BizTalk.Dsl.Binding.BindingException with message "[...] Receive Location's Transport is not valid: Transport's Host is not defined."_

Let us too configure the [transport](./Transport.md) for each of our receive locations, which completes their configuration &mdash;at least up to a point where the `ApplicationFixture`'s tests are passing.

<!-- links -->

[github.samples]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Factory.Samples

<!--
cSpell:ignore Anization
-->
