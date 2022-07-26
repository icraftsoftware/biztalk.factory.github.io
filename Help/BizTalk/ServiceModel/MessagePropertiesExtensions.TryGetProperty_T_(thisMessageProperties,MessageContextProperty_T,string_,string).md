#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel.Channels.Extensions](Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.md 'Be.Stateless.BizTalk.ServiceModel.Channels.Extensions').[MessagePropertiesExtensions](MessagePropertiesExtensions.md 'Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessagePropertiesExtensions')

## MessagePropertiesExtensions.TryGetProperty<T>(this MessageProperties, MessageContextProperty<T,string>, string) Method

```csharp
public static bool TryGetProperty<T>(this System.ServiceModel.Channels.MessageProperties properties, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,string> property, out string value)
    where T : Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase, new();
```
#### Type parameters

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessagePropertiesExtensions.TryGetProperty_T_(thisSystem.ServiceModel.Channels.MessageProperties,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,string_,string).T'></a>

`T`
#### Parameters

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessagePropertiesExtensions.TryGetProperty_T_(thisSystem.ServiceModel.Channels.MessageProperties,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,string_,string).properties'></a>

`properties` [System.ServiceModel.Channels.MessageProperties](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.MessageProperties 'System.ServiceModel.Channels.MessageProperties')

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessagePropertiesExtensions.TryGetProperty_T_(thisSystem.ServiceModel.Channels.MessageProperties,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,string_,string).property'></a>

`property` [Be.Stateless.BizTalk.ContextProperties.MessageContextProperty&lt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.MessageContextProperty-2 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty`2')[T](MessagePropertiesExtensions.TryGetProperty_T_(thisMessageProperties,MessageContextProperty_T,string_,string).md#Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessagePropertiesExtensions.TryGetProperty_T_(thisSystem.ServiceModel.Channels.MessageProperties,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,string_,string).T 'Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessagePropertiesExtensions.TryGetProperty<T>(this System.ServiceModel.Channels.MessageProperties, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,string>, string).T')[,](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.MessageContextProperty-2 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty`2')[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.MessageContextProperty-2 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty`2')

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessagePropertiesExtensions.TryGetProperty_T_(thisSystem.ServiceModel.Channels.MessageProperties,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,string_,string).value'></a>

`value` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')