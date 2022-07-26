#### [Be.Stateless.BizTalk.ServiceModel.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.ServiceModel.Channels](Be.Stateless.BizTalk.Unit.ServiceModel.Channels.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Channels')

## IMessageService Interface

Defines a most-general contract that the [SoapStub](SoapStub.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.SoapStub') implements to be on the responding side of a
request-reply communication between messaging endpoints.

```csharp
public interface IMessageService
```

Derived  
&#8627; [SoapStub](SoapStub.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.SoapStub')

| Methods | |
| :--- | :--- |
| [Invoke(Message)](IMessageService.Invoke(Message).md 'Be.Stateless.BizTalk.Unit.ServiceModel.Channels.IMessageService.Invoke(System.ServiceModel.Channels.Message)') | Sends a [System.ServiceModel.Channels.Message](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.Message 'System.ServiceModel.Channels.Message')-based request and returns the correlated [System.ServiceModel.Channels.Message](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Channels.Message 'System.ServiceModel.Channels.Message')-based response. |
