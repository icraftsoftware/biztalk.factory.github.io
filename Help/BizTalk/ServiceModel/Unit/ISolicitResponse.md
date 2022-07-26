#### [Be.Stateless.BizTalk.ServiceModel.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.ServiceModel.Stub](Be.Stateless.BizTalk.Unit.ServiceModel.Stub.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub')

## ISolicitResponse Interface

A scaffolding interface to support setting up response against [Microsoft.BizTalk.Component.Interop.DocumentSpec](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.DocumentSpec 'Microsoft.BizTalk.Component.Interop.DocumentSpec') message type expectations. It
is not meant to be used in user code.

```csharp
public interface ISolicitResponse :
Be.Stateless.BizTalk.IFluentInterface
```

Implements [IFluentInterface](IFluentInterface.md 'Be.Stateless.BizTalk.IFluentInterface')

### See Also
- [SoapStub](SoapStub.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.SoapStub')

| Methods | |
| :--- | :--- |
| [Request(DocumentSpec)](ISolicitResponse.Request(DocumentSpec).md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.ISolicitResponse.Request(Microsoft.BizTalk.Component.Interop.DocumentSpec)') | A generic [Request(DocumentSpec)](ISolicitResponse.Request(DocumentSpec).md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.ISolicitResponse.Request(Microsoft.BizTalk.Component.Interop.DocumentSpec)') operation used to support the setting up of the response [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') to be returned upon the invocation of the [Request(DocumentSpec)](ISolicitResponse.Request(DocumentSpec).md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.ISolicitResponse.Request(Microsoft.BizTalk.Component.Interop.DocumentSpec)') operation with a message of some [Microsoft.BizTalk.Component.Interop.DocumentSpec](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.DocumentSpec 'Microsoft.BizTalk.Component.Interop.DocumentSpec') type. |
