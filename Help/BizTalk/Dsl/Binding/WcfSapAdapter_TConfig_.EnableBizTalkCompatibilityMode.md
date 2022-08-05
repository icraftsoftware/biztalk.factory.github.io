#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfSapAdapter&lt;TConfig&gt;](WcfSapAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter<TConfig>')

## WcfSapAdapter<TConfig>.EnableBizTalkCompatibilityMode Property

Specifies whether the BizTalk Layered Channel Binding Element should be loaded. The BizTalk Layered Channel Binding
Element is loaded to enable BizTalk transactions to flow through the SAP adapter to the SAP system.

```csharp
public bool EnableBizTalkCompatibilityMode { get; set; }
```

Implements [EnableBizTalkCompatibilityMode](IAdapterConfigBizTalkCompatibilityMode.EnableBizTalkCompatibilityMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigBizTalkCompatibilityMode.EnableBizTalkCompatibilityMode')

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks

Set this to `True` to load the binding element. Otherwise, set this to `False`.

When using the adapters from BizTalk Server, you must always set the property to true. When using the adapters from
Visual Studio, you must always set the property to false.