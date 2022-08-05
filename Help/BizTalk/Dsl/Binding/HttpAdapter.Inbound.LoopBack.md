#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[HttpAdapter](HttpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter').[Inbound](HttpAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Inbound')

## HttpAdapter.Inbound.LoopBack Property

Specifies that the request message received on this location will be routed either to a send port or back to the
receive location to be sent as a response. This property is valid only for request-response receive ports. It is
ignored for one-way receive ports.

```csharp
public bool LoopBack { get; set; }
```

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks
It defaults to `False`.