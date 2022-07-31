#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfWebHttpAdapter](WcfWebHttpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter').[Inbound](WcfWebHttpAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter.Inbound')

## WcfWebHttpAdapter.Inbound.AddMessageBodyForHttpVerbs Property

Specify whether to add a empty payload message for some incoming HTTP request made for some HTTP verbs.

```csharp
public string AddMessageBodyForHttpVerbs { get; set; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks

List of coma separated HTTP Verbs.

Message body being added: 

```csharp
<WCF-WebHttpMessageBody xmlns="http://schemas.microsoft.com/BizTalk/2014/01/Adapters/WCF-WebHttp.EmptyMessage">
```