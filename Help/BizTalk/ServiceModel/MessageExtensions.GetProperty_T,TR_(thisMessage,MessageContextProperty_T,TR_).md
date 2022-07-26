#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel.Channels.Extensions](Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.md 'Be.Stateless.BizTalk.ServiceModel.Channels.Extensions').[MessageExtensions](MessageExtensions.md 'Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions')

## MessageExtensions.GetProperty<T,TR>(this Message, MessageContextProperty<T,TR>) Method

```csharp
public static TR GetProperty<T,TR>(this System.ServiceModel.Channels.Message message, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR> property)
    where T : Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase, new()
    where TR : struct, System.ValueType, System.ValueType;
```
#### Type parameters

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.GetProperty_T,TR_(thisSystem.ServiceModel.Channels.Message,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_).T'></a>

`T`

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.GetProperty_T,TR_(thisSystem.ServiceModel.Channels.Message,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_).TR'></a>

`TR`
#### Parameters

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.GetProperty_T,TR_(thisSystem.ServiceModel.Channels.Message,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_).message'></a>

`message` [System.ServiceModel.Channels.Message](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.Message 'System.ServiceModel.Channels.Message')

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.GetProperty_T,TR_(thisSystem.ServiceModel.Channels.Message,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_).property'></a>

`property` [Be.Stateless.BizTalk.ContextProperties.MessageContextProperty&lt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.MessageContextProperty-2 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty`2')[T](MessageExtensions.GetProperty_T,TR_(thisMessage,MessageContextProperty_T,TR_).md#Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.GetProperty_T,TR_(thisSystem.ServiceModel.Channels.Message,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_).T 'Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.GetProperty<T,TR>(this System.ServiceModel.Channels.Message, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>).T')[,](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.MessageContextProperty-2 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty`2')[TR](MessageExtensions.GetProperty_T,TR_(thisMessage,MessageContextProperty_T,TR_).md#Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.GetProperty_T,TR_(thisSystem.ServiceModel.Channels.Message,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_).TR 'Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.GetProperty<T,TR>(this System.ServiceModel.Channels.Message, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>).TR')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.MessageContextProperty-2 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty`2')

#### Returns
[TR](MessageExtensions.GetProperty_T,TR_(thisMessage,MessageContextProperty_T,TR_).md#Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.GetProperty_T,TR_(thisSystem.ServiceModel.Channels.Message,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_).TR 'Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.GetProperty<T,TR>(this System.ServiceModel.Channels.Message, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>).TR')