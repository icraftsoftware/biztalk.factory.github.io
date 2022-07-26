#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Text](Be.Stateless.Text.md 'Be.Stateless.Text')

## EncodingConverter Class

Converts an [System.Text.Encoding](https://docs.microsoft.com/en-us/dotnet/api/System.Text.Encoding 'System.Text.Encoding') back-and-forth to a [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String').

```csharp
public class EncodingConverter : System.ComponentModel.ExpandableObjectConverter
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [System.ComponentModel.TypeConverter](https://docs.microsoft.com/en-us/dotnet/api/System.ComponentModel.TypeConverter 'System.ComponentModel.TypeConverter') &#129106; [System.ComponentModel.ExpandableObjectConverter](https://docs.microsoft.com/en-us/dotnet/api/System.ComponentModel.ExpandableObjectConverter 'System.ComponentModel.ExpandableObjectConverter') &#129106; EncodingConverter

| Methods | |
| :--- | :--- |
| [CanConvertFrom(ITypeDescriptorContext, Type)](EncodingConverter.CanConvertFrom(ITypeDescriptorContext,Type).md 'Be.Stateless.Text.EncodingConverter.CanConvertFrom(System.ComponentModel.ITypeDescriptorContext, System.Type)') | Returns whether this converter can convert an object of the given type to the type of this converter, using the specified context. |
| [CanConvertTo(ITypeDescriptorContext, Type)](EncodingConverter.CanConvertTo(ITypeDescriptorContext,Type).md 'Be.Stateless.Text.EncodingConverter.CanConvertTo(System.ComponentModel.ITypeDescriptorContext, System.Type)') | Returns whether this converter can convert the object to the specified type, using the specified context. |
| [ConvertFrom(ITypeDescriptorContext, CultureInfo, object)](EncodingConverter.ConvertFrom(ITypeDescriptorContext,CultureInfo,object).md 'Be.Stateless.Text.EncodingConverter.ConvertFrom(System.ComponentModel.ITypeDescriptorContext, System.Globalization.CultureInfo, object)') | Converts the given object to the type of this converter, using the specified context and culture information. |
| [ConvertTo(ITypeDescriptorContext, CultureInfo, object, Type)](EncodingConverter.ConvertTo(ITypeDescriptorContext,CultureInfo,object,Type).md 'Be.Stateless.Text.EncodingConverter.ConvertTo(System.ComponentModel.ITypeDescriptorContext, System.Globalization.CultureInfo, object, System.Type)') | Converts the given value object to the specified type, using the specified context and culture information. |
| [Deserialize(string)](EncodingConverter.Deserialize(string).md 'Be.Stateless.Text.EncodingConverter.Deserialize(string)') | Converts the given [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') to a [System.Text.Encoding](https://docs.microsoft.com/en-us/dotnet/api/System.Text.Encoding 'System.Text.Encoding') instance. |
| [Serialize(Encoding)](EncodingConverter.Serialize(Encoding).md 'Be.Stateless.Text.EncodingConverter.Serialize(System.Text.Encoding)') | Converts a [System.Text.Encoding](https://docs.microsoft.com/en-us/dotnet/api/System.Text.Encoding 'System.Text.Encoding') instance to its [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') representation. |
