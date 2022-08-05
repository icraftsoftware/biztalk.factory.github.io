#### [Be.Stateless.BizTalk.Pipeline.Components](README.md 'README')
### [Be.Stateless.BizTalk.Component.Interop](Be.Stateless.BizTalk.Component.Interop.md 'Be.Stateless.BizTalk.Component.Interop')

## PropertyBag Class

[Microsoft.BizTalk.Component.Interop.IPropertyBag](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPropertyBag 'Microsoft.BizTalk.Component.Interop.IPropertyBag') extension methods to read and write individual properties in a type-safe way.

```csharp
public static class PropertyBag
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; PropertyBag

| Methods | |
| :--- | :--- |
| [ReadProperty(this IPropertyBag, string, Action&lt;bool&gt;)](PropertyBag.ReadProperty(thisIPropertyBag,string,Action_bool_).md 'Be.Stateless.BizTalk.Component.Interop.PropertyBag.ReadProperty(this Microsoft.BizTalk.Component.Interop.IPropertyBag, string, System.Action<bool>)') | Read a [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') property value. |
| [ReadProperty(this IPropertyBag, string, Action&lt;int&gt;)](PropertyBag.ReadProperty(thisIPropertyBag,string,Action_int_).md 'Be.Stateless.BizTalk.Component.Interop.PropertyBag.ReadProperty(this Microsoft.BizTalk.Component.Interop.IPropertyBag, string, System.Action<int>)') | Read a [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') property value. |
| [ReadProperty(this IPropertyBag, string, Action&lt;string&gt;)](PropertyBag.ReadProperty(thisIPropertyBag,string,Action_string_).md 'Be.Stateless.BizTalk.Component.Interop.PropertyBag.ReadProperty(this Microsoft.BizTalk.Component.Interop.IPropertyBag, string, System.Action<string>)') | Read a [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') property value. |
| [ReadProperty&lt;T&gt;(this IPropertyBag, string, Action&lt;T&gt;)](PropertyBag.ReadProperty_T_(thisIPropertyBag,string,Action_T_).md 'Be.Stateless.BizTalk.Component.Interop.PropertyBag.ReadProperty<T>(this Microsoft.BizTalk.Component.Interop.IPropertyBag, string, System.Action<T>)') | Read and assign an [System.Enum](https://docs.microsoft.com/en-us/dotnet/api/System.Enum 'System.Enum') property value. |
| [WriteProperty(this IPropertyBag, string, bool)](PropertyBag.WriteProperty(thisIPropertyBag,string,bool).md 'Be.Stateless.BizTalk.Component.Interop.PropertyBag.WriteProperty(this Microsoft.BizTalk.Component.Interop.IPropertyBag, string, bool)') | Write a property value to the [Microsoft.BizTalk.Component.Interop.IPropertyBag](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPropertyBag 'Microsoft.BizTalk.Component.Interop.IPropertyBag') bag. |
| [WriteProperty(this IPropertyBag, string, int)](PropertyBag.WriteProperty(thisIPropertyBag,string,int).md 'Be.Stateless.BizTalk.Component.Interop.PropertyBag.WriteProperty(this Microsoft.BizTalk.Component.Interop.IPropertyBag, string, int)') | Write a property value to the [Microsoft.BizTalk.Component.Interop.IPropertyBag](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPropertyBag 'Microsoft.BizTalk.Component.Interop.IPropertyBag') bag. |
| [WriteProperty(this IPropertyBag, string, string)](PropertyBag.WriteProperty(thisIPropertyBag,string,string).md 'Be.Stateless.BizTalk.Component.Interop.PropertyBag.WriteProperty(this Microsoft.BizTalk.Component.Interop.IPropertyBag, string, string)') | Write a property value to the [Microsoft.BizTalk.Component.Interop.IPropertyBag](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPropertyBag 'Microsoft.BizTalk.Component.Interop.IPropertyBag') bag. |
| [WriteProperty&lt;T&gt;(this IPropertyBag, string, T)](PropertyBag.WriteProperty_T_(thisIPropertyBag,string,T).md 'Be.Stateless.BizTalk.Component.Interop.PropertyBag.WriteProperty<T>(this Microsoft.BizTalk.Component.Interop.IPropertyBag, string, T)') | Write an [System.Enum](https://docs.microsoft.com/en-us/dotnet/api/System.Enum 'System.Enum') property value to the [Microsoft.BizTalk.Component.Interop.IPropertyBag](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPropertyBag 'Microsoft.BizTalk.Component.Interop.IPropertyBag') bag. |
