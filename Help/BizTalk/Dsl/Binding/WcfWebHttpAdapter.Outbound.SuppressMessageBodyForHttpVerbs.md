#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfWebHttpAdapter](WcfWebHttpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter').[Outbound](WcfWebHttpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter.Outbound')

## WcfWebHttpAdapter.Outbound.SuppressMessageBodyForHttpVerbs Property

Specify whether to remove the message payload for outgoing HTTP request made for some HTTP verbs.

```csharp
public string SuppressMessageBodyForHttpVerbs { get; set; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks

Based on the verb you use to invoke a REST endpoint, you may or may not require a message payload. For example,
you may not need a message payload while using the GET or DELETE verbs. However, to trigger a call to the REST
endpoint using the send port, you may use a dummy message that includes a message payload. Before the message is
sent to the REST endpoint, the message payload from the dummy message must be removed. You can specify the verbs
for which the message payload must be removed using the Suppress Body for Verbs property.

For example, if you want to remove the message payload while using a GET verb, specify the value for this property
as GET.