#### [Be.Stateless.BizTalk.Messaging](README.md 'README')
### [Be.Stateless.BizTalk.Schema.Annotation](Be.Stateless.BizTalk.Schema.Annotation.md 'Be.Stateless.BizTalk.Schema.Annotation')

## PropertyExtractorCollectionConverter Class

Converts a [PropertyExtractorCollection](PropertyExtractorCollection.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection') back and forth to a [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String').

```csharp
public class PropertyExtractorCollectionConverter : System.ComponentModel.ExpandableObjectConverter
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [System.ComponentModel.TypeConverter](https://docs.microsoft.com/en-us/dotnet/api/System.ComponentModel.TypeConverter 'System.ComponentModel.TypeConverter') &#129106; [System.ComponentModel.ExpandableObjectConverter](https://docs.microsoft.com/en-us/dotnet/api/System.ComponentModel.ExpandableObjectConverter 'System.ComponentModel.ExpandableObjectConverter') &#129106; PropertyExtractorCollectionConverter

### Remarks
Notice that [PropertyExtractorCollectionConverter](PropertyExtractorCollectionConverter.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollectionConverter') delegates the XML serialization and deserialization to [PropertyExtractorCollection](PropertyExtractorCollection.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection').

### See Also
- [PropertyExtractorCollection](PropertyExtractorCollection.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection')

| Methods | |
| :--- | :--- |
| [CanConvertFrom(ITypeDescriptorContext, Type)](PropertyExtractorCollectionConverter.CanConvertFrom(ITypeDescriptorContext,Type).md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollectionConverter.CanConvertFrom(System.ComponentModel.ITypeDescriptorContext, System.Type)') | Returns whether this converter can convert an object of the given type to the type of this converter, using the specified context. |
| [CanConvertTo(ITypeDescriptorContext, Type)](PropertyExtractorCollectionConverter.CanConvertTo(ITypeDescriptorContext,Type).md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollectionConverter.CanConvertTo(System.ComponentModel.ITypeDescriptorContext, System.Type)') | Returns whether this converter can convert the object to the specified type, using the specified context. |
| [ConvertFrom(ITypeDescriptorContext, CultureInfo, object)](PropertyExtractorCollectionConverter.ConvertFrom(ITypeDescriptorContext,CultureInfo,object).md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollectionConverter.ConvertFrom(System.ComponentModel.ITypeDescriptorContext, System.Globalization.CultureInfo, object)') | Converts the given object to the type of this converter, using the specified context and culture information. |
| [ConvertTo(ITypeDescriptorContext, CultureInfo, object, Type)](PropertyExtractorCollectionConverter.ConvertTo(ITypeDescriptorContext,CultureInfo,object,Type).md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollectionConverter.ConvertTo(System.ComponentModel.ITypeDescriptorContext, System.Globalization.CultureInfo, object, System.Type)') | Converts the given value object to the specified type, using the specified context and culture information. |
| [Deserialize(string)](PropertyExtractorCollectionConverter.Deserialize(string).md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollectionConverter.Deserialize(string)') | Deserializes a [PropertyExtractorCollection](PropertyExtractorCollection.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection') from its XML serialization [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String'). |
| [Serialize(PropertyExtractorCollection)](PropertyExtractorCollectionConverter.Serialize(PropertyExtractorCollection).md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollectionConverter.Serialize(Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection)') | Serializes a [PropertyExtractorCollection](PropertyExtractorCollection.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollection') to its XML [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') representation. |
