#### [Be.Stateless.BizTalk.Dsl.Pipeline](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Pipeline](Be.Stateless.BizTalk.Dsl.Pipeline.md 'Be.Stateless.BizTalk.Dsl.Pipeline')

## Pipeline<T> Class

```csharp
public abstract class Pipeline<T> :
Be.Stateless.BizTalk.IFluentInterface,
Be.Stateless.BizTalk.Dsl.IVisitable<Be.Stateless.BizTalk.Dsl.Pipeline.IPipelineVisitor>
    where T : Be.Stateless.BizTalk.Dsl.Pipeline.IPipelineStageList
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Dsl.Pipeline.Pipeline_T_.T'></a>

`T`

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; Pipeline<T>

Derived  
&#8627; [ReceivePipeline](ReceivePipeline.md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline')  
&#8627; [SendPipeline](SendPipeline.md 'Be.Stateless.BizTalk.Dsl.Pipeline.SendPipeline')

Implements [Be.Stateless.BizTalk.IFluentInterface](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.IFluentInterface 'Be.Stateless.BizTalk.IFluentInterface'), [Be.Stateless.BizTalk.Dsl.IVisitable&lt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.IVisitable-1 'Be.Stateless.BizTalk.Dsl.IVisitable`1')[IPipelineVisitor](IPipelineVisitor.md 'Be.Stateless.BizTalk.Dsl.Pipeline.IPipelineVisitor')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.IVisitable-1 'Be.Stateless.BizTalk.Dsl.IVisitable`1')

| Constructors | |
| :--- | :--- |
| [Pipeline(T)](Pipeline_T_.Pipeline(T).md 'Be.Stateless.BizTalk.Dsl.Pipeline.Pipeline<T>.Pipeline(T)') | |

| Properties | |
| :--- | :--- |
| [Description](Pipeline_T_.Description.md 'Be.Stateless.BizTalk.Dsl.Pipeline.Pipeline<T>.Description') | |
| [Stages](Pipeline_T_.Stages.md 'Be.Stateless.BizTalk.Dsl.Pipeline.Pipeline<T>.Stages') | |
| [Version](Pipeline_T_.Version.md 'Be.Stateless.BizTalk.Dsl.Pipeline.Pipeline<T>.Version') | |
| [VersionDependentGuid](Pipeline_T_.VersionDependentGuid.md 'Be.Stateless.BizTalk.Dsl.Pipeline.Pipeline<T>.VersionDependentGuid') | |

| Methods | |
| :--- | :--- |
| [Equals(object)](Pipeline_T_.Equals(object).md 'Be.Stateless.BizTalk.Dsl.Pipeline.Pipeline<T>.Equals(object)') | |
| [GetHashCode()](Pipeline_T_.GetHashCode().md 'Be.Stateless.BizTalk.Dsl.Pipeline.Pipeline<T>.GetHashCode()') | |
| [ToString()](Pipeline_T_.ToString().md 'Be.Stateless.BizTalk.Dsl.Pipeline.Pipeline<T>.ToString()') | |

| Explicit Interface Implementations | |
| :--- | :--- |
| [Be.Stateless.BizTalk.Dsl.IVisitable&lt;Be.Stateless.BizTalk.Dsl.Pipeline.IPipelineVisitor&gt;.Accept&lt;T1&gt;(T1)](Pipeline_T_.Be.Stateless.BizTalk.Dsl.IVisitable_Be.Stateless.BizTalk.Dsl.Pipeline.IPipelineVisitor_.Accept_T1_(T1).md 'Be.Stateless.BizTalk.Dsl.Pipeline.Pipeline<T>.Be.Stateless.BizTalk.Dsl.IVisitable<Be.Stateless.BizTalk.Dsl.Pipeline.IPipelineVisitor>.Accept<T1>(T1)') | |
| [Be.Stateless.BizTalk.IFluentInterface.GetType()](Pipeline_T_.Be.Stateless.BizTalk.IFluentInterface.GetType().md 'Be.Stateless.BizTalk.Dsl.Pipeline.Pipeline<T>.Be.Stateless.BizTalk.IFluentInterface.GetType()') | |
