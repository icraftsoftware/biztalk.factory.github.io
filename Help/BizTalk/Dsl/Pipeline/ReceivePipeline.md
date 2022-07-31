#### [Be.Stateless.BizTalk.Dsl.Pipeline](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Pipeline](Be.Stateless.BizTalk.Dsl.Pipeline.md 'Be.Stateless.BizTalk.Dsl.Pipeline')

## ReceivePipeline Class

```csharp
public abstract class ReceivePipeline : Be.Stateless.BizTalk.Dsl.Pipeline.Pipeline<Be.Stateless.BizTalk.Dsl.Pipeline.IReceivePipelineStageList>
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [Be.Stateless.BizTalk.Dsl.Pipeline.Pipeline&lt;](Pipeline_T_.md 'Be.Stateless.BizTalk.Dsl.Pipeline.Pipeline<T>')[IReceivePipelineStageList](IReceivePipelineStageList.md 'Be.Stateless.BizTalk.Dsl.Pipeline.IReceivePipelineStageList')[&gt;](Pipeline_T_.md 'Be.Stateless.BizTalk.Dsl.Pipeline.Pipeline<T>') &#129106; ReceivePipeline

| Properties | |
| :--- | :--- |
| [Decoders](ReceivePipeline.Decoders.md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.Decoders') | Components of the 1st stage of a [ReceivePipeline](ReceivePipeline.md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline'), i.e. the [Decode](IReceivePipelineStageList.Decode.md 'Be.Stateless.BizTalk.Dsl.Pipeline.IReceivePipelineStageList.Decode') stage. |
| [Disassemblers](ReceivePipeline.Disassemblers.md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.Disassemblers') | Components of the 2nd stage of a [ReceivePipeline](ReceivePipeline.md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline'), i.e. the [Disassemble](IReceivePipelineStageList.Disassemble.md 'Be.Stateless.BizTalk.Dsl.Pipeline.IReceivePipelineStageList.Disassemble') stage. |
| [PartyResolvers](ReceivePipeline.PartyResolvers.md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.PartyResolvers') | Components of the 4th stage of a [ReceivePipeline](ReceivePipeline.md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline'), i.e. the [ResolveParty](IReceivePipelineStageList.ResolveParty.md 'Be.Stateless.BizTalk.Dsl.Pipeline.IReceivePipelineStageList.ResolveParty') stage. |
| [Validators](ReceivePipeline.Validators.md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.Validators') | Components of the 3rd stage of a [ReceivePipeline](ReceivePipeline.md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline'), i.e. the [Validate](IReceivePipelineStageList.Validate.md 'Be.Stateless.BizTalk.Dsl.Pipeline.IReceivePipelineStageList.Validate') stage. |

| Methods | |
| :--- | :--- |
| [Decoder&lt;T&gt;()](ReceivePipeline.Decoder_T_().md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.Decoder<T>()') | |
| [Decoder&lt;T&gt;(Action&lt;T&gt;)](ReceivePipeline.Decoder_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.Decoder<T>(System.Action<T>)') | |
| [DecoderAt&lt;T&gt;(int)](ReceivePipeline.DecoderAt_T_(int).md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.DecoderAt<T>(int)') | |
| [Disassembler&lt;T&gt;()](ReceivePipeline.Disassembler_T_().md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.Disassembler<T>()') | |
| [Disassembler&lt;T&gt;(Action&lt;T&gt;)](ReceivePipeline.Disassembler_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.Disassembler<T>(System.Action<T>)') | |
| [DisassemblerAt&lt;T&gt;(int)](ReceivePipeline.DisassemblerAt_T_(int).md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.DisassemblerAt<T>(int)') | |
| [FifthDecoder&lt;T&gt;(Action&lt;T&gt;)](ReceivePipeline.FifthDecoder_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.FifthDecoder<T>(System.Action<T>)') | |
| [FifthDisassembler&lt;T&gt;(Action&lt;T&gt;)](ReceivePipeline.FifthDisassembler_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.FifthDisassembler<T>(System.Action<T>)') | |
| [FifthPartyResolver&lt;T&gt;(Action&lt;T&gt;)](ReceivePipeline.FifthPartyResolver_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.FifthPartyResolver<T>(System.Action<T>)') | |
| [FifthValidator&lt;T&gt;(Action&lt;T&gt;)](ReceivePipeline.FifthValidator_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.FifthValidator<T>(System.Action<T>)') | |
| [FirstDecoder&lt;T&gt;(Action&lt;T&gt;)](ReceivePipeline.FirstDecoder_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.FirstDecoder<T>(System.Action<T>)') | |
| [FirstDisassembler&lt;T&gt;(Action&lt;T&gt;)](ReceivePipeline.FirstDisassembler_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.FirstDisassembler<T>(System.Action<T>)') | |
| [FirstPartyResolver&lt;T&gt;(Action&lt;T&gt;)](ReceivePipeline.FirstPartyResolver_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.FirstPartyResolver<T>(System.Action<T>)') | |
| [FirstValidator&lt;T&gt;(Action&lt;T&gt;)](ReceivePipeline.FirstValidator_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.FirstValidator<T>(System.Action<T>)') | |
| [FourthDecoder&lt;T&gt;(Action&lt;T&gt;)](ReceivePipeline.FourthDecoder_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.FourthDecoder<T>(System.Action<T>)') | |
| [FourthDisassembler&lt;T&gt;(Action&lt;T&gt;)](ReceivePipeline.FourthDisassembler_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.FourthDisassembler<T>(System.Action<T>)') | |
| [FourthPartyResolver&lt;T&gt;(Action&lt;T&gt;)](ReceivePipeline.FourthPartyResolver_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.FourthPartyResolver<T>(System.Action<T>)') | |
| [FourthValidator&lt;T&gt;(Action&lt;T&gt;)](ReceivePipeline.FourthValidator_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.FourthValidator<T>(System.Action<T>)') | |
| [PartyResolver&lt;T&gt;()](ReceivePipeline.PartyResolver_T_().md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.PartyResolver<T>()') | |
| [PartyResolver&lt;T&gt;(Action&lt;T&gt;)](ReceivePipeline.PartyResolver_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.PartyResolver<T>(System.Action<T>)') | |
| [PartyResolverAt&lt;T&gt;(int)](ReceivePipeline.PartyResolverAt_T_(int).md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.PartyResolverAt<T>(int)') | |
| [SecondDecoder&lt;T&gt;(Action&lt;T&gt;)](ReceivePipeline.SecondDecoder_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.SecondDecoder<T>(System.Action<T>)') | |
| [SecondDisassembler&lt;T&gt;(Action&lt;T&gt;)](ReceivePipeline.SecondDisassembler_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.SecondDisassembler<T>(System.Action<T>)') | |
| [SecondPartyResolver&lt;T&gt;(Action&lt;T&gt;)](ReceivePipeline.SecondPartyResolver_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.SecondPartyResolver<T>(System.Action<T>)') | |
| [SecondValidator&lt;T&gt;(Action&lt;T&gt;)](ReceivePipeline.SecondValidator_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.SecondValidator<T>(System.Action<T>)') | |
| [ThirdDecoder&lt;T&gt;(Action&lt;T&gt;)](ReceivePipeline.ThirdDecoder_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.ThirdDecoder<T>(System.Action<T>)') | |
| [ThirdDisassembler&lt;T&gt;(Action&lt;T&gt;)](ReceivePipeline.ThirdDisassembler_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.ThirdDisassembler<T>(System.Action<T>)') | |
| [ThirdPartyResolver&lt;T&gt;(Action&lt;T&gt;)](ReceivePipeline.ThirdPartyResolver_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.ThirdPartyResolver<T>(System.Action<T>)') | |
| [ThirdValidator&lt;T&gt;(Action&lt;T&gt;)](ReceivePipeline.ThirdValidator_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.ThirdValidator<T>(System.Action<T>)') | |
| [Validator&lt;T&gt;()](ReceivePipeline.Validator_T_().md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.Validator<T>()') | |
| [Validator&lt;T&gt;(Action&lt;T&gt;)](ReceivePipeline.Validator_T_(Action_T_).md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.Validator<T>(System.Action<T>)') | |
| [ValidatorAt&lt;T&gt;(int)](ReceivePipeline.ValidatorAt_T_(int).md 'Be.Stateless.BizTalk.Dsl.Pipeline.ReceivePipeline.ValidatorAt<T>(int)') | |
