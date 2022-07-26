#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel.Channels.Extensions](Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.md 'Be.Stateless.BizTalk.ServiceModel.Channels.Extensions').[MessageExtensions](MessageExtensions.md 'Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions')

## MessageExtensions.TryGetProperty<T,TR>(this Message, MessageContextProperty<T,TR>, TR) Method

```csharp
public static bool TryGetProperty<T,TR>(this System.ServiceModel.Channels.Message message, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR> property, out TR value)
    where T : Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase, new()
    where TR : struct, System.ValueType, System.ValueType;
```
#### Type parameters

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.TryGetProperty_T,TR_(thisSystem.ServiceModel.Channels.Message,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_,TR).T'></a>

`T`

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.TryGetProperty_T,TR_(thisSystem.ServiceModel.Channels.Message,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_,TR).TR'></a>

`TR`
#### Parameters

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.TryGetProperty_T,TR_(thisSystem.ServiceModel.Channels.Message,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_,TR).message'></a>

`message` [System.ServiceModel.Channels.Message](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.Message 'System.ServiceModel.Channels.Message')

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.TryGetProperty_T,TR_(thisSystem.ServiceModel.Channels.Message,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_,TR).property'></a>

`property` [Be.Stateless.BizTalk.ContextProperties.MessageContextProperty&lt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.MessageContextProperty-2 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty`2')[T](MessageExtensions.TryGetProperty_T,TR_(thisMessage,MessageContextProperty_T,TR_,TR).md#Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.TryGetProperty_T,TR_(thisSystem.ServiceModel.Channels.Message,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_,TR).T 'Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.TryGetProperty<T,TR>(this System.ServiceModel.Channels.Message, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>, TR).T')[,](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.MessageContextProperty-2 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty`2')[TR](MessageExtensions.TryGetProperty_T,TR_(thisMessage,MessageContextProperty_T,TR_,TR).md#Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.TryGetProperty_T,TR_(thisSystem.ServiceModel.Channels.Message,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_,TR).TR 'Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.TryGetProperty<T,TR>(this System.ServiceModel.Channels.Message, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>, TR).TR')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.MessageContextProperty-2 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty`2')

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.TryGetProperty_T,TR_(thisSystem.ServiceModel.Channels.Message,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_,TR).value'></a>

`value` [TR](MessageExtensions.TryGetProperty_T,TR_(thisMessage,MessageContextProperty_T,TR_,TR).md#Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.TryGetProperty_T,TR_(thisSystem.ServiceModel.Channels.Message,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_,TR).TR 'Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.TryGetProperty<T,TR>(this System.ServiceModel.Channels.Message, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>, TR).TR')

#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')