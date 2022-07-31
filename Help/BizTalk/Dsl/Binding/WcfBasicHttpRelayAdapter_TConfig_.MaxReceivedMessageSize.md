#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfBasicHttpRelayAdapter&lt;TConfig&gt;](WcfBasicHttpRelayAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter<TConfig>')

## WcfBasicHttpRelayAdapter<TConfig>.MaxReceivedMessageSize Property

Specify the maximum size, in bytes, for a message including headers, which can be received on the wire. The size of
the messages is bounded by the amount of memory allocated for each message. You can use this property to limit
exposure to denial of service (DoS) attacks.

```csharp
public int MaxReceivedMessageSize { get; set; }
```

Implements [MaxReceivedMessageSize](IAdapterConfigMaxReceivedMessageSize.MaxReceivedMessageSize.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMaxReceivedMessageSize.MaxReceivedMessageSize')

#### Property Value
[System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

### Remarks

The WCF-BasicHttpRelay adapter leverages the [Microsoft.ServiceBus.BasicHttpRelayBinding](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.ServiceBus.BasicHttpRelayBinding 'Microsoft.ServiceBus.BasicHttpRelayBinding') class in the buffered transfer mode
to communicate with an endpoint. For the buffered transport mode, the [Microsoft.ServiceBus.BasicHttpRelayBinding](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.ServiceBus.BasicHttpRelayBinding 'Microsoft.ServiceBus.BasicHttpRelayBinding').[Microsoft.ServiceBus.BasicHttpRelayBinding.MaxBufferSize](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.ServiceBus.BasicHttpRelayBinding.MaxBufferSize 'Microsoft.ServiceBus.BasicHttpRelayBinding.MaxBufferSize') property is always equal to the value of this property.

It defaults to roughly [UInt16.MaxValue](https://docs.microsoft.com/en-us/dotnet/api/System.UInt16.MaxValue 'System.UInt16.MaxValue'), 65536.