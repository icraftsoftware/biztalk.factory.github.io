#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[HttpAdapter](HttpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter').[Outbound](HttpAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Outbound')

## HttpAdapter.Outbound.RequestTimeout Property

Specify the time-out for the HTTP/HTTPS transmission. If the HTTP adapter does not receive the response within
this time, the service logs the error and resubmits the message based on the retry infrastructure.

```csharp
public System.TimeSpan RequestTimeout { get; set; }
```

#### Property Value
[System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan')

### Remarks
If set to zero (0), the BizTalk Messaging Engine calculates the time-out based on the request message size. If you
do not provide a value, the value for the handler is used.