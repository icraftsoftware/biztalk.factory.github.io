#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel.Channels.Extensions](Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.md 'Be.Stateless.BizTalk.ServiceModel.Channels.Extensions').[MessagePropertiesExtensions](MessagePropertiesExtensions.md 'Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessagePropertiesExtensions')

## MessagePropertiesExtensions.GetProperty<T,TR>(this MessageProperties, MessageContextProperty<T,TR>) Method

```csharp
public static TR GetProperty<T,TR>(this System.ServiceModel.Channels.MessageProperties properties, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR> property)
    where T : Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase, new()
    where TR : struct, System.ValueType, System.ValueType;
```
#### Type parameters

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessagePropertiesExtensions.GetProperty_T,TR_(thisSystem.ServiceModel.Channels.MessageProperties,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_).T'></a>

`T`

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessagePropertiesExtensions.GetProperty_T,TR_(thisSystem.ServiceModel.Channels.MessageProperties,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_).TR'></a>

`TR`
#### Parameters

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessagePropertiesExtensions.GetProperty_T,TR_(thisSystem.ServiceModel.Channels.MessageProperties,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_).properties'></a>

`properties` [System.ServiceModel.Channels.MessageProperties](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.MessageProperties 'System.ServiceModel.Channels.MessageProperties')

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessagePropertiesExtensions.GetProperty_T,TR_(thisSystem.ServiceModel.Channels.MessageProperties,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_).property'></a>

`property` [Be.Stateless.BizTalk.ContextProperties.MessageContextProperty&lt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.MessageContextProperty-2 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty`2')[T](MessagePropertiesExtensions.GetProperty_T,TR_(thisMessageProperties,MessageContextProperty_T,TR_).md#Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessagePropertiesExtensions.GetProperty_T,TR_(thisSystem.ServiceModel.Channels.MessageProperties,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_).T 'Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessagePropertiesExtensions.GetProperty<T,TR>(this System.ServiceModel.Channels.MessageProperties, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>).T')[,](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.MessageContextProperty-2 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty`2')[TR](MessagePropertiesExtensions.GetProperty_T,TR_(thisMessageProperties,MessageContextProperty_T,TR_).md#Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessagePropertiesExtensions.GetProperty_T,TR_(thisSystem.ServiceModel.Channels.MessageProperties,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_).TR 'Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessagePropertiesExtensions.GetProperty<T,TR>(this System.ServiceModel.Channels.MessageProperties, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>).TR')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.MessageContextProperty-2 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty`2')

#### Returns
[TR](MessagePropertiesExtensions.GetProperty_T,TR_(thisMessageProperties,MessageContextProperty_T,TR_).md#Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessagePropertiesExtensions.GetProperty_T,TR_(thisSystem.ServiceModel.Channels.MessageProperties,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TR_).TR 'Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessagePropertiesExtensions.GetProperty<T,TR>(this System.ServiceModel.Channels.MessageProperties, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TR>).TR')