#### [Be.Stateless.BizTalk.Pipeline.Components](README.md 'README')
### [Be.Stateless.BizTalk.Component.Interop](Be.Stateless.BizTalk.Component.Interop.md 'Be.Stateless.BizTalk.Component.Interop').[PropertyBag](PropertyBag.md 'Be.Stateless.BizTalk.Component.Interop.PropertyBag')

## PropertyBag.WriteProperty<T>(this IPropertyBag, string, T) Method

Write an [System.Enum](https://docs.microsoft.com/en-us/dotnet/api/System.Enum 'System.Enum') property value to the [Microsoft.BizTalk.Component.Interop.IPropertyBag](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPropertyBag 'Microsoft.BizTalk.Component.Interop.IPropertyBag') bag.

```csharp
public static void WriteProperty<T>(this Microsoft.BizTalk.Component.Interop.IPropertyBag propertyBag, string name, T value)
    where T : struct, System.ValueType, System.ValueType;
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Component.Interop.PropertyBag.WriteProperty_T_(thisMicrosoft.BizTalk.Component.Interop.IPropertyBag,string,T).T'></a>

`T`

The [System.Enum](https://docs.microsoft.com/en-us/dotnet/api/System.Enum 'System.Enum') type of the property.
#### Parameters

<a name='Be.Stateless.BizTalk.Component.Interop.PropertyBag.WriteProperty_T_(thisMicrosoft.BizTalk.Component.Interop.IPropertyBag,string,T).propertyBag'></a>

`propertyBag` [Microsoft.BizTalk.Component.Interop.IPropertyBag](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPropertyBag 'Microsoft.BizTalk.Component.Interop.IPropertyBag')

The [Microsoft.BizTalk.Component.Interop.IPropertyBag](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPropertyBag 'Microsoft.BizTalk.Component.Interop.IPropertyBag') bag instance.

<a name='Be.Stateless.BizTalk.Component.Interop.PropertyBag.WriteProperty_T_(thisMicrosoft.BizTalk.Component.Interop.IPropertyBag,string,T).name'></a>

`name` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The name of the property to write to the [Microsoft.BizTalk.Component.Interop.IPropertyBag](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPropertyBag 'Microsoft.BizTalk.Component.Interop.IPropertyBag') bag.

<a name='Be.Stateless.BizTalk.Component.Interop.PropertyBag.WriteProperty_T_(thisMicrosoft.BizTalk.Component.Interop.IPropertyBag,string,T).value'></a>

`value` [T](PropertyBag.WriteProperty_T_(thisIPropertyBag,string,T).md#Be.Stateless.BizTalk.Component.Interop.PropertyBag.WriteProperty_T_(thisMicrosoft.BizTalk.Component.Interop.IPropertyBag,string,T).T 'Be.Stateless.BizTalk.Component.Interop.PropertyBag.WriteProperty<T>(this Microsoft.BizTalk.Component.Interop.IPropertyBag, string, T).T')

The [System.Enum](https://docs.microsoft.com/en-us/dotnet/api/System.Enum 'System.Enum') property value to write to the [Microsoft.BizTalk.Component.Interop.IPropertyBag](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPropertyBag 'Microsoft.BizTalk.Component.Interop.IPropertyBag') bag.