#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfSapAdapter](WcfSapAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter').[Inbound](WcfSapAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter.Inbound')

## WcfSapAdapter.Inbound.ReceiveIdocFormat Property

Determines the XML format of the incoming (from SAP) IDoc

```csharp
public Microsoft.Adapters.SAP.IdocReceiveFormat ReceiveIdocFormat { get; set; }
```

#### Property Value
[Microsoft.Adapters.SAP.IdocReceiveFormat](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.Adapters.SAP.IdocReceiveFormat 'Microsoft.Adapters.SAP.IdocReceiveFormat')

### Remarks
There are three possible values for the ReceiveIDocFormat property:
- [Microsoft.Adapters.SAP.IdocReceiveFormat.String](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.Adapters.SAP.IdocReceiveFormat.String 'Microsoft.Adapters.SAP.IdocReceiveFormat.String') specifies that the IDoc message should be represented as a single, string
              field in the WCF message.
- [Microsoft.Adapters.SAP.IdocReceiveFormat.Typed](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.Adapters.SAP.IdocReceiveFormat.Typed 'Microsoft.Adapters.SAP.IdocReceiveFormat.Typed') specifies that the IDoc message should be parsed and represented as a
              strongly-typed WCF message.
- [Microsoft.Adapters.SAP.IdocReceiveFormat.Rfc](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.Adapters.SAP.IdocReceiveFormat.Rfc 'Microsoft.Adapters.SAP.IdocReceiveFormat.Rfc') specifies that the SAP adapter should pass the incoming RFC call as a WCF
              message with RFC parameters.

The default is [Microsoft.Adapters.SAP.IdocReceiveFormat.Typed](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.Adapters.SAP.IdocReceiveFormat.Typed 'Microsoft.Adapters.SAP.IdocReceiveFormat.Typed').