#### [Be.Stateless.BizTalk.Schemas](README.md 'README')
### [Be.Stateless.BizTalk.ContextProperties.Subscribable](Be.Stateless.BizTalk.ContextProperties.Subscribable.md 'Be.Stateless.BizTalk.ContextProperties.Subscribable').[BizTalkFactoryProperties](BizTalkFactoryProperties.md 'Be.Stateless.BizTalk.ContextProperties.Subscribable.BizTalkFactoryProperties')

## BizTalkFactoryProperties.EnvironmentTag Field

To be used when one application has to be connected to several distinct sets of interacting parties and cannot leak
messages from one set of parties into another. In concrete terms, to be used in pub/sub of messages in order to keep
them strictly insulated within an individual set of such interacting parties.

```csharp
public static readonly MessageContextProperty<EnvironmentTag,string> EnvironmentTag;
```

#### Field Value
[Be.Stateless.BizTalk.ContextProperties.MessageContextProperty&lt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.MessageContextProperty-2 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty`2')[Be.Stateless.BizTalk.Schemas.BizTalkFactory.EnvironmentTag](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Schemas.BizTalkFactory.EnvironmentTag 'Be.Stateless.BizTalk.Schemas.BizTalkFactory.EnvironmentTag')[,](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.MessageContextProperty-2 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty`2')[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.MessageContextProperty-2 'Be.Stateless.BizTalk.ContextProperties.MessageContextProperty`2')