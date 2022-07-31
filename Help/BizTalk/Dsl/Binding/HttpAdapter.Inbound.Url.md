#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[HttpAdapter](HttpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter').[Inbound](HttpAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Inbound')

## HttpAdapter.Inbound.Url Property

Specify the fully qualified URI for this receive location. The value for this property is a combination of the
server name and the virtual directory. The BizTalk Messaging Engine exposes this address to external partners. The
specified URI should designate the public Web site URL for trading partners to connect to when sending messages to
BizTalk Server.

```csharp
public System.Uri Url { get; set; }
```

#### Property Value
[System.Uri](https://docs.microsoft.com/en-us/dotnet/api/System.Uri 'System.Uri')

### Remarks
This information is optional and is not used by BizTalk Server. This parameter is available to allow
administrators to document the public URL that the receive location is tied to.