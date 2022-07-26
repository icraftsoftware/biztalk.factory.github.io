#### [Be.Stateless.BizTalk.ServiceModel.Unit](README.md 'README')
### [Be.Stateless.BizTalk](Be.Stateless.BizTalk.md 'Be.Stateless.BizTalk')

## IFluentInterface Interface

Interface that is used to build fluent interfaces by hiding methods declared by [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') from IntelliSense.

```csharp
public interface IFluentInterface
```

Derived  
&#8627; [ISolicitResponse](ISolicitResponse.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.ISolicitResponse')  
&#8627; [IOperationAbortResponseSetup&lt;TContract,TResult&gt;](IOperationAbortResponseSetup_TContract,TResult_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortResponseSetup<TContract,TResult>')  
&#8627; [IOperationAbortSetup&lt;TContract,TResult&gt;](IOperationAbortSetup_TContract,TResult_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortSetup<TContract,TResult>')  
&#8627; [IOperationAbortSetup&lt;TContract&gt;](IOperationAbortSetup_TContract_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationAbortSetup<TContract>')  
&#8627; [IOperationCallbackSetup&lt;TContract,TResult&gt;](IOperationCallbackSetup_TContract,TResult_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallbackSetup<TContract,TResult>')  
&#8627; [IOperationCallbackSetup&lt;TContract&gt;](IOperationCallbackSetup_TContract_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallbackSetup<TContract>')  
&#8627; [IOperationCallSetup&lt;TContract,TResult&gt;](IOperationCallSetup_TContract,TResult_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallSetup<TContract,TResult>')  
&#8627; [IOperationCallSetup&lt;TContract&gt;](IOperationCallSetup_TContract_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationCallSetup<TContract>')  
&#8627; [IOperationResponseSetup&lt;TContract,TResult&gt;](IOperationResponseSetup_TContract,TResult_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.IOperationResponseSetup<TContract,TResult>')  
&#8627; [ISetupActionOperation&lt;TContract&gt;](ISetupActionOperation_TContract_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupActionOperation<TContract>')  
&#8627; [ISetupFunctionOperation&lt;TContract&gt;](ISetupFunctionOperation_TContract_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupFunctionOperation<TContract>')  
&#8627; [ISetupOperation&lt;TContract&gt;](ISetupOperation_TContract_.md 'Be.Stateless.BizTalk.Unit.ServiceModel.Stub.Language.ISetupOperation<TContract>')

### Remarks
Code that consumes implementations of this interface should expect one of two things:
1. When referencing the interface from within the same solution (project reference), you will still see the methods this interface is meant to hide.
2. When referencing the interface through the compiled output assembly (external reference), the standard Object methods will be hidden as intended.
3. When using Resharper, be sure to configure it to respect the attribute: Options, go to Environment | IntelliSense | Completion Appearance and check "Filter members by [EditorBrowsable] attribute".
See https://kzu.github.io/IFluentInterface for more information.

| Methods | |
| :--- | :--- |
| [Equals(object)](IFluentInterface.Equals(object).md 'Be.Stateless.BizTalk.IFluentInterface.Equals(object)') | Redeclaration that hides the [System.Object.Equals(System.Object)](https://docs.microsoft.com/en-us/dotnet/api/System.Object.Equals#System_Object_Equals_System_Object_ 'System.Object.Equals(System.Object)') method from IntelliSense. |
| [GetHashCode()](IFluentInterface.GetHashCode().md 'Be.Stateless.BizTalk.IFluentInterface.GetHashCode()') | Redeclaration that hides the [System.Object.GetHashCode](https://docs.microsoft.com/en-us/dotnet/api/System.Object.GetHashCode 'System.Object.GetHashCode') method from IntelliSense. |
| [GetType()](IFluentInterface.GetType().md 'Be.Stateless.BizTalk.IFluentInterface.GetType()') | Redeclaration that hides the [System.Object.GetType](https://docs.microsoft.com/en-us/dotnet/api/System.Object.GetType 'System.Object.GetType') method from IntelliSense. |
| [ToString()](IFluentInterface.ToString().md 'Be.Stateless.BizTalk.IFluentInterface.ToString()') | Redeclaration that hides the [System.Object.ToString](https://docs.microsoft.com/en-us/dotnet/api/System.Object.ToString 'System.Object.ToString') method from IntelliSense. |
