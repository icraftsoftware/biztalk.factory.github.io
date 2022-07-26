#### [Be.Stateless.BizTalk.Xml](README.md 'README')
### [Be.Stateless.BizTalk.Xml.Xsl](Be.Stateless.BizTalk.Xml.Xsl.md 'Be.Stateless.BizTalk.Xml.Xsl').[XslCompiledTransformDescriptor](XslCompiledTransformDescriptor.md 'Be.Stateless.BizTalk.Xml.Xsl.XslCompiledTransformDescriptor')

## XslCompiledTransformDescriptor.Arguments Property

The cloneable [Be.Stateless.Xml.Xsl.XsltArgumentList](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.Xml.Xsl.XsltArgumentList 'Be.Stateless.Xml.Xsl.XsltArgumentList') equivalent of the [Microsoft.XLANGs.BaseTypes.TransformBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.TransformBase 'Microsoft.XLANGs.BaseTypes.TransformBase')-derived [Microsoft.XLANGs.BaseTypes.TransformBase.TransformArgs](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.TransformBase.TransformArgs 'Microsoft.XLANGs.BaseTypes.TransformBase.TransformArgs').

```csharp
public Be.Stateless.Xml.Xsl.XsltArgumentList Arguments { get; }
```

#### Property Value
[Be.Stateless.Xml.Xsl.XsltArgumentList](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.Xml.Xsl.XsltArgumentList 'Be.Stateless.Xml.Xsl.XsltArgumentList')

### Remarks
Relying on the cloneable [Be.Stateless.Xml.Xsl.XsltArgumentList](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.Xml.Xsl.XsltArgumentList 'Be.Stateless.Xml.Xsl.XsltArgumentList') allows a [XslCompiledTransformDescriptor](XslCompiledTransformDescriptor.md 'Be.Stateless.BizTalk.Xml.Xsl.XslCompiledTransformDescriptor') not to keep a reference on a [Microsoft.XLANGs.BaseTypes.TransformBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.TransformBase 'Microsoft.XLANGs.BaseTypes.TransformBase') instance.