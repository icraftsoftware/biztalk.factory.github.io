#### [Be.Stateless.BizTalk.Pipeline.MicroComponents](README.md 'README')
### [Be.Stateless.BizTalk.MicroComponent](Be.Stateless.BizTalk.MicroComponent.md 'Be.Stateless.BizTalk.MicroComponent')

## MicroPipeline Class

Runs a sequence of micro components, i.e. components implementing [IMicroComponent](IMicroComponent.md 'Be.Stateless.BizTalk.MicroComponent.IMicroComponent'), similarly to what a
regular Microsoft BizTalk Server pipeline would do if the micro components were regular pipeline components.

```csharp
public class MicroPipeline
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; MicroPipeline

| Properties | |
| :--- | :--- |
| [Components](MicroPipeline.Components.md 'Be.Stateless.BizTalk.MicroComponent.MicroPipeline.Components') | List of micro components that will be run in sequence by the micro pipeline. |

| Methods | |
| :--- | :--- |
| [Execute(IPipelineContext, IBaseMessage)](MicroPipeline.Execute(IPipelineContext,IBaseMessage).md 'Be.Stateless.BizTalk.MicroComponent.MicroPipeline.Execute(Microsoft.BizTalk.Component.Interop.IPipelineContext, Microsoft.BizTalk.Message.Interop.IBaseMessage)') | |
| [LoadConfiguration(string)](MicroPipeline.LoadConfiguration(string).md 'Be.Stateless.BizTalk.MicroComponent.MicroPipeline.LoadConfiguration(string)') | |
| [SaveConfiguration()](MicroPipeline.SaveConfiguration().md 'Be.Stateless.BizTalk.MicroComponent.MicroPipeline.SaveConfiguration()') | |
