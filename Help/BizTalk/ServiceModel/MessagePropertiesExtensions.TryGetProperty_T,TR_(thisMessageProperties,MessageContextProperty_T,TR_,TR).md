#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel.Channels.Extensions](Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.md 'Be.Stateless.BizTalk.ServiceModel.Channels.Extensions').[MessagePropertiesExtensions](MessagePropertiesExtensions.md 'Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessagePropertiesExtensions')

## MessagePropertiesExtensions.TryGetProperty<T,TR>(this MessageProperties, MessageContextProperty<T,TR>, TR) Method

```csharp
public static bool TryGetProperty<T,TR>(this System.ServiceModel.Channels.MessageProperties properties, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR> property, out TR value)
    where T : Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase, new()
    where TR : struct, System.ValueType, System.ValueType;
```
#### Type parameters

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessagePropertiesExtensions.TryGetProperty_T,TR_(thisSystem.ServiceModel.Channels.MessageProperties,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_,TR).T'></a>

`T`

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessagePropertiesExtensions.TryGetProperty_T,TR_(thisSystem.ServiceModel.Channels.MessageProperties,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_,TR).TR'></a>

`TR`
#### Parameters

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessagePropertiesExtensions.TryGetProperty_T,TR_(thisSystem.ServiceModel.Channels.MessageProperties,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_,TR).properties'></a>

`properties` [System.ServiceModel.Channels.MessageProperties](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.MessageProperties 'System.ServiceModel.Channels.MessageProperties')

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessagePropertiesExtensions.TryGetProperty_T,TR_(thisSystem.ServiceModel.Channels.MessageProperties,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_,TR).property'></a>

`property` [Be.Stateless.BizTalk.ContextProperties.MessageContextProperty&lt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.MessageContextProperty-2 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty`2')[T](MessagePropertiesExtensions.TryGetProperty_T,TR_(thisMessageProperties,MessageContextProperty_T,TR_,TR).md#Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessagePropertiesExtensions.TryGetProperty_T,TR_(thisSystem.ServiceModel.Channels.MessageProperties,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_,TR).T 'Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessagePropertiesExtensions.TryGetProperty<T,TR>(this System.ServiceModel.Channels.MessageProperties, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>, TR).T')[,](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.MessageContextProperty-2 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty`2')[TR](MessagePropertiesExtensions.TryGetProperty_T,TR_(thisMessageProperties,MessageContextProperty_T,TR_,TR).md#Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessagePropertiesExtensions.TryGetProperty_T,TR_(thisSystem.ServiceModel.Channels.MessageProperties,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_,TR).TR 'Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessagePropertiesExtensions.TryGetProperty<T,TR>(this System.ServiceModel.Channels.MessageProperties, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>, TR).TR')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.MessageContextProperty-2 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty`2')

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessagePropertiesExtensions.TryGetProperty_T,TR_(thisSystem.ServiceModel.Channels.MessageProperties,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_,TR).value'></a>

`value` [TR](MessagePropertiesExtensions.TryGetProperty_T,TR_(thisMessageProperties,MessageContextProperty_T,TR_,TR).md#Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessagePropertiesExtensions.TryGetProperty_T,TR_(thisSystem.ServiceModel.Channels.MessageProperties,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_,TR).TR 'Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessagePropertiesExtensions.TryGetProperty<T,TR>(this System.ServiceModel.Channels.MessageProperties, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>, TR).TR')

#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')