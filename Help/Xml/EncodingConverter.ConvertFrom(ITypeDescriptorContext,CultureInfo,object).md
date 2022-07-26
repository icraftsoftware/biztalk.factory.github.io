#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Text](Be.Stateless.Text.md 'Be.Stateless.Text').[EncodingConverter](EncodingConverter.md 'Be.Stateless.Text.EncodingConverter')

## EncodingConverter.ConvertFrom(ITypeDescriptorContext, CultureInfo, object) Method

Converts the given object to the type of this converter, using the specified context and culture information.

```csharp
public override object ConvertFrom(System.ComponentModel.ITypeDescriptorContext context, System.Globalization.CultureInfo culture, object value);
```
#### Parameters

<a name='Be.Stateless.Text.EncodingConverter.ConvertFrom(System.ComponentModel.ITypeDescriptorContext,System.Globalization.CultureInfo,object).context'></a>

`context` [System.ComponentModel.ITypeDescriptorContext](https://docs.microsoft.com/en-us/dotnet/api/System.ComponentModel.ITypeDescriptorContext 'System.ComponentModel.ITypeDescriptorContext')

An [System.ComponentModel.ITypeDescriptorContext](https://docs.microsoft.com/en-us/dotnet/api/System.ComponentModel.ITypeDescriptorContext 'System.ComponentModel.ITypeDescriptorContext') that provides a format context.

<a name='Be.Stateless.Text.EncodingConverter.ConvertFrom(System.ComponentModel.ITypeDescriptorContext,System.Globalization.CultureInfo,object).culture'></a>

`culture` [System.Globalization.CultureInfo](https://docs.microsoft.com/en-us/dotnet/api/System.Globalization.CultureInfo 'System.Globalization.CultureInfo')

The [System.Globalization.CultureInfo](https://docs.microsoft.com/en-us/dotnet/api/System.Globalization.CultureInfo 'System.Globalization.CultureInfo') to use as the current culture.

<a name='Be.Stateless.Text.EncodingConverter.ConvertFrom(System.ComponentModel.ITypeDescriptorContext,System.Globalization.CultureInfo,object).value'></a>

`value` [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object')

The [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') to convert.

#### Returns
[System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object')  
An [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') that represents the converted value.

#### Exceptions

[System.NotSupportedException](https://docs.microsoft.com/en-us/dotnet/api/System.NotSupportedException 'System.NotSupportedException')  
The conversion cannot be performed.