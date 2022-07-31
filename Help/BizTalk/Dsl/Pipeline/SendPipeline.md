#### [Be.Stateless.BizTalk.Dsl.Pipeline](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Pipeline](Be.Stateless.BizTalk.Dsl.Pipeline.md 'Be.Stateless.BizTalk.Dsl.Pipeline')

## SendPipeline Class

```csharp
public abstract class SendPipeline : Be.Stateless.BizTalk.Dsl.Pipeline.Pipeline<Be.Stateless.BizTalk.Dsl.Pipeline.ISendPipelineStageList>
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [Be.Stateless.BizTalk.Dsl.Pipeline.Pipeline&lt;](Pipeline_T_.md 'Be.Stateless.BizTalk.Dsl.Pipeline.Pipeline<T>')[ISendPipelineStageList](ISendPipelineStageList.md 'Be.Stateless.BizTalk.Dsl.Pipeline.ISendPipelineStageList')[&gt;](Pipeline_T_.md 'Be.Stateless.BizTalk.Dsl.Pipeline.Pipeline<T>') &#129106; SendPipeline

| Properties | |
| :--- | :--- |
| [Assemblers](SendPipeline.Assemblers.md 'Be.Stateless.BizTalk.Dsl.Pipeline.SendPipeline.Assemblers') | Components of the 2nd stage of a [SendPipeline](SendPipeline.md 'Be.Stateless.BizTalk.Dsl.Pipeline.SendPipeline'), i.e. the [Assemble](ISendPipelineStageList.Assemble.md 'Be.Stateless.BizTalk.Dsl.Pipeline.ISendPipelineStageList.Assemble') stage. |
| [Encoders](SendPipeline.Encoders.md 'Be.Stateless.BizTalk.Dsl.Pipeline.SendPipeline.Encoders') | Components of the 3rd stage of a [SendPipeline](SendPipeline.md 'Be.Stateless.BizTalk.Dsl.Pipeline.SendPipeline'), i.e. the [Encode](ISendPipelineStageList.Encode.md 'Be.Stateless.BizTalk.Dsl.Pipeline.ISendPipelineStageList.Encode') stage. |
| [PreAssemblers](SendPipeline.PreAssemblers.md 'Be.Stateless.BizTalk.Dsl.Pipeline.SendPipeline.PreAssemblers') | Components of the 1st stage of a [SendPipeline](SendPipeline.md 'Be.Stateless.BizTalk.Dsl.Pipeline.SendPipeline'), i.e. the [PreAssemble](ISendPipelineStageList.PreAssemble.md 'Be.Stateless.BizTalk.Dsl.Pipeline.ISendPipelineStageList.PreAssemble') stage. |

| Methods | |
| :--- | :--- |
| [Assembler&lt;T&gt;()](SendPipeline.Assembler_T_().md 'Be.Stateless.BizTalk.Dsl.Pipeline.SendPipeline.Assembler<T>()') | |
| [Assembler&lt;T&gt;(Action&lt;T&gt;)](SendPipeline.Assembler_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.SendPipeline.Assembler<T>(System.Action<T>)') | |
| [AssemblerAt&lt;T&gt;(int)](SendPipeline.AssemblerAt_T_(int).md 'Be.Stateless.BizTalk.Dsl.Pipeline.SendPipeline.AssemblerAt<T>(int)') | |
| [Encoder&lt;T&gt;()](SendPipeline.Encoder_T_().md 'Be.Stateless.BizTalk.Dsl.Pipeline.SendPipeline.Encoder<T>()') | |
| [Encoder&lt;T&gt;(Action&lt;T&gt;)](SendPipeline.Encoder_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.SendPipeline.Encoder<T>(System.Action<T>)') | |
| [EncoderAt&lt;T&gt;(int)](SendPipeline.EncoderAt_T_(int).md 'Be.Stateless.BizTalk.Dsl.Pipeline.SendPipeline.EncoderAt<T>(int)') | |
| [FifthAssembler&lt;T&gt;(Action&lt;T&gt;)](SendPipeline.FifthAssembler_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.SendPipeline.FifthAssembler<T>(System.Action<T>)') | |
| [FifthEncoder&lt;T&gt;(Action&lt;T&gt;)](SendPipeline.FifthEncoder_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.SendPipeline.FifthEncoder<T>(System.Action<T>)') | |
| [FifthPreAssembler&lt;T&gt;(Action&lt;T&gt;)](SendPipeline.FifthPreAssembler_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.SendPipeline.FifthPreAssembler<T>(System.Action<T>)') | |
| [FirstAssembler&lt;T&gt;(Action&lt;T&gt;)](SendPipeline.FirstAssembler_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.SendPipeline.FirstAssembler<T>(System.Action<T>)') | |
| [FirstEncoder&lt;T&gt;(Action&lt;T&gt;)](SendPipeline.FirstEncoder_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.SendPipeline.FirstEncoder<T>(System.Action<T>)') | |
| [FirstPreAssembler&lt;T&gt;(Action&lt;T&gt;)](SendPipeline.FirstPreAssembler_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.SendPipeline.FirstPreAssembler<T>(System.Action<T>)') | |
| [FourthAssembler&lt;T&gt;(Action&lt;T&gt;)](SendPipeline.FourthAssembler_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.SendPipeline.FourthAssembler<T>(System.Action<T>)') | |
| [FourthEncoder&lt;T&gt;(Action&lt;T&gt;)](SendPipeline.FourthEncoder_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.SendPipeline.FourthEncoder<T>(System.Action<T>)') | |
| [FourthPreAssembler&lt;T&gt;(Action&lt;T&gt;)](SendPipeline.FourthPreAssembler_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.SendPipeline.FourthPreAssembler<T>(System.Action<T>)') | |
| [PreAssembler&lt;T&gt;()](SendPipeline.PreAssembler_T_().md 'Be.Stateless.BizTalk.Dsl.Pipeline.SendPipeline.PreAssembler<T>()') | |
| [PreAssembler&lt;T&gt;(Action&lt;T&gt;)](SendPipeline.PreAssembler_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.SendPipeline.PreAssembler<T>(System.Action<T>)') | |
| [PreAssemblerAt&lt;T&gt;(int)](SendPipeline.PreAssemblerAt_T_(int).md 'Be.Stateless.BizTalk.Dsl.Pipeline.SendPipeline.PreAssemblerAt<T>(int)') | |
| [SecondAssembler&lt;T&gt;(Action&lt;T&gt;)](SendPipeline.SecondAssembler_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.SendPipeline.SecondAssembler<T>(System.Action<T>)') | |
| [SecondEncoder&lt;T&gt;(Action&lt;T&gt;)](SendPipeline.SecondEncoder_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.SendPipeline.SecondEncoder<T>(System.Action<T>)') | |
| [SecondPreAssembler&lt;T&gt;(Action&lt;T&gt;)](SendPipeline.SecondPreAssembler_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.SendPipeline.SecondPreAssembler<T>(System.Action<T>)') | |
| [ThirdAssembler&lt;T&gt;(Action&lt;T&gt;)](SendPipeline.ThirdAssembler_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.SendPipeline.ThirdAssembler<T>(System.Action<T>)') | |
| [ThirdEncoder&lt;T&gt;(Action&lt;T&gt;)](SendPipeline.ThirdEncoder_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.SendPipeline.ThirdEncoder<T>(System.Action<T>)') | |
| [ThirdPreAssembler&lt;T&gt;(Action&lt;T&gt;)](SendPipeline.ThirdPreAssembler_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.SendPipeline.ThirdPreAssembler<T>(System.Action<T>)') | |
