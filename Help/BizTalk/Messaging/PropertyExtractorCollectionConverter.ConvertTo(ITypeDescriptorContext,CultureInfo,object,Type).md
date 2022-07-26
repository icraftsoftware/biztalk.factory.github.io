#### [Be.Stateless.BizTalk.Messaging](README.md 'README')
### [Be.Stateless.BizTalk.Schema.Annotation](Be.Stateless.BizTalk.Schema.Annotation.md 'Be.Stateless.BizTalk.Schema.Annotation').[PropertyExtractorCollectionConverter](PropertyExtractorCollectionConverter.md 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollectionConverter')

## PropertyExtractorCollectionConverter.ConvertTo(ITypeDescriptorContext, CultureInfo, object, Type) Method

Converts the given value object to the specified type, using the specified context and culture information.

```csharp
public override object ConvertTo(System.ComponentModel.ITypeDescriptorContext context, System.Globalization.CultureInfo culture, object value, System.Type destinationType);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollectionConverter.ConvertTo(System.ComponentModel.ITypeDescriptorContext,System.Globalization.CultureInfo,object,System.Type).context'></a>

`context` [System.ComponentModel.ITypeDescriptorContext](https://docs.microsoft.com/en-us/dotnet/api/System.ComponentModel.ITypeDescriptorContext 'System.ComponentModel.ITypeDescriptorContext')

An [System.ComponentModel.ITypeDescriptorContext](https://docs.microsoft.com/en-us/dotnet/api/System.ComponentModel.ITypeDescriptorContext 'System.ComponentModel.ITypeDescriptorContext') that provides a format context.

<a name='Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollectionConverter.ConvertTo(System.ComponentModel.ITypeDescriptorContext,System.Globalization.CultureInfo,object,System.Type).culture'></a>

`culture` [System.Globalization.CultureInfo](https://docs.microsoft.com/en-us/dotnet/api/System.Globalization.CultureInfo 'System.Globalization.CultureInfo')

A [System.Globalization.CultureInfo](https://docs.microsoft.com/en-us/dotnet/api/System.Globalization.CultureInfo 'System.Globalization.CultureInfo'). If null is passed, the current culture is assumed.

<a name='Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollectionConverter.ConvertTo(System.ComponentModel.ITypeDescriptorContext,System.Globalization.CultureInfo,object,System.Type).value'></a>

`value` [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object')

The [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') to convert.

<a name='Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollectionConverter.ConvertTo(System.ComponentModel.ITypeDescriptorContext,System.Globalization.CultureInfo,object,System.Type).destinationType'></a>

`destinationType` [System.Type](https://docs.microsoft.com/en-us/dotnet/api/System.Type 'System.Type')

The [System.Type](https://docs.microsoft.com/en-us/dotnet/api/System.Type 'System.Type') to convert the [value](PropertyExtractorCollectionConverter.ConvertTo(ITypeDescriptorContext,CultureInfo,object,Type).md#Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollectionConverter.ConvertTo(System.ComponentModel.ITypeDescriptorContext,System.Globalization.CultureInfo,object,System.Type).value 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollectionConverter.ConvertTo(System.ComponentModel.ITypeDescriptorContext, System.Globalization.CultureInfo, object, System.Type).value') parameter to.

#### Returns
[System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object')  
An [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') that represents the converted value.

#### Exceptions

[System.ArgumentNullException](https://docs.microsoft.com/en-us/dotnet/api/System.ArgumentNullException 'System.ArgumentNullException')  
The [destinationType](PropertyExtractorCollectionConverter.ConvertTo(ITypeDescriptorContext,CultureInfo,object,Type).md#Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollectionConverter.ConvertTo(System.ComponentModel.ITypeDescriptorContext,System.Globalization.CultureInfo,object,System.Type).destinationType 'Be.Stateless.BizTalk.Schema.Annotation.PropertyExtractorCollectionConverter.ConvertTo(System.ComponentModel.ITypeDescriptorContext, System.Globalization.CultureInfo, object, System.Type).destinationType') parameter is null.

[System.NotSupportedException](https://docs.microsoft.com/en-us/dotnet/api/System.NotSupportedException 'System.NotSupportedException')  
The conversion cannot be performed.