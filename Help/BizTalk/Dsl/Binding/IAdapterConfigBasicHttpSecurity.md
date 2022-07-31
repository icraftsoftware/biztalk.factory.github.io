#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter')

## IAdapterConfigBasicHttpSecurity Interface

```csharp
public interface IAdapterConfigBasicHttpSecurity :
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSecurityMode<System.ServiceModel.BasicHttpSecurityMode>,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMessageSecurity<System.ServiceModel.BasicHttpMessageCredentialType>,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigTransportSecurity<System.ServiceModel.HttpClientCredentialType>
```

Derived  
&#8627; [WcfBasicHttpAdapter&lt;TAddress,TConfig&gt;](WcfBasicHttpAdapter_TAddress,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpAdapter<TAddress,TConfig>')

Implements [Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSecurityMode&lt;](IAdapterConfigSecurityMode_T_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSecurityMode<T>')[System.ServiceModel.BasicHttpSecurityMode](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.BasicHttpSecurityMode 'System.ServiceModel.BasicHttpSecurityMode')[&gt;](IAdapterConfigSecurityMode_T_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSecurityMode<T>'), [Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMessageSecurity&lt;](IAdapterConfigMessageSecurity_T_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMessageSecurity<T>')[System.ServiceModel.BasicHttpMessageCredentialType](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.BasicHttpMessageCredentialType 'System.ServiceModel.BasicHttpMessageCredentialType')[&gt;](IAdapterConfigMessageSecurity_T_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMessageSecurity<T>'), [Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigTransportSecurity&lt;](IAdapterConfigTransportSecurity_T_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigTransportSecurity<T>')[System.ServiceModel.HttpClientCredentialType](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.HttpClientCredentialType 'System.ServiceModel.HttpClientCredentialType')[&gt;](IAdapterConfigTransportSecurity_T_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigTransportSecurity<T>')