#### [Be.Stateless.BizTalk.ServiceModel.NUnit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.ServiceModel](Be.Stateless.BizTalk.Unit.ServiceModel.md 'Be.Stateless.BizTalk.Unit.ServiceModel')

## SoapStubHostActivatorAttribute Class

Triggers the [Be.Stateless.BizTalk.Unit.ServiceModel.Stub.SoapStubHostActivator](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Unit.ServiceModel.Stub.SoapStubHostActivator 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.SoapStubHostActivator')-derived [System.ServiceModel.ServiceHost](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.ServiceHost 'System.ServiceModel.ServiceHost') activator meant to facilitate
NUnit-based unit testing requiring to interact with the [Be.Stateless.BizTalk.Unit.ServiceModel.Stub.SoapStub](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Unit.ServiceModel.Stub.SoapStub 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.SoapStub').

```csharp
public class SoapStubHostActivatorAttribute : Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivatorAttribute
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [System.Attribute](https://docs.microsoft.com/en-us/dotnet/api/System.Attribute 'System.Attribute') &#129106; [NUnit.Framework.TestActionAttribute](https://docs.microsoft.com/en-us/dotnet/api/NUnit.Framework.TestActionAttribute 'NUnit.Framework.TestActionAttribute') &#129106; [SoapServiceHostActivatorAttribute](SoapServiceHostActivatorAttribute.md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivatorAttribute') &#129106; SoapStubHostActivatorAttribute

### Remarks

[SoapStubHostActivatorAttribute](SoapStubHostActivatorAttribute.md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapStubHostActivatorAttribute') ensures that the [System.ServiceModel.ServiceHost](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.ServiceHost 'System.ServiceModel.ServiceHost') meant to be activated by the
            [Be.Stateless.BizTalk.Unit.ServiceModel.Stub.SoapStubHostActivator](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Unit.ServiceModel.Stub.SoapStubHostActivator 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.SoapStubHostActivator')-derived [System.ServiceModel.ServiceHost](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.ServiceHost 'System.ServiceModel.ServiceHost') activator is started before any NUnit-test
            depending on it runs.

Making use of this attribute therefore assumes and requires that unit tests are written on the basis of the NUnit
testing framework.

The in-process [Be.Stateless.BizTalk.Unit.ServiceModel.Stub.SoapStubHostActivator](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Unit.ServiceModel.Stub.SoapStubHostActivator 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.SoapStubHostActivator') will host the [Be.Stateless.BizTalk.Unit.ServiceModel.Stub.SoapStub](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Unit.ServiceModel.Stub.SoapStub 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.SoapStub') service's endpoint over the [System.ServiceModel.BasicHttpBinding](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.BasicHttpBinding 'System.ServiceModel.BasicHttpBinding') binding at the [SoapStubHostActivator.Uri](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Unit.ServiceModel.Stub.SoapStubHostActivator.Uri 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.SoapStubHostActivator.Uri') address,
i.e. `http://localhost:8000/soap-stub`.

### See Also
- [SoapServiceHostActivatorAttribute](SoapServiceHostActivatorAttribute.md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivatorAttribute')
- [Be.Stateless.BizTalk.Unit.ServiceModel.Stub.SoapStubHostActivator](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Unit.ServiceModel.Stub.SoapStubHostActivator 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.SoapStubHostActivator')
- [Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivator&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivator-2 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHostActivator`2')
- [Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost-2 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapServiceHost`2')
- [NUnit.Framework.ITestAction](https://docs.microsoft.com/en-us/dotnet/api/NUnit.Framework.ITestAction 'NUnit.Framework.ITestAction')
- [NUnit.Framework.TestActionAttribute](https://docs.microsoft.com/en-us/dotnet/api/NUnit.Framework.TestActionAttribute 'NUnit.Framework.TestActionAttribute')

| Properties | |
| :--- | :--- |
| [Targets](SoapStubHostActivatorAttribute.Targets.md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapStubHostActivatorAttribute.Targets') | |

| Methods | |
| :--- | :--- |
| [AfterTest(ITest)](SoapStubHostActivatorAttribute.AfterTest(ITest).md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapStubHostActivatorAttribute.AfterTest(NUnit.Framework.Interfaces.ITest)') | |
| [BeforeTest(ITest)](SoapStubHostActivatorAttribute.BeforeTest(ITest).md 'Be.Stateless.BizTalk.Unit.ServiceModel.SoapStubHostActivatorAttribute.BeforeTest(NUnit.Framework.Interfaces.ITest)') | |
