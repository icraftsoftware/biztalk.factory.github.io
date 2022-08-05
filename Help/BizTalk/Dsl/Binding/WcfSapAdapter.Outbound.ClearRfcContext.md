#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfSapAdapter](WcfSapAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter').[Outbound](WcfSapAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter.Outbound')

## WcfSapAdapter.Outbound.ClearRfcContext Property

Determines whether the state acquired by the R/3 user context should be reset before returning a connection back
to the connection pool.

```csharp
public bool ClearRfcContext { get; set; }
```

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks
It defaults to `False`.