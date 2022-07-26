#### [Be.Stateless.BizTalk.Pipeline.MicroComponents](README.md 'README')
### [Be.Stateless.BizTalk.MicroComponent](Be.Stateless.BizTalk.MicroComponent.md 'Be.Stateless.BizTalk.MicroComponent').[MicroComponentEnumerableConverter](MicroComponentEnumerableConverter.md 'Be.Stateless.BizTalk.MicroComponent.MicroComponentEnumerableConverter')

## MicroComponentEnumerableConverter.CanConvertTo(ITypeDescriptorContext, Type) Method

Returns whether this converter can convert the object to the specified type, using the specified context.

```csharp
public override bool CanConvertTo(System.ComponentModel.ITypeDescriptorContext context, System.Type destinationType);
```
#### Parameters

<a name='Be.Stateless.BizTalk.MicroComponent.MicroComponentEnumerableConverter.CanConvertTo(System.ComponentModel.ITypeDescriptorContext,System.Type).context'></a>

`context` [System.ComponentModel.ITypeDescriptorContext](https://docs.microsoft.com/en-us/dotnet/api/System.ComponentModel.ITypeDescriptorContext 'System.ComponentModel.ITypeDescriptorContext')

An [System.ComponentModel.ITypeDescriptorContext](https://docs.microsoft.com/en-us/dotnet/api/System.ComponentModel.ITypeDescriptorContext 'System.ComponentModel.ITypeDescriptorContext') that provides a format context.

<a name='Be.Stateless.BizTalk.MicroComponent.MicroComponentEnumerableConverter.CanConvertTo(System.ComponentModel.ITypeDescriptorContext,System.Type).destinationType'></a>

`destinationType` [System.Type](https://docs.microsoft.com/en-us/dotnet/api/System.Type 'System.Type')

A [System.Type](https://docs.microsoft.com/en-us/dotnet/api/System.Type 'System.Type') that represents the type you want to convert to.

#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')  
true if this converter can perform the conversion; otherwise, false.