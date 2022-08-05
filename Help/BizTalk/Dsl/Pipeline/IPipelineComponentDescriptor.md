#### [Be.Stateless.BizTalk.Dsl.Pipeline](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Pipeline](Be.Stateless.BizTalk.Dsl.Pipeline.md 'Be.Stateless.BizTalk.Dsl.Pipeline')

## IPipelineComponentDescriptor Interface

Merge BizTalk Server pipeline component's interfaces that are used and required by Pipeline DSL.

```csharp
public interface IPipelineComponentDescriptor :
Microsoft.BizTalk.Component.Interop.IBaseComponent,
Microsoft.BizTalk.Component.Interop.IPersistPropertyBag,
Be.Stateless.BizTalk.Dsl.ITypeDescriptor,
Be.Stateless.BizTalk.Dsl.IVisitable<Be.Stateless.BizTalk.Dsl.Pipeline.IPipelineVisitor>
```

Implements [Microsoft.BizTalk.Component.Interop.IBaseComponent](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IBaseComponent 'Microsoft.BizTalk.Component.Interop.IBaseComponent'), [Microsoft.BizTalk.Component.Interop.IPersistPropertyBag](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPersistPropertyBag 'Microsoft.BizTalk.Component.Interop.IPersistPropertyBag'), [Be.Stateless.BizTalk.Dsl.ITypeDescriptor](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.ITypeDescriptor 'Be.Stateless.BizTalk.Dsl.ITypeDescriptor'), [Be.Stateless.BizTalk.Dsl.IVisitable&lt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.IVisitable-1 'Be.Stateless.BizTalk.Dsl.IVisitable`1')[IPipelineVisitor](IPipelineVisitor.md 'Be.Stateless.BizTalk.Dsl.Pipeline.IPipelineVisitor')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.IVisitable-1 'Be.Stateless.BizTalk.Dsl.IVisitable`1')

### Remarks
This interface is not meant to be used explicitly but only fulfills a Pipeline DSL scaffolding role and is meant
to be used in conjunction with [Be.Stateless.BizTalk.Dsl.Pipeline.PipelineComponentDescriptor&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.Pipeline.PipelineComponentDescriptor-1 'Be.Stateless.BizTalk.Dsl.Pipeline.PipelineComponentDescriptor`1').

| Properties | |
| :--- | :--- |
| [Properties](IPipelineComponentDescriptor.Properties.md 'Be.Stateless.BizTalk.Dsl.Pipeline.IPipelineComponentDescriptor.Properties') | |
| [PropertyContents](IPipelineComponentDescriptor.PropertyContents.md 'Be.Stateless.BizTalk.Dsl.Pipeline.IPipelineComponentDescriptor.PropertyContents') | |
