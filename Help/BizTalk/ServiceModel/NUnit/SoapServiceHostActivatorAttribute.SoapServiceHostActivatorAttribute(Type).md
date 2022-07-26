#### [Be.Stateless.BizTalk.ServiceModel.NUnit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.ServiceModel](Be.Stateless.BizTalk.Unit.ServiceModel.md 'Be.Stateless.BizTalk.Unit.ServiceModel').[SoapServiceHostActivatorAttribute](SoapServiceHostActivatorAttribute.md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivatorAttribute')

## SoapServiceHostActivatorAttribute(Type) Constructor

Creates a [SoapServiceHostActivatorAttribute](SoapServiceHostActivatorAttribute.md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivatorAttribute') that will ensure that the
[Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivator&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivator-2 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivator`2')-derived [System.ServiceModel.ServiceHost](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.ServiceHost 'System.ServiceModel.ServiceHost') activator
[Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost-2 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost`2')-derived [serviceHostActivator](SoapServiceHostActivatorAttribute.SoapServiceHostActivatorAttribute(Type).md#Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivatorAttribute.SoapServiceHostActivatorAttribute(System.Type).serviceHostActivator 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivatorAttribute.SoapServiceHostActivatorAttribute(System.Type).serviceHostActivator') is started before any NUnit-test
depending on it runs.

```csharp
public SoapServiceHostActivatorAttribute(System.Type serviceHostActivator);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivatorAttribute.SoapServiceHostActivatorAttribute(System.Type).serviceHostActivator'></a>

`serviceHostActivator` [System.Type](https://docs.microsoft.com/en-us/dotnet/api/System.Type 'System.Type')

The [System.Type](https://docs.microsoft.com/en-us/dotnet/api/System.Type 'System.Type') of the [Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost-2 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost`2')-derived host to activate.

### Remarks
Don't forget to [configure
            HTTP](https://docs.microsoft.com/en-us/dotnet/framework/wcf/feature-details/configuring-http-and-https 'https://docs.microsoft.com/en-us/dotnet/framework/wcf/feature-details/configuring-http-and-https'); e.g.:

```csharp
netsh http add urlacl url=http://+:8001/calculator user=$env:USERDOMAIN\$env:USERNAME!
```

### See Also
- [https://docs.microsoft.com/en-us/dotnet/framework/wcf/feature-details/configuring-http-and-https](https://docs.microsoft.com/en-us/dotnet/framework/wcf/feature-details/configuring-http-and-https 'https://docs.microsoft.com/en-us/dotnet/framework/wcf/feature-details/configuring-http-and-https')