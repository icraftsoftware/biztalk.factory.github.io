#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[IAdapterConfigMessageEncoding](IAdapterConfigMessageEncoding.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMessageEncoding')

## IAdapterConfigMessageEncoding.TextEncoding Property

Specify the character set encoding to be used for emitting messages on the binding when the [MessageEncoding](IAdapterConfigMessageEncoding.MessageEncoding.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigMessageEncoding.MessageEncoding') property is set to [System.ServiceModel.WSMessageEncoding.Text](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.WSMessageEncoding.Text 'System.ServiceModel.WSMessageEncoding.Text').

```csharp
System.Text.Encoding TextEncoding { get; set; }
```

#### Property Value
[System.Text.Encoding](https://docs.microsoft.com/en-us/dotnet/api/System.Text.Encoding 'System.Text.Encoding')

### Remarks
It defaults to [System.Text.Encoding.UTF8](https://docs.microsoft.com/en-us/dotnet/api/System.Text.Encoding.UTF8 'System.Text.Encoding.UTF8').