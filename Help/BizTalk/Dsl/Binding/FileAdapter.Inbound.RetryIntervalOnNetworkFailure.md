#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[FileAdapter](FileAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter').[Inbound](FileAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter.Inbound')

## FileAdapter.Inbound.RetryIntervalOnNetworkFailure Property

Specify the retry interval time (in minutes) between attempts to access the receive location on the network share
if it is temporarily unavailable.

```csharp
public System.TimeSpan RetryIntervalOnNetworkFailure { get; set; }
```

#### Property Value
[System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/System.TimeSpan 'System.TimeSpan')