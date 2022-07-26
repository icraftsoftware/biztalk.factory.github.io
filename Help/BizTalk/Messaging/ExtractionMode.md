#### [Be.Stateless.BizTalk.Messaging](README.md 'README')
### [Be.Stateless.BizTalk.Schema.Annotation](Be.Stateless.BizTalk.Schema.Annotation.md 'Be.Stateless.BizTalk.Schema.Annotation')

## ExtractionMode Enum

Denotes how a context property has to be processed by the
`Be.Stateless.BizTalk.Component.ContextPropertyExtractorComponent` pipeline component.

```csharp
public enum ExtractionMode
```
### Fields

<a name='Be.Stateless.BizTalk.Schema.Annotation.ExtractionMode.Clear'></a>

`Clear` 1

The property is deleted from the context.

<a name='Be.Stateless.BizTalk.Schema.Annotation.ExtractionMode.Demote'></a>

`Demote` 2

The property is demoted from the context, that is to say that its value is written back into the outgoing XML stream according to its [XPathExtractor](XPathExtractor.md 'Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor')'s [XPathExpression](XPathExtractor.XPathExpression.md 'Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor.XPathExpression').

### Remarks
This [ExtractionMode](ExtractionMode.md 'Be.Stateless.BizTalk.Schema.Annotation.ExtractionMode') is not compatible with [ConstantExtractor](ConstantExtractor.md 'Be.Stateless.BizTalk.Schema.Annotation.ConstantExtractor') and cannot be used with it.

<a name='Be.Stateless.BizTalk.Schema.Annotation.ExtractionMode.Ignore'></a>

`Ignore` 3

The extractor is ignored and no action is performed.

<a name='Be.Stateless.BizTalk.Schema.Annotation.ExtractionMode.Promote'></a>

`Promote` 4

The value either given via the [ConstantExtractor.Value](ConstantExtractor.Value.md 'Be.Stateless.BizTalk.Schema.Annotation.ConstantExtractor.Value') property or
extracted according to its [XPathExtractor.XPathExpression](XPathExtractor.XPathExpression.md 'Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor.XPathExpression') is
promoted to the context.

<a name='Be.Stateless.BizTalk.Schema.Annotation.ExtractionMode.Write'></a>

`Write` 0

The value either given via the [ConstantExtractor.Value](ConstantExtractor.Value.md 'Be.Stateless.BizTalk.Schema.Annotation.ConstantExtractor.Value') property or
extracted according to its [XPathExtractor.XPathExpression](XPathExtractor.XPathExpression.md 'Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor.XPathExpression') is written
to the context.

### Remarks
Extraction can either means
- [Clear](ExtractionMode.md#Be.Stateless.BizTalk.Schema.Annotation.ExtractionMode.Clear 'Be.Stateless.BizTalk.Schema.Annotation.ExtractionMode.Clear') — the property is deleted from the context.
- [Demote](ExtractionMode.md#Be.Stateless.BizTalk.Schema.Annotation.ExtractionMode.Demote 'Be.Stateless.BizTalk.Schema.Annotation.ExtractionMode.Demote') — the property is demoted from the context, that is to say that its value is
              written back into the outgoing XML stream according to its [XPathExtractor](XPathExtractor.md 'Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor')'s [XPathExpression](XPathExtractor.XPathExpression.md 'Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor.XPathExpression').
- [Ignore](ExtractionMode.md#Be.Stateless.BizTalk.Schema.Annotation.ExtractionMode.Ignore 'Be.Stateless.BizTalk.Schema.Annotation.ExtractionMode.Ignore') — the extractor is ignored and no action is performed.
- [Promote](ExtractionMode.md#Be.Stateless.BizTalk.Schema.Annotation.ExtractionMode.Promote 'Be.Stateless.BizTalk.Schema.Annotation.ExtractionMode.Promote') — the value either given via the [ConstantExtractor.Value](ConstantExtractor.Value.md 'Be.Stateless.BizTalk.Schema.Annotation.ConstantExtractor.Value')
              property or extracted according to its [XPathExtractor.XPathExpression](XPathExtractor.XPathExpression.md 'Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor.XPathExpression')
              is promoted to the context.
- [Write](ExtractionMode.md#Be.Stateless.BizTalk.Schema.Annotation.ExtractionMode.Write 'Be.Stateless.BizTalk.Schema.Annotation.ExtractionMode.Write') — the value either given via the [ConstantExtractor.Value](ConstantExtractor.Value.md 'Be.Stateless.BizTalk.Schema.Annotation.ConstantExtractor.Value')
              property or extracted according to its [XPathExtractor.XPathExpression](XPathExtractor.XPathExpression.md 'Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor.XPathExpression')
              is written to the context.