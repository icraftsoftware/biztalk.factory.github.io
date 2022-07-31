#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter')

## AdapterBase Class

```csharp
public abstract class AdapterBase :
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter,
Be.Stateless.BizTalk.Dsl.ISupportValidation
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; AdapterBase

Derived  
&#8627; [FileAdapter](FileAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter')  
&#8627; [HttpAdapter](HttpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter')  
&#8627; [LegacyAdapterBase](LegacyAdapterBase.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.LegacyAdapterBase')  
&#8627; [Office365EmailAdapter&lt;TConfig&gt;](Office365EmailAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter<TConfig>')  
&#8627; [SBMessagingAdapter&lt;TConfig&gt;](SBMessagingAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SBMessagingAdapter<TConfig>')  
&#8627; [SftpAdapter&lt;TConfig&gt;](SftpAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.SftpAdapter<TConfig>')  
&#8627; [WcfAdapterBase&lt;TAddress,TBinding,TConfig&gt;](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')

Implements [IAdapter](IAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter'), [Be.Stateless.BizTalk.Dsl.ISupportValidation](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.ISupportValidation 'Be.Stateless.BizTalk.Dsl.ISupportValidation')

| Constructors | |
| :--- | :--- |
| [AdapterBase(ProtocolType)](AdapterBase.AdapterBase(ProtocolType).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase.AdapterBase(Microsoft.BizTalk.Deployment.Binding.ProtocolType)') | |

| Methods | |
| :--- | :--- |
| [BuildTimeSpan(int, PollingIntervalUnit)](AdapterBase.BuildTimeSpan(int,PollingIntervalUnit).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase.BuildTimeSpan(int, Microsoft.BizTalk.Adapter.Sftp.PollingIntervalUnit)') | |
| [GetAddress()](AdapterBase.GetAddress().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase.GetAddress()') | |
| [GetProtocolTypeFromConfigurationClassId(Guid)](AdapterBase.GetProtocolTypeFromConfigurationClassId(Guid).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase.GetProtocolTypeFromConfigurationClassId(System.Guid)') | |
| [GetPublicAddress()](AdapterBase.GetPublicAddress().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase.GetPublicAddress()') | |
| [Save(IPropertyBag)](AdapterBase.Save(IPropertyBag).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase.Save(Microsoft.BizTalk.Component.Interop.IPropertyBag)') | |
| [UnbuildTimeSpan(TimeSpan, Action&lt;int,PollingIntervalUnit&gt;)](AdapterBase.UnbuildTimeSpan(TimeSpan,Action_int,PollingIntervalUnit_).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase.UnbuildTimeSpan(System.TimeSpan, System.Action<int,Microsoft.BizTalk.Adapter.Sftp.PollingIntervalUnit>)') | |
| [Validate()](AdapterBase.Validate().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase.Validate()') | |

| Explicit Interface Implementations | |
| :--- | :--- |
| [Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter.Address](AdapterBase.Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter.Address.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase.Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter.Address') | |
| [Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter.ProtocolType](AdapterBase.Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter.ProtocolType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase.Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter.ProtocolType') | |
| [Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter.PublicAddress](AdapterBase.Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter.PublicAddress.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase.Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter.PublicAddress') | |
| [Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter.Save(IPropertyBag)](AdapterBase.Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter.Save(IPropertyBag).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase.Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter.Save(Microsoft.BizTalk.Component.Interop.IPropertyBag)') | |
| [Be.Stateless.BizTalk.Dsl.ISupportValidation.Validate()](AdapterBase.Be.Stateless.BizTalk.Dsl.ISupportValidation.Validate().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase.Be.Stateless.BizTalk.Dsl.ISupportValidation.Validate()') | |
