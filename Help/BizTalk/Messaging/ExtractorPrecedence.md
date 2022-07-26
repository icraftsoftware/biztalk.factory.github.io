#### [Be.Stateless.BizTalk.Messaging](README.md 'README')
### [Be.Stateless.BizTalk.Schema.Annotation](Be.Stateless.BizTalk.Schema.Annotation.md 'Be.Stateless.BizTalk.Schema.Annotation')

## ExtractorPrecedence Enum

Determines how to merge two [PropertyExtractorCollection](PropertyExtractorCollection.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection') instances.

```csharp
public enum ExtractorPrecedence
```
### Fields

<a name='Be.Stateless.BizTalk.Schema.Annotation.ExtractorPrecedence.Pipeline'></a>

`Pipeline` 2

[PropertyExtractorCollection](PropertyExtractorCollection.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection') declared by pipeline configuration have precedence over the one declared by XML schema annotations.

<a name='Be.Stateless.BizTalk.Schema.Annotation.ExtractorPrecedence.PipelineOnly'></a>

`PipelineOnly` 3

Only the [PropertyExtractorCollection](PropertyExtractorCollection.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection') declared by pipeline configuration is taken into account and the one declared by XML schema
annotations is ignored.

<a name='Be.Stateless.BizTalk.Schema.Annotation.ExtractorPrecedence.Schema'></a>

`Schema` 0

[PropertyExtractorCollection](PropertyExtractorCollection.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection') declared by XML schema annotations have precedence over the one declared by pipeline configuration.

<a name='Be.Stateless.BizTalk.Schema.Annotation.ExtractorPrecedence.SchemaOnly'></a>

`SchemaOnly` 1

Only [PropertyExtractorCollection](PropertyExtractorCollection.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection') declared by XML schema annotations is taken into account and the one declared by pipeline
configuration is ignored.

### Remarks

[PropertyExtractorCollection](PropertyExtractorCollection.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection') can only be declared at 2 places, via XML schema annotations or via pipeline configuration. By default,
            precedence will be given to the [PropertyExtractorCollection](PropertyExtractorCollection.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection') being declared by XML schema annotations.

Should conflicting [ExtractorPrecedence](ExtractorPrecedence.md 'Be.Stateless.BizTalk.Schema.Annotation.ExtractorPrecedence')s be declared by XML schema annotations and pipeline configuration, the [ExtractorPrecedence](ExtractorPrecedence.md 'Be.Stateless.BizTalk.Schema.Annotation.ExtractorPrecedence') declared by the pipeline configuration will always have the precedence over the one declared by XML schema annotations.
It would consequently make sense to <b>only declare the <see cref="T:Be.Stateless.BizTalk.Schema.Annotation.ExtractorPrecedence"/> at the pipeline level.</b> Declaring an [ExtractorPrecedence](ExtractorPrecedence.md 'Be.Stateless.BizTalk.Schema.Annotation.ExtractorPrecedence') via XML schema annotations is possible but pointless.

### See Also
- [Union(PropertyExtractorCollection)](PropertyExtractorCollection.Union(PropertyExtractorCollection).md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection.Union(Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection)')
- [Be.Stateless.BizTalk.Component.ContextPropertyExtractorComponent](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Component.ContextPropertyExtractorComponent 'Be.Stateless.BizTalk.Component.ContextPropertyExtractorComponent')