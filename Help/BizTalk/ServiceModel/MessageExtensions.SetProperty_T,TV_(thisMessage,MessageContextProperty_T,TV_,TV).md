#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel.Channels.Extensions](Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.md 'Be.Stateless.BizTalk.ServiceModel.Channels.Extensions').[MessageExtensions](MessageExtensions.md 'Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions')

## MessageExtensions.SetProperty<T,TV>(this Message, MessageContextProperty<T,TV>, TV) Method

```csharp
public static void SetProperty<T,TV>(this System.ServiceModel.Channels.Message message, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TV> property, TV value)
    where T : Microsoft.XLANGs.BaseTypes.MessageContextPropertyBase, new()
    where TV : struct, System.ValueType, System.ValueType;
```
#### Type parameters

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.SetProperty_T,TV_(thisSystem.ServiceModel.Channels.Message,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_,TV).T'></a>

`T`

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.SetProperty_T,TV_(thisSystem.ServiceModel.Channels.Message,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_,TV).TV'></a>

`TV`
#### Parameters

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.SetProperty_T,TV_(thisSystem.ServiceModel.Channels.Message,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_,TV).message'></a>

`message` [System.ServiceModel.Channels.Message](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.Message 'System.ServiceModel.Channels.Message')

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.SetProperty_T,TV_(thisSystem.ServiceModel.Channels.Message,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_,TV).property'></a>

`property` [Be.Stateless.BizTalk.ContextProperties.MessageContextProperty&lt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.MessageContextProperty-2 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty`2')[T](MessageExtensions.SetProperty_T,TV_(thisMessage,MessageContextProperty_T,TV_,TV).md#Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.SetProperty_T,TV_(thisSystem.ServiceModel.Channels.Message,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_,TV).T 'Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.SetProperty<T,TV>(this System.ServiceModel.Channels.Message, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TV>, TV).T')[,](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.MessageContextProperty-2 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty`2')[TV](MessageExtensions.SetProperty_T,TV_(thisMessage,MessageContextProperty_T,TV_,TV).md#Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.SetProperty_T,TV_(thisSystem.ServiceModel.Channels.Message,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_,TV).TV 'Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.SetProperty<T,TV>(this System.ServiceModel.Channels.Message, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TV>, TV).TV')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.MessageContextProperty-2 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty`2')

<a name='Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.SetProperty_T,TV_(thisSystem.ServiceModel.Channels.Message,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_,TV).value'></a>

`value` [TV](MessageExtensions.SetProperty_T,TV_(thisMessage,MessageContextProperty_T,TV_,TV).md#Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.SetProperty_T,TV_(thisSystem.ServiceModel.Channels.Message,Be.Stateless.BizTalk.ContextProperties.MessageContextProperty_T,TV_,TV).TV 'Be.Stateless.BizTalk.ServiceModel.Channels.Extensions.MessageExtensions.SetProperty<T,TV>(this System.ServiceModel.Channels.Message, Be.Stateless.BizTalk.ContextProperties.MessageContextProperty<T,TV>, TV).TV')