#### [Be.Stateless.BizTalk.Pipeline.MicroComponents](README.md 'README')
### [Be.Stateless.BizTalk.Component.Extensions](Be.Stateless.BizTalk.Component.Extensions.md 'Be.Stateless.BizTalk.Component.Extensions').[PipelineContextExtensions](PipelineContextExtensions.md 'Be.Stateless.BizTalk.Component.Extensions.PipelineContextExtensions')

## PipelineContextExtensions.GetSchemaMetadataByType(this IPipelineContext, string, bool) Method

Returns the [Be.Stateless.BizTalk.Schema.ISchemaMetadata](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Schema.ISchemaMetadata 'Be.Stateless.BizTalk.Schema.ISchemaMetadata') associated to the XML schema of messages of a given [Microsoft.BizTalk.Component.Interop.DocumentSpec](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.DocumentSpec 'Microsoft.BizTalk.Component.Interop.DocumentSpec') type.

```csharp
public static Be.Stateless.BizTalk.Schema.ISchemaMetadata GetSchemaMetadataByType(this Microsoft.BizTalk.Component.Interop.IPipelineContext pipelineContext, string docType, bool throwOnError);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Component.Extensions.PipelineContextExtensions.GetSchemaMetadataByType(thisMicrosoft.BizTalk.Component.Interop.IPipelineContext,string,bool).pipelineContext'></a>

`pipelineContext` [Microsoft.BizTalk.Component.Interop.IPipelineContext](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPipelineContext 'Microsoft.BizTalk.Component.Interop.IPipelineContext')

The pipeline context from which the [Microsoft.BizTalk.Component.Interop.DocumentSpec](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.DocumentSpec 'Microsoft.BizTalk.Component.Interop.DocumentSpec') can be queried.

<a name='Be.Stateless.BizTalk.Component.Extensions.PipelineContextExtensions.GetSchemaMetadataByType(thisMicrosoft.BizTalk.Component.Interop.IPipelineContext,string,bool).docType'></a>

`docType` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The [Microsoft.BizTalk.Component.Interop.DocumentSpec](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.DocumentSpec 'Microsoft.BizTalk.Component.Interop.DocumentSpec') type of the messages for which the [Be.Stateless.BizTalk.Schema.ISchemaMetadata](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Schema.ISchemaMetadata 'Be.Stateless.BizTalk.Schema.ISchemaMetadata') are to be returned.

<a name='Be.Stateless.BizTalk.Component.Extensions.PipelineContextExtensions.GetSchemaMetadataByType(thisMicrosoft.BizTalk.Component.Interop.IPipelineContext,string,bool).throwOnError'></a>

`throwOnError` [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

`false` to swallow [System.Runtime.InteropServices.COMException](https://docs.microsoft.com/en-us/dotnet/api/System.Runtime.InteropServices.COMException 'System.Runtime.InteropServices.COMException') and return a [Be.Stateless.BizTalk.Schema.SchemaMetadata.Unknown](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Schema.SchemaMetadata.Unknown 'Be.Stateless.BizTalk.Schema.SchemaMetadata.Unknown') should the
            document specification not to be found; it will however be logged as a warning. `true` to let any exception
            through.

#### Returns
[Be.Stateless.BizTalk.Schema.ISchemaMetadata](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Schema.ISchemaMetadata 'Be.Stateless.BizTalk.Schema.ISchemaMetadata')  
The [Be.Stateless.BizTalk.Schema.ISchemaMetadata](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Schema.ISchemaMetadata 'Be.Stateless.BizTalk.Schema.ISchemaMetadata') associated to the XML Schema.