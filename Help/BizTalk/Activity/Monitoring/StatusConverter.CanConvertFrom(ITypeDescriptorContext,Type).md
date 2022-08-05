#### [Be.Stateless.BizTalk.Activity.Monitoring](README.md 'README')
### [Be.Stateless.BizTalk.Activity.Monitoring.Model](Be.Stateless.BizTalk.Activity.Monitoring.Model.md 'Be.Stateless.BizTalk.Activity.Monitoring.Model').[StatusConverter](StatusConverter.md 'Be.Stateless.BizTalk.Activity.Monitoring.Model.StatusConverter')

## StatusConverter.CanConvertFrom(ITypeDescriptorContext, Type) Method

Returns whether this converter can convert an object of the given type to the type of this converter, using the
specified context.

```csharp
public override bool CanConvertFrom(System.ComponentModel.ITypeDescriptorContext context, System.Type sourceType);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Activity.Monitoring.Model.StatusConverter.CanConvertFrom(System.ComponentModel.ITypeDescriptorContext,System.Type).context'></a>

`context` [System.ComponentModel.ITypeDescriptorContext](https://docs.microsoft.com/en-us/dotnet/api/System.ComponentModel.ITypeDescriptorContext 'System.ComponentModel.ITypeDescriptorContext')

An [System.ComponentModel.ITypeDescriptorContext](https://docs.microsoft.com/en-us/dotnet/api/System.ComponentModel.ITypeDescriptorContext 'System.ComponentModel.ITypeDescriptorContext') that provides a format context.

<a name='Be.Stateless.BizTalk.Activity.Monitoring.Model.StatusConverter.CanConvertFrom(System.ComponentModel.ITypeDescriptorContext,System.Type).sourceType'></a>

`sourceType` [System.Type](https://docs.microsoft.com/en-us/dotnet/api/System.Type 'System.Type')

A [System.Type](https://docs.microsoft.com/en-us/dotnet/api/System.Type 'System.Type') that represents the type you want to convert from.

#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')  
true if this converter can perform the conversion; otherwise, false.