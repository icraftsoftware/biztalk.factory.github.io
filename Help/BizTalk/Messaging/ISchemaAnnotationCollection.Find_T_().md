#### [Be.Stateless.BizTalk.Messaging](README.md 'README')
### [Be.Stateless.BizTalk.Schema](Be.Stateless.BizTalk.Schema.md 'Be.Stateless.BizTalk.Schema').[ISchemaAnnotationCollection](ISchemaAnnotationCollection.md 'Be.Stateless.BizTalk.Schema.ISchemaAnnotationCollection')

## ISchemaAnnotationCollection.Find<T>() Method

Look up for an embedded schema annotation of type [T](ISchemaAnnotationCollection.Find_T_().md#Be.Stateless.BizTalk.Schema.ISchemaAnnotationCollection.Find_T_().T 'Be.Stateless.BizTalk.Schema.ISchemaAnnotationCollection.Find<T>().T').

```csharp
T Find<T>()
    where T : Be.Stateless.BizTalk.Schema.ISchemaAnnotation<T>, new();
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Schema.ISchemaAnnotationCollection.Find_T_().T'></a>

`T`

The type of the embedded schema annotation to look up.

#### Returns
[T](ISchemaAnnotationCollection.Find_T_().md#Be.Stateless.BizTalk.Schema.ISchemaAnnotationCollection.Find_T_().T 'Be.Stateless.BizTalk.Schema.ISchemaAnnotationCollection.Find<T>().T')  
The [T](ISchemaAnnotationCollection.Find_T_().md#Be.Stateless.BizTalk.Schema.ISchemaAnnotationCollection.Find_T_().T 'Be.Stateless.BizTalk.Schema.ISchemaAnnotationCollection.Find<T>().T') embedded schema annotation instance.