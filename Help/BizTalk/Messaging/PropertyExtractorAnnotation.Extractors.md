#### [Be.Stateless.BizTalk.Messaging](README.md 'README')
### [Be.Stateless.BizTalk.Schema](Be.Stateless.BizTalk.Schema.md 'Be.Stateless.BizTalk.Schema').[PropertyExtractorAnnotation](PropertyExtractorAnnotation.md 'Be.Stateless.BizTalk.Schema.PropertyExtractorAnnotation')

## PropertyExtractorAnnotation.Extractors Property

Collection of [PropertyExtractor](PropertyExtractor.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractor')-derived extractors used to read, write or promote values to and from
the context properties of an [Microsoft.BizTalk.Message.Interop.IBaseMessagePart](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessagePart 'Microsoft.BizTalk.Message.Interop.IBaseMessagePart')'s payload while being processed through the pipelines.

```csharp
public Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection Extractors { get; set; }
```

#### Property Value
[PropertyExtractorCollection](PropertyExtractorCollection.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection')