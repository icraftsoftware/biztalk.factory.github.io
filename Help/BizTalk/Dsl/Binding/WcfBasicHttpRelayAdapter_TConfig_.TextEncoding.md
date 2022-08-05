#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfBasicHttpRelayAdapter&lt;TConfig&gt;](WcfBasicHttpRelayAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter<TConfig>')

## WcfBasicHttpRelayAdapter<TConfig>.TextEncoding Property

Specify the character set encoding to be used for emitting messages on the binding when the [MessageEncoding](WcfBasicHttpRelayAdapter_TConfig_.MessageEncoding.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter<TConfig>.MessageEncoding') property is set to [System.ServiceModel.WSMessageEncoding.Text](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.WSMessageEncoding.Text 'System.ServiceModel.WSMessageEncoding.Text').

```csharp
public System.Text.Encoding TextEncoding { get; set; }
```

Implements [TextEncoding](IAdapterConfigMessageEncoding.TextEncoding.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMessageEncoding.TextEncoding')

#### Property Value
[System.Text.Encoding](https://docs.microsoft.com/en-us/dotnet/api/System.Text.Encoding 'System.Text.Encoding')

### Remarks

Valid values include the following:
- [System.Text.Encoding.BigEndianUnicode](https://docs.microsoft.com/en-us/dotnet/api/System.Text.Encoding.BigEndianUnicode 'System.Text.Encoding.BigEndianUnicode')
- [System.Text.Encoding.Unicode](https://docs.microsoft.com/en-us/dotnet/api/System.Text.Encoding.Unicode 'System.Text.Encoding.Unicode')
- [System.Text.Encoding.UTF8](https://docs.microsoft.com/en-us/dotnet/api/System.Text.Encoding.UTF8 'System.Text.Encoding.UTF8')

It defaults to [System.Text.Encoding.UTF8](https://docs.microsoft.com/en-us/dotnet/api/System.Text.Encoding.UTF8 'System.Text.Encoding.UTF8').