#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Visitor](Be.Stateless.BizTalk.Dsl.Binding.Visitor.md 'Be.Stateless.BizTalk.Dsl.Binding.Visitor')

## BindingInfoBuilder Class

[IApplicationBindingVisitor](IApplicationBindingVisitor.md 'Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor') implementation that generates BizTalk Server bindings file.

```csharp
public class BindingInfoBuilder :
Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; BindingInfoBuilder

Implements [IApplicationBindingVisitor](IApplicationBindingVisitor.md 'Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor')

### Remarks

See [Microsoft.BizTalk.Deployment.Binding
            Namespace](https://docs.microsoft.com/en-us/dotnet/api/microsoft.biztalk.deployment.binding 'https://docs.microsoft.com/en-us/dotnet/api/microsoft.biztalk.deployment.binding')

| Properties | |
| :--- | :--- |
| [BindingInfo](BindingInfoBuilder.BindingInfo.md 'Be.Stateless.BizTalk.Dsl.Binding.Visitor.BindingInfoBuilder.BindingInfo') | |

| Methods | |
| :--- | :--- |
| [CreateBindingInfo&lt;TNamingConvention&gt;(IApplicationBinding&lt;TNamingConvention&gt;)](BindingInfoBuilder.CreateBindingInfo_TNamingConvention_(IApplicationBinding_TNamingConvention_).md 'Be.Stateless.BizTalk.Dsl.Binding.Visitor.BindingInfoBuilder.CreateBindingInfo<TNamingConvention>(Be.Stateless.BizTalk.Dsl.Binding.IApplicationBinding<TNamingConvention>)') | |
| [CreateOrFindModuleRef(IOrchestrationBinding)](BindingInfoBuilder.CreateOrFindModuleRef(IOrchestrationBinding).md 'Be.Stateless.BizTalk.Dsl.Binding.Visitor.BindingInfoBuilder.CreateOrFindModuleRef(Be.Stateless.BizTalk.Dsl.Binding.IOrchestrationBinding)') | |
| [CreateReceiveLocation&lt;TNamingConvention&gt;(IReceiveLocation&lt;TNamingConvention&gt;)](BindingInfoBuilder.CreateReceiveLocation_TNamingConvention_(IReceiveLocation_TNamingConvention_).md 'Be.Stateless.BizTalk.Dsl.Binding.Visitor.BindingInfoBuilder.CreateReceiveLocation<TNamingConvention>(Be.Stateless.BizTalk.Dsl.Binding.IReceiveLocation<TNamingConvention>)') | |
| [CreateReceivePipelineRef(ReceivePipeline)](BindingInfoBuilder.CreateReceivePipelineRef(ReceivePipeline).md 'Be.Stateless.BizTalk.Dsl.Binding.Visitor.BindingInfoBuilder.CreateReceivePipelineRef(Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline)') | |
| [CreateReceivePort&lt;TNamingConvention&gt;(IReceivePort&lt;TNamingConvention&gt;)](BindingInfoBuilder.CreateReceivePort_TNamingConvention_(IReceivePort_TNamingConvention_).md 'Be.Stateless.BizTalk.Dsl.Binding.Visitor.BindingInfoBuilder.CreateReceivePort<TNamingConvention>(Be.Stateless.BizTalk.Dsl.Binding.IReceivePort<TNamingConvention>)') | |
| [CreateSendPipelineRef(SendPipeline)](BindingInfoBuilder.CreateSendPipelineRef(SendPipeline).md 'Be.Stateless.BizTalk.Dsl.Binding.Visitor.BindingInfoBuilder.CreateSendPipelineRef(Be.Stateless.BizTalk.Dsl.Pipeline.SendPipeline)') | |
| [CreateSendPort&lt;TNamingConvention&gt;(ISendPort&lt;TNamingConvention&gt;)](BindingInfoBuilder.CreateSendPort_TNamingConvention_(ISendPort_TNamingConvention_).md 'Be.Stateless.BizTalk.Dsl.Binding.Visitor.BindingInfoBuilder.CreateSendPort<TNamingConvention>(Be.Stateless.BizTalk.Dsl.Binding.ISendPort<TNamingConvention>)') | |
| [CreateServicePortRef(IOrchestrationPortBinding)](BindingInfoBuilder.CreateServicePortRef(IOrchestrationPortBinding).md 'Be.Stateless.BizTalk.Dsl.Binding.Visitor.BindingInfoBuilder.CreateServicePortRef(Be.Stateless.BizTalk.Dsl.Binding.IOrchestrationPortBinding)') | |
| [CreateServiceRef(IOrchestrationBinding)](BindingInfoBuilder.CreateServiceRef(IOrchestrationBinding).md 'Be.Stateless.BizTalk.Dsl.Binding.Visitor.BindingInfoBuilder.CreateServiceRef(Be.Stateless.BizTalk.Dsl.Binding.IOrchestrationBinding)') | |
| [CreateTransportInfo&lt;TNamingConvention&gt;(SendPortTransport&lt;TNamingConvention&gt;)](BindingInfoBuilder.CreateTransportInfo_TNamingConvention_(SendPortTransport_TNamingConvention_).md 'Be.Stateless.BizTalk.Dsl.Binding.Visitor.BindingInfoBuilder.CreateTransportInfo<TNamingConvention>(Be.Stateless.BizTalk.Dsl.Binding.SendPortTransport<TNamingConvention>)') | |

| Explicit Interface Implementations | |
| :--- | :--- |
| [Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor.VisitApplicationBinding&lt;TNamingConvention&gt;(IApplicationBinding&lt;TNamingConvention&gt;)](BindingInfoBuilder.Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor.VisitApplicationBinding_TNamingConvention_(IApplicationBinding_TNamingConvention_).md 'Be.Stateless.BizTalk.Dsl.Binding.Visitor.BindingInfoBuilder.Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor.VisitApplicationBinding<TNamingConvention>(Be.Stateless.BizTalk.Dsl.Binding.IApplicationBinding<TNamingConvention>)') | |
| [Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor.VisitOrchestration(IOrchestrationBinding)](BindingInfoBuilder.Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor.VisitOrchestration(IOrchestrationBinding).md 'Be.Stateless.BizTalk.Dsl.Binding.Visitor.BindingInfoBuilder.Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor.VisitOrchestration(Be.Stateless.BizTalk.Dsl.Binding.IOrchestrationBinding)') | |
| [Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor.VisitReceiveLocation&lt;TNamingConvention&gt;(IReceiveLocation&lt;TNamingConvention&gt;)](BindingInfoBuilder.Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor.VisitReceiveLocation_TNamingConvention_(IReceiveLocation_TNamingConvention_).md 'Be.Stateless.BizTalk.Dsl.Binding.Visitor.BindingInfoBuilder.Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor.VisitReceiveLocation<TNamingConvention>(Be.Stateless.BizTalk.Dsl.Binding.IReceiveLocation<TNamingConvention>)') | |
| [Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor.VisitReceivePort&lt;TNamingConvention&gt;(IReceivePort&lt;TNamingConvention&gt;)](BindingInfoBuilder.Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor.VisitReceivePort_TNamingConvention_(IReceivePort_TNamingConvention_).md 'Be.Stateless.BizTalk.Dsl.Binding.Visitor.BindingInfoBuilder.Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor.VisitReceivePort<TNamingConvention>(Be.Stateless.BizTalk.Dsl.Binding.IReceivePort<TNamingConvention>)') | |
| [Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor.VisitReferencedApplicationBinding(IVisitable&lt;IApplicationBindingVisitor&gt;)](BindingInfoBuilder.Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor.VisitReferencedApplicationBinding(IVisitable_IApplicationBindingVisitor_).md 'Be.Stateless.BizTalk.Dsl.Binding.Visitor.BindingInfoBuilder.Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor.VisitReferencedApplicationBinding(Be.Stateless.BizTalk.Dsl.IVisitable<Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor>)') | |
| [Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor.VisitSendPort&lt;TNamingConvention&gt;(ISendPort&lt;TNamingConvention&gt;)](BindingInfoBuilder.Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor.VisitSendPort_TNamingConvention_(ISendPort_TNamingConvention_).md 'Be.Stateless.BizTalk.Dsl.Binding.Visitor.BindingInfoBuilder.Be.Stateless.BizTalk.Dsl.Binding.IApplicationBindingVisitor.VisitSendPort<TNamingConvention>(Be.Stateless.BizTalk.Dsl.Binding.ISendPort<TNamingConvention>)') | |
