#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfSapAdapter](WcfSapAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter').[Outbound](WcfSapAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter.Outbound')

## WcfSapAdapter.Outbound.AutoConfirmSentIdocs Property

Determines whether the adapter automatically calls RfcConfirmTransID() after sending an IDoc.

```csharp
public bool AutoConfirmSentIdocs { get; set; }
```

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks
Specifies whether the SAP adapter auto-commits tRFC client calls used for sending IDocs. The default is false;
auto-commit is disabled. If auto-commit is disabled, the client application must explicitly commit the tRFC call
by invoking the RfcConfirmTransID operation. The RfcConfirmTransID operation is a special operation surfaced by
the SAP adapter. It appears under the TRFC node when you use the Add Adapter Service Reference Visual Studio
Plug-in or the Consume Adapter Service BizTalk Project Add-in.