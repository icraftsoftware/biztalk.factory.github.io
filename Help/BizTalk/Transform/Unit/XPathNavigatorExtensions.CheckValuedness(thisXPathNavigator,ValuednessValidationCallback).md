#### [Be.Stateless.BizTalk.Transform.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.Xml.XPath.Extensions](Be.Stateless.BizTalk.Unit.Xml.XPath.Extensions.md 'Be.Stateless.BizTalk.Unit.Xml.XPath.Extensions').[XPathNavigatorExtensions](XPathNavigatorExtensions.md 'Be.Stateless.BizTalk.Unit.Xml.XPath.Extensions.XPathNavigatorExtensions')

## XPathNavigatorExtensions.CheckValuedness(this XPathNavigator, ValuednessValidationCallback) Method

Test whether the XML denoted by the [System.Xml.XPath.XPathNavigator](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XPath.XPathNavigator 'System.Xml.XPath.XPathNavigator') contains any empty element or attribute.

```csharp
public static bool CheckValuedness(this System.Xml.XPath.XPathNavigator navigator, Be.Stateless.BizTalk.Unit.Xml.ValuednessValidationCallback valuednessValidationCallback);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Unit.Xml.XPath.Extensions.XPathNavigatorExtensions.CheckValuedness(thisSystem.Xml.XPath.XPathNavigator,Be.Stateless.BizTalk.Unit.Xml.ValuednessValidationCallback).navigator'></a>

`navigator` [System.Xml.XPath.XPathNavigator](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XPath.XPathNavigator 'System.Xml.XPath.XPathNavigator')

The [System.Xml.XPath.XPathNavigator](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XPath.XPathNavigator 'System.Xml.XPath.XPathNavigator') over the XML to test for valuedness.

<a name='Be.Stateless.BizTalk.Unit.Xml.XPath.Extensions.XPathNavigatorExtensions.CheckValuedness(thisSystem.Xml.XPath.XPathNavigator,Be.Stateless.BizTalk.Unit.Xml.ValuednessValidationCallback).valuednessValidationCallback'></a>

`valuednessValidationCallback` [ValuednessValidationCallback(object, ValuednessValidationCallbackArgs)](ValuednessValidationCallback(object,ValuednessValidationCallbackArgs).md 'Be.Stateless.BizTalk.Unit.Xml.ValuednessValidationCallback(object, Be.Stateless.BizTalk.Unit.Xml.ValuednessValidationCallbackArgs)')

An optional validation callback that can be used to demote the [System.Xml.Schema.XmlSeverityType](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSeverityType 'System.Xml.Schema.XmlSeverityType') so that no exception is
thrown if all the empty elements or attributes are only to be considered as [System.Xml.Schema.XmlSeverityType.Warning](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSeverityType.Warning 'System.Xml.Schema.XmlSeverityType.Warning').

#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')  
[true](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/bool 'https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/bool') if there are any empty element or attribute; [false](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/bool 'https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/bool') otherwise.

### Remarks

An element is considered empty if it has either no children nor any value; an element, which has the xsi:nil='true',
is not considered empty.

An attribute is considered empty if it has no value.

Empty elements or attributes will be considered as an [System.Xml.Schema.XmlSeverityType.Error](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSeverityType.Error 'System.Xml.Schema.XmlSeverityType.Error') condition which will entail
that an [System.Xml.XmlException](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.XmlException 'System.Xml.XmlException') will be thrown unless a [ValuednessValidationCallback(object, ValuednessValidationCallbackArgs)](ValuednessValidationCallback(object,ValuednessValidationCallbackArgs).md 'Be.Stateless.BizTalk.Unit.Xml.ValuednessValidationCallback(object, Be.Stateless.BizTalk.Unit.Xml.ValuednessValidationCallbackArgs)') validation
callback is passed to demote the severity of the error for a given element or attribute to [System.Xml.Schema.XmlSeverityType.Warning](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Schema.XmlSeverityType.Warning 'System.Xml.Schema.XmlSeverityType.Warning').