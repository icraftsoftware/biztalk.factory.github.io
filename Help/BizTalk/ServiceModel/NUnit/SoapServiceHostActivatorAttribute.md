#### [Be.Stateless.BizTalk.ServiceModel.NUnit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.ServiceModel](Be.Stateless.BizTalk.Unit.ServiceModel.md 'Be.Stateless.BizTalk.Unit.ServiceModel')

## SoapServiceHostActivatorAttribute Class

Triggers the [Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivator&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivator-2 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivator`2')-derived [System.ServiceModel.ServiceHost](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.ServiceHost 'System.ServiceModel.ServiceHost') activator meant to
facilitate the NUnit-based unit testing of WCF services and their contracts.

```csharp
public class SoapServiceHostActivatorAttribute : NUnit.Framework.TestActionAttribute
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [System.Attribute](https://docs.microsoft.com/en-us/dotnet/api/System.Attribute 'System.Attribute') &#129106; [NUnit.Framework.TestActionAttribute](https://docs.microsoft.com/en-us/dotnet/api/NUnit.Framework.TestActionAttribute 'NUnit.Framework.TestActionAttribute') &#129106; SoapServiceHostActivatorAttribute

Derived  
&#8627; [SoapStubHostActivatorAttribute](SoapStubHostActivatorAttribute.md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapStubHostActivatorAttribute')

### Remarks

[SoapServiceHostActivatorAttribute](SoapServiceHostActivatorAttribute.md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivatorAttribute') ensures that the [System.ServiceModel.ServiceHost](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.ServiceHost 'System.ServiceModel.ServiceHost') meant to be activated by the
            [Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivator&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivator-2 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivator`2')-derived [System.ServiceModel.ServiceHost](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.ServiceHost 'System.ServiceModel.ServiceHost') activator is started before any
            NUnit-test depending on it runs.

Making use of this attribute therefore assumes and requires that unit tests are written on the basis of the NUnit
testing framework.

### See Also
- [Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivator&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivator-2 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivator`2')
- [Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost-2 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost`2')
- [NUnit.Framework.ITestAction](https://docs.microsoft.com/en-us/dotnet/api/NUnit.Framework.ITestAction 'NUnit.Framework.ITestAction')
- [NUnit.Framework.TestActionAttribute](https://docs.microsoft.com/en-us/dotnet/api/NUnit.Framework.TestActionAttribute 'NUnit.Framework.TestActionAttribute')

| Constructors | |
| :--- | :--- |
| [SoapServiceHostActivatorAttribute(Type)](SoapServiceHostActivatorAttribute.SoapServiceHostActivatorAttribute(Type).md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivatorAttribute.SoapServiceHostActivatorAttribute(System.Type)') | Creates a [SoapServiceHostActivatorAttribute](SoapServiceHostActivatorAttribute.md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivatorAttribute') that will ensure that the [Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivator&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivator-2 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivator`2')-derived [System.ServiceModel.ServiceHost](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.ServiceHost 'System.ServiceModel.ServiceHost') activator [Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost-2 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost`2')-derived [serviceHostActivator](SoapServiceHostActivatorAttribute.SoapServiceHostActivatorAttribute(Type).md#Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivatorAttribute.SoapServiceHostActivatorAttribute(System.Type).serviceHostActivator 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivatorAttribute.SoapServiceHostActivatorAttribute(System.Type).serviceHostActivator') is started before any NUnit-test depending on it runs. |

| Properties | |
| :--- | :--- |
| [ServiceHostActivator](SoapServiceHostActivatorAttribute.ServiceHostActivator.md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivatorAttribute.ServiceHostActivator') | |
| [Targets](SoapServiceHostActivatorAttribute.Targets.md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivatorAttribute.Targets') | |

| Methods | |
| :--- | :--- |
| [AfterTest(ITest)](SoapServiceHostActivatorAttribute.AfterTest(ITest).md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivatorAttribute.AfterTest(NUnit.Framework.Interfaces.ITest)') | |
| [BeforeTest(ITest)](SoapServiceHostActivatorAttribute.BeforeTest(ITest).md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivatorAttribute.BeforeTest(NUnit.Framework.Interfaces.ITest)') | |
