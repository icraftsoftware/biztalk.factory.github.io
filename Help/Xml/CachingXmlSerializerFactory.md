#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Xml.Serialization](Be.Stateless.Xml.Serialization.md 'Be.Stateless.Xml.Serialization')

## CachingXmlSerializerFactory Class

Cache dynamically generated assemblies.

```csharp
public static class CachingXmlSerializerFactory
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; CachingXmlSerializerFactory

### Remarks

To increase performance, the XML serialization infrastructure dynamically generates assemblies to serialize and
deserialize specified types. The infrastructure finds and reuses those assemblies. This behavior occurs only when using
the following constructors:
- [System.Xml.Serialization.XmlSerializer.#ctor(System.Type)](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Serialization.XmlSerializer.#ctor#System_Xml_Serialization_XmlSerializer_#ctor_System_Type_ 'System.Xml.Serialization.XmlSerializer.#ctor(System.Type)')
- [System.Xml.Serialization.XmlSerializer.#ctor(System.Type,System.String)](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Serialization.XmlSerializer.#ctor#System_Xml_Serialization_XmlSerializer_#ctor_System_Type,System_String_ 'System.Xml.Serialization.XmlSerializer.#ctor(System.Type,System.String)')

If you use any of the other constructors, multiple versions of the same assembly are generated and never unloaded, which
results in a memory leak and poor performance.

This class takes care of caching the dynamically generated assemblies should the serialization infrastructure not do it.

### See Also
- [Dynamically Generated Assemblies](https://docs.microsoft.com/en-us/dotnet/api/system.xml.serialization.xmlserializer#dynamically-generated-assemblies 'https://docs.microsoft.com/en-us/dotnet/api/system.xml.serialization.xmlserializer#dynamically-generated-assemblies')

| Methods | |
| :--- | :--- |
| [Create(Type, XmlAttributeOverrides)](CachingXmlSerializerFactory.Create(Type,XmlAttributeOverrides).md 'Be.Stateless.Xml.Serialization.CachingXmlSerializerFactory.Create(System.Type, System.Xml.Serialization.XmlAttributeOverrides)') | |
| [Create(Type, XmlRootAttribute)](CachingXmlSerializerFactory.Create(Type,XmlRootAttribute).md 'Be.Stateless.Xml.Serialization.CachingXmlSerializerFactory.Create(System.Type, System.Xml.Serialization.XmlRootAttribute)') | |
| [Create(Type)](CachingXmlSerializerFactory.Create(Type).md 'Be.Stateless.Xml.Serialization.CachingXmlSerializerFactory.Create(System.Type)') | |
