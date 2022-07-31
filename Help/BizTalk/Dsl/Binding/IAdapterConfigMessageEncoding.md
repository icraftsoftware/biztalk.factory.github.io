#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter')

## IAdapterConfigMessageEncoding Interface

```csharp
public interface IAdapterConfigMessageEncoding
```

Derived  
&#8627; [WcfBasicHttpAdapter&lt;TAddress,TConfig&gt;](WcfBasicHttpAdapter_TAddress,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpAdapter<TAddress,TConfig>')  
&#8627; [WcfBasicHttpRelayAdapter&lt;TConfig&gt;](WcfBasicHttpRelayAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpRelayAdapter<TConfig>')  
&#8627; [WcfWSHttpAdapter&lt;TAddress,TConfig&gt;](WcfWSHttpAdapter_TAddress,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWSHttpAdapter<TAddress,TConfig>')

| Properties | |
| :--- | :--- |
| [MessageEncoding](IAdapterConfigMessageEncoding.MessageEncoding.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMessageEncoding.MessageEncoding') | Specify the encoder used to encode the SOAP message. |
| [TextEncoding](IAdapterConfigMessageEncoding.TextEncoding.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMessageEncoding.TextEncoding') | Specify the character set encoding to be used for emitting messages on the binding when the [MessageEncoding](IAdapterConfigMessageEncoding.MessageEncoding.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMessageEncoding.MessageEncoding') property is set to [System.ServiceModel.WSMessageEncoding.Text](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.WSMessageEncoding.Text 'System.ServiceModel.WSMessageEncoding.Text'). |
