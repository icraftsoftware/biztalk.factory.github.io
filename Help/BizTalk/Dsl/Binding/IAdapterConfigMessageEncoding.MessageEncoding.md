#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[IAdapterConfigMessageEncoding](IAdapterConfigMessageEncoding.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMessageEncoding')

## IAdapterConfigMessageEncoding.MessageEncoding Property

Specify the encoder used to encode the SOAP message.

```csharp
System.ServiceModel.WSMessageEncoding MessageEncoding { get; set; }
```

#### Property Value
[System.ServiceModel.WSMessageEncoding](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.WSMessageEncoding 'System.ServiceModel.WSMessageEncoding')

### Remarks

- [System.ServiceModel.WSMessageEncoding.Mtom](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.WSMessageEncoding.Mtom 'System.ServiceModel.WSMessageEncoding.Mtom') — Use a Message Transmission Optimization Mechanism 1.0 (MTOM) encoder.
- [System.ServiceModel.WSMessageEncoding.Text](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.WSMessageEncoding.Text 'System.ServiceModel.WSMessageEncoding.Text') — Use a text message encoder.

It defaults to [System.ServiceModel.WSMessageEncoding.Text](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.WSMessageEncoding.Text 'System.ServiceModel.WSMessageEncoding.Text').