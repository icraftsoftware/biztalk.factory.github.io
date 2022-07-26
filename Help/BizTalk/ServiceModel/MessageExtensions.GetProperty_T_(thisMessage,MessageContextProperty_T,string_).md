#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel.Channels.Extensions](Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.md 'Be.Stateless.BizTalk.ServiceModel.Channels.Extensions').[MessageExtensions](MessageExtensions.md 'Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions')

## MessageExtensions.GetProperty<T>(this Message, MessageContextProperty<T,string>) Method

```csharp
public static string GetProperty<T>(this System.ServiceModel.Channels.Message message, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,string> property)
    where T : Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase, new();
```
#### Type parameters

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.GetProperty_T_(thisSystem.ServiceModel.Channels.Message,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,string_).T'></a>

`T`
#### Parameters

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.GetProperty_T_(thisSystem.ServiceModel.Channels.Message,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,string_).message'></a>

`message` [System.ServiceModel.Channels.Message](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.Message 'System.ServiceModel.Channels.Message')

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.GetProperty_T_(thisSystem.ServiceModel.Channels.Message,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,string_).property'></a>

`property` [Be.Stateless.BizTalk.ContextProperties.MessageContextProperty&lt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.MessageContextProperty-2 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty`2')[T](MessageExtensions.GetProperty_T_(thisMessage,MessageContextProperty_T,string_).md#Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.GetProperty_T_(thisSystem.ServiceModel.Channels.Message,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,string_).T 'Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.GetProperty<T>(this System.ServiceModel.Channels.Message, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,string>).T')[,](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.MessageContextProperty-2 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty`2')[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.MessageContextProperty-2 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty`2')

#### Returns
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')