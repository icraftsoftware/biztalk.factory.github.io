#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[SBMessagingAdapter](SBMessagingAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter').[Outbound](SBMessagingAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter.Outbound')

## SBMessagingAdapter.Outbound.CustomBrokeredPropertyNamespace Property

Specify the namespace that contains the BizTalk message context properties that you want to write as user-defined
Brokered Message properties on the outgoing message sent to the Service Bus Queue.

```csharp
public string CustomBrokeredPropertyNamespace { get; set; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks
All the properties that belong to the namespace are written to the message as user-defined Brokered Message
properties. The adapter ignores the namespace while writing the properties as Brokered Message properties. It uses
the namespace only to ascertain what properties to write.