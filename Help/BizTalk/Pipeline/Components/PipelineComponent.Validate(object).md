#### [Be.Stateless.BizTalk.Pipeline.Components](README.md 'README')
### [Be.Stateless.BizTalk.Component](Be.Stateless.BizTalk.Component.md 'Be.Stateless.BizTalk.Component').[PipelineComponent](PipelineComponent.md 'Be.Stateless.BizTalk.Component.PipelineComponent')

## PipelineComponent.Validate(object) Method

The Validate method is called by the BizTalk Editor during the build of a BizTalk project.

```csharp
public virtual System.Collections.IEnumerator Validate(object projectSystem);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Component.PipelineComponent.Validate(object).projectSystem'></a>

`projectSystem` [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object')

An object containing the configuration properties.

Implements [Validate(object)](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IComponentUI.Validate#Microsoft_BizTalk_Component_Interop_IComponentUI_Validate_System_Object_ 'Microsoft.BizTalk.Component.Interop.IComponentUI.Validate(System.Object)')

#### Returns
[System.Collections.IEnumerator](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.IEnumerator 'System.Collections.IEnumerator')  
The IEnumerator enables the caller to enumerate through a collection of strings containing error messages. These
error messages appear as compiler error messages. To report successful property validation, the method should return
an empty enumerator.