#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfSapAdapter](WcfSapAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter').[Inbound](WcfSapAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter.Inbound')

## WcfSapAdapter.Inbound.PadReceivedIdocWithSpaces Property

Determines whether the received IDoc, when in flat file format, has extra spaces at the end of each segment. This
is required if the flat file is converted to XML using the Flat File Parser pipeline component in BizTalk.

```csharp
public bool PadReceivedIdocWithSpaces { get; set; }
```

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks
The default is false; lines are not padded.