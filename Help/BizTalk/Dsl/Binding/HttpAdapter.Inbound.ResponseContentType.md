#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[HttpAdapter](HttpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter').[Inbound](HttpAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Inbound')

## HttpAdapter.Inbound.ResponseContentType Property

Content type of the HTTP response messages that the HTTP adapter sends back to clients from this receive location.
This property is valid only for request-response receive ports and is ignored for one-way receive ports.

```csharp
public string ResponseContentType { get; set; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks
It defaults to [System.Net.Mime.MediaTypeNames.Text.Xml](https://docs.microsoft.com/en-us/dotnet/api/System.Net.Mime.MediaTypeNames.Text.Xml 'System.Net.Mime.MediaTypeNames.Text.Xml').