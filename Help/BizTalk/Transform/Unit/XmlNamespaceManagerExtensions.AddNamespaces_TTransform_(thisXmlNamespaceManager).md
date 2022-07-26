#### [Be.Stateless.BizTalk.Transform.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.Xml.Extensions](Be.Stateless.BizTalk.Unit.Xml.Extensions.md 'Be.Stateless.BizTalk.Unit.Xml.Extensions').[XmlNamespaceManagerExtensions](XmlNamespaceManagerExtensions.md 'Be.Stateless.BizTalk.Unit.Xml.Extensions.XmlNamespaceManagerExtensions')

## XmlNamespaceManagerExtensions.AddNamespaces<TTransform>(this XmlNamespaceManager) Method

Add all the namespaces and their prefixes declared in a given [Microsoft.XLANGs.BaseTypes.TransformBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.TransformBase 'Microsoft.XLANGs.BaseTypes.TransformBase')-derived the XSLT transform.

```csharp
public static System.Xml.XmlNamespaceManager AddNamespaces<TTransform>(this System.Xml.XmlNamespaceManager xmlNamespaceManager)
    where TTransform : Microsoft.XLANGs.BaseTypes.TransformBase, new();
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Unit.Xml.Extensions.XmlNamespaceManagerExtensions.AddNamespaces_TTransform_(thisSystem.Xml.XmlNamespaceManager).TTransform'></a>

`TTransform`

The [Microsoft.XLANGs.BaseTypes.TransformBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.TransformBase 'Microsoft.XLANGs.BaseTypes.TransformBase')-derived XSLT transform to get the namespaces to declare from.
#### Parameters

<a name='Be.Stateless.BizTalk.Unit.Xml.Extensions.XmlNamespaceManagerExtensions.AddNamespaces_TTransform_(thisSystem.Xml.XmlNamespaceManager).xmlNamespaceManager'></a>

`xmlNamespaceManager` [System.Xml.XmlNamespaceManager](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlNamespaceManager 'System.Xml.XmlNamespaceManager')

The [System.Xml.XmlNamespaceManager](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlNamespaceManager 'System.Xml.XmlNamespaceManager') to which to add the namespace declared in the given [TTransform](XmlNamespaceManagerExtensions.AddNamespaces_TTransform_(thisXmlNamespaceManager).md#Be.Stateless.BizTalk.Unit.Xml.Extensions.XmlNamespaceManagerExtensions.AddNamespaces_TTransform_(thisSystem.Xml.XmlNamespaceManager).TTransform 'Be.Stateless.BizTalk.Unit.Xml.Extensions.XmlNamespaceManagerExtensions.AddNamespaces<TTransform>(this System.Xml.XmlNamespaceManager).TTransform')[Microsoft.XLANGs.BaseTypes.TransformBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.TransformBase 'Microsoft.XLANGs.BaseTypes.TransformBase') transform.

#### Returns
[System.Xml.XmlNamespaceManager](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlNamespaceManager 'System.Xml.XmlNamespaceManager')  
The [System.Xml.XmlNamespaceManager](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlNamespaceManager 'System.Xml.XmlNamespaceManager') to which the namespace declarations have been added.