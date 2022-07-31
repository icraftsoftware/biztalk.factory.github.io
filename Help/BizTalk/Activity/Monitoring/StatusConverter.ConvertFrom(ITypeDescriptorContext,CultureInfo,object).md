#### [Be.Stateless.BizTalk.Activity.Monitoring](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Monitoring.Model](Be.Stateless.BizTalk.Activity.Monitoring.Model.md 'Be.Stateless.BizTalk.Activity.Monitoring.Model').[StatusConverter](StatusConverter.md 'Be.Stateless.BizTalk.Activity.Monitoring.Model.StatusConverter')

## StatusConverter.ConvertFrom(ITypeDescriptorContext, CultureInfo, object) Method

Converts the given object to the type of this converter, using the specified context and culture information.

```csharp
public override object ConvertFrom(System.ComponentModel.ITypeDescriptorContext context, System.Globalization.CultureInfo culture, object value);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Activity.Monitoring.Model.StatusConverter.ConvertFrom(System.ComponentModel.ITypeDescriptorContext,System.Globalization.CultureInfo,object).context'></a>

`context` [System.ComponentModel.ITypeDescriptorContext](https://docs.microsoft.com/en-us/dotnet/api/System.ComponentModel.ITypeDescriptorContext 'System.ComponentModel.ITypeDescriptorContext')

An [System.ComponentModel.ITypeDescriptorContext](https://docs.microsoft.com/en-us/dotnet/api/System.ComponentModel.ITypeDescriptorContext 'System.ComponentModel.ITypeDescriptorContext') that provides a format context.

<a name='Be.Stateless.BizTalk.Activity.Monitoring.Model.StatusConverter.ConvertFrom(System.ComponentModel.ITypeDescriptorContext,System.Globalization.CultureInfo,object).culture'></a>

`culture` [System.Globalization.CultureInfo](https://docs.microsoft.com/en-us/dotnet/api/System.Globalization.CultureInfo 'System.Globalization.CultureInfo')

The [System.Globalization.CultureInfo](https://docs.microsoft.com/en-us/dotnet/api/System.Globalization.CultureInfo 'System.Globalization.CultureInfo') to use as the current culture.

<a name='Be.Stateless.BizTalk.Activity.Monitoring.Model.StatusConverter.ConvertFrom(System.ComponentModel.ITypeDescriptorContext,System.Globalization.CultureInfo,object).value'></a>

`value` [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object')

The [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') to convert.

#### Returns
[System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object')  
An [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') that represents the converted value.

#### Exceptions

[System.NotSupportedException](https://docs.microsoft.com/en-us/dotnet/api/System.NotSupportedException 'System.NotSupportedException')  
The conversion cannot be performed.