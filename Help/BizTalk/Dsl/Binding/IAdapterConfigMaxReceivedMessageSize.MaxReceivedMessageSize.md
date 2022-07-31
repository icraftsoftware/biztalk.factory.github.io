#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[IAdapterConfigMaxReceivedMessageSize](IAdapterConfigMaxReceivedMessageSize.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMaxReceivedMessageSize')

## IAdapterConfigMaxReceivedMessageSize.MaxReceivedMessageSize Property

Specify the maximum size, in bytes, for a message (including headers) that can be received on the wire. The size of
the messages is bounded by the amount of memory allocated for each message. You can use this property to limit
exposure to denial of service (DoS) attacks.

```csharp
int MaxReceivedMessageSize { get; set; }
```

#### Property Value
[System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

### Remarks
It defaults to roughly [UInt16.MaxValue](https://docs.microsoft.com/en-us/dotnet/api/System.UInt16.MaxValue 'System.UInt16.MaxValue'), 65536.