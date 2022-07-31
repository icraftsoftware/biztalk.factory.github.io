#### [Be.Stateless.Dsl.Configuration](README.md 'README')
### [Be.Stateless.Dsl.Configuration](Be.Stateless.Dsl.Configuration.md 'Be.Stateless.Dsl.Configuration')

## ConfigurationElement Class

```csharp
public class ConfigurationElement
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; ConfigurationElement

Derived  
&#8627; [ConfigurationRootElement](ConfigurationRootElement.md 'Be.Stateless.Dsl.Configuration.ConfigurationRootElement')

| Properties | |
| :--- | :--- |
| [HasConfigurationElements](ConfigurationElement.HasConfigurationElements.md 'Be.Stateless.Dsl.Configuration.ConfigurationElement.HasConfigurationElements') | |
| [Name](ConfigurationElement.Name.md 'Be.Stateless.Dsl.Configuration.ConfigurationElement.Name') | |
| [Path](ConfigurationElement.Path.md 'Be.Stateless.Dsl.Configuration.ConfigurationElement.Path') | |

| Methods | |
| :--- | :--- |
| [Apply(SpecificationElement)](ConfigurationElement.Apply(SpecificationElement).md 'Be.Stateless.Dsl.Configuration.ConfigurationElement.Apply(Be.Stateless.Dsl.Configuration.SpecificationElement)') | Apply the children [SpecificationElement](SpecificationElement.md 'Be.Stateless.Dsl.Configuration.SpecificationElement')s of the [SpecificationElement](SpecificationElement.md 'Be.Stateless.Dsl.Configuration.SpecificationElement')[specificationElement](ConfigurationElement.Apply(SpecificationElement).md#Be.Stateless.Dsl.Configuration.ConfigurationElement.Apply(Be.Stateless.Dsl.Configuration.SpecificationElement).specificationElement 'Be.Stateless.Dsl.Configuration.ConfigurationElement.Apply(Be.Stateless.Dsl.Configuration.SpecificationElement).specificationElement') to the children of the current [ConfigurationElement](ConfigurationElement.md 'Be.Stateless.Dsl.Configuration.ConfigurationElement') while transforming —rewriting in place— the [SpecificationElement](SpecificationElement.md 'Be.Stateless.Dsl.Configuration.SpecificationElement')s into their inverse —undo— [SpecificationElement](SpecificationElement.md 'Be.Stateless.Dsl.Configuration.SpecificationElement')s on the fly. |
| [ConfigurationAttribute(XName)](ConfigurationElement.ConfigurationAttribute(XName).md 'Be.Stateless.Dsl.Configuration.ConfigurationElement.ConfigurationAttribute(System.Xml.Linq.XName)') | |
| [ConfigurationAttributes()](ConfigurationElement.ConfigurationAttributes().md 'Be.Stateless.Dsl.Configuration.ConfigurationElement.ConfigurationAttributes()') | |
| [ConfigurationElements()](ConfigurationElement.ConfigurationElements().md 'Be.Stateless.Dsl.Configuration.ConfigurationElement.ConfigurationElements()') | |

| Operators | |
| :--- | :--- |
| [explicit operator XElement(ConfigurationElement)](ConfigurationElement.explicitoperatorXElement(ConfigurationElement).md 'Be.Stateless.Dsl.Configuration.ConfigurationElement.op_Explicit System.Xml.Linq.XElement(Be.Stateless.Dsl.Configuration.ConfigurationElement)') | |
