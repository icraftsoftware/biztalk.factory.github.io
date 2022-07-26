#### [Be.Stateless.Stream.Unit](README.md 'README')
### [Be.Stateless.Unit.Resources](Be.Stateless.Unit.Resources.md 'Be.Stateless.Unit.Resources')

## IResourceManager Interface

```csharp
public interface IResourceManager
```

| Methods | |
| :--- | :--- |
| [Load(string)](IResourceManager.Load(string).md 'Be.Stateless.Unit.Resources.IResourceManager.Load(string)') | Loads a [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') embedded in the calling assembly. |
| [Load&lt;T&gt;(string, Func&lt;Stream,T&gt;)](IResourceManager.Load_T_(string,Func_Stream,T_).md 'Be.Stateless.Unit.Resources.IResourceManager.Load<T>(string, System.Func<System.IO.Stream,T>)') | Loads and deserializes a resource embedded in the calling assembly. |
| [LoadString(string)](IResourceManager.LoadString(string).md 'Be.Stateless.Unit.Resources.IResourceManager.LoadString(string)') | Loads and deserializes a [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') embedded in the calling assembly. |
| [LoadTransform(string)](IResourceManager.LoadTransform(string).md 'Be.Stateless.Unit.Resources.IResourceManager.LoadTransform(string)') | Loads and deserializes an [System.Xml.Xsl.XslCompiledTransform](https://docs.microsoft.com/en-us/dotnet/api/System.Xml.Xsl.XslCompiledTransform 'System.Xml.Xsl.XslCompiledTransform') embedded in the calling assembly. |
| [LoadXmlString(string)](IResourceManager.LoadXmlString(string).md 'Be.Stateless.Unit.Resources.IResourceManager.LoadXmlString(string)') | Loads and deserializes an XML [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') embedded in the calling assembly. |
