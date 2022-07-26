#### [Be.Stateless.BizTalk.ServiceModel.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.ServiceModel.Stub](Be.Stateless.BizTalk.Unit.ServiceModel.Stub.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub').[ISolicitResponse](ISolicitResponse.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.ISolicitResponse')

## ISolicitResponse.Request(DocumentSpec) Method

A generic [Request(DocumentSpec)](ISolicitResponse.Request(DocumentSpec).md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.ISolicitResponse.Request(Microsoft.BizTalk.Component.Interop.DocumentSpec)') operation used to support the setting up of the response [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') to be returned upon the invocation of the [Request(DocumentSpec)](ISolicitResponse.Request(DocumentSpec).md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.ISolicitResponse.Request(Microsoft.BizTalk.Component.Interop.DocumentSpec)') operation
with a message of some [Microsoft.BizTalk.Component.Interop.DocumentSpec](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.DocumentSpec 'Microsoft.BizTalk.Component.Interop.DocumentSpec') type.

```csharp
System.IO.Stream Request(Microsoft.BizTalk.Component.Interop.DocumentSpec documentSpec);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Unit.ServiceModel.Stub.ISolicitResponse.Request(Microsoft.BizTalk.Component.Interop.DocumentSpec).documentSpec'></a>

`documentSpec` [Microsoft.BizTalk.Component.Interop.DocumentSpec](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.DocumentSpec 'Microsoft.BizTalk.Component.Interop.DocumentSpec')

The expected [Microsoft.BizTalk.Component.Interop.DocumentSpec](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.DocumentSpec 'Microsoft.BizTalk.Component.Interop.DocumentSpec') of some incoming message for which a response needs to be setup.

#### Returns
[System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')  
The response message [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream').