#### [Be.Stateless.BizTalk.Pipeline.Components](README.md 'README')
### [Be.Stateless.BizTalk.Component.Interop](Be.Stateless.BizTalk.Component.Interop.md 'Be.Stateless.BizTalk.Component.Interop').[PropertyBag](PropertyBag.md 'Be.Stateless.BizTalk.Component.Interop.PropertyBag')

## PropertyBag.ReadProperty(this IPropertyBag, string, Action<string>) Method

Read a [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') property value.

```csharp
public static void ReadProperty(this Microsoft.BizTalk.Component.Interop.IPropertyBag propertyBag, string name, System.Action<string> setter);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Component.Interop.PropertyBag.ReadProperty(thisMicrosoft.BizTalk.Component.Interop.IPropertyBag,string,System.Action_string_).propertyBag'></a>

`propertyBag` [Microsoft.BizTalk.Component.Interop.IPropertyBag](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPropertyBag 'Microsoft.BizTalk.Component.Interop.IPropertyBag')

The [Microsoft.BizTalk.Component.Interop.IPropertyBag](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPropertyBag 'Microsoft.BizTalk.Component.Interop.IPropertyBag') bag instance.

<a name='Be.Stateless.BizTalk.Component.Interop.PropertyBag.ReadProperty(thisMicrosoft.BizTalk.Component.Interop.IPropertyBag,string,System.Action_string_).name'></a>

`name` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The name of the property to read from the [Microsoft.BizTalk.Component.Interop.IPropertyBag](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPropertyBag 'Microsoft.BizTalk.Component.Interop.IPropertyBag') bag.

<a name='Be.Stateless.BizTalk.Component.Interop.PropertyBag.ReadProperty(thisMicrosoft.BizTalk.Component.Interop.IPropertyBag,string,System.Action_string_).setter'></a>

`setter` [System.Action&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-1 'System.Action`1')[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Action-1 'System.Action`1')

The property setter to assign the value read from the [Microsoft.BizTalk.Component.Interop.IPropertyBag](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPropertyBag 'Microsoft.BizTalk.Component.Interop.IPropertyBag') bag if not null nor empty.