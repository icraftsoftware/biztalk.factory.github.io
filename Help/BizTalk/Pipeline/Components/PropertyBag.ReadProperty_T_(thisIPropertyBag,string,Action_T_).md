#### [Be.Stateless.BizTalk.Pipeline.Components](README.md 'README')
### [Be.Stateless.BizTalk.Component.Interop](Be.Stateless.BizTalk.Component.Interop.md 'Be.Stateless.BizTalk.Component.Interop').[PropertyBag](PropertyBag.md 'Be.Stateless.BizTalk.Component.Interop.PropertyBag')

## PropertyBag.ReadProperty<T>(this IPropertyBag, string, Action<T>) Method

Read and assign an [System.Enum](https://docs.microsoft.com/en-us/dotnet/api/System.Enum 'System.Enum') property value.

```csharp
public static void ReadProperty<T>(this Microsoft.BizTalk.Component.Interop.IPropertyBag propertyBag, string name, System.Action<T> setter)
    where T : struct, System.ValueType, System.ValueType;
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Component.Interop.PropertyBag.ReadProperty_T_(thisMicrosoft.BizTalk.Component.Interop.IPropertyBag,string,System.Action_T_).T'></a>

`T`

The [System.Enum](https://docs.microsoft.com/en-us/dotnet/api/System.Enum 'System.Enum') type of the property.
#### Parameters

<a name='Be.Stateless.BizTalk.Component.Interop.PropertyBag.ReadProperty_T_(thisMicrosoft.BizTalk.Component.Interop.IPropertyBag,string,System.Action_T_).propertyBag'></a>

`propertyBag` [Microsoft.BizTalk.Component.Interop.IPropertyBag](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPropertyBag 'Microsoft.BizTalk.Component.Interop.IPropertyBag')

The [Microsoft.BizTalk.Component.Interop.IPropertyBag](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPropertyBag 'Microsoft.BizTalk.Component.Interop.IPropertyBag') bag instance.

<a name='Be.Stateless.BizTalk.Component.Interop.PropertyBag.ReadProperty_T_(thisMicrosoft.BizTalk.Component.Interop.IPropertyBag,string,System.Action_T_).name'></a>

`name` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The name of the property to read from the [Microsoft.BizTalk.Component.Interop.IPropertyBag](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPropertyBag 'Microsoft.BizTalk.Component.Interop.IPropertyBag') bag.

<a name='Be.Stateless.BizTalk.Component.Interop.PropertyBag.ReadProperty_T_(thisMicrosoft.BizTalk.Component.Interop.IPropertyBag,string,System.Action_T_).setter'></a>

`setter` [System.Action&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-1 'System.Action`1')[T](PropertyBag.ReadProperty_T_(thisIPropertyBag,string,Action_T_).md#Be.Stateless.BizTalk.Component.Interop.PropertyBag.ReadProperty_T_(thisMicrosoft.BizTalk.Component.Interop.IPropertyBag,string,System.Action_T_).T 'Be.Stateless.BizTalk.Component.Interop.PropertyBag.ReadProperty<T>(this Microsoft.BizTalk.Component.Interop.IPropertyBag, string, System.Action<T>).T')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-1 'System.Action`1')

The property setter to assign the value read from the [Microsoft.BizTalk.Component.Interop.IPropertyBag](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPropertyBag 'Microsoft.BizTalk.Component.Interop.IPropertyBag') bag if not null.