#### [Be.Stateless.Stream.Unit](README.md 'README')
### [Be.Stateless.Unit.Resources](Be.Stateless.Unit.Resources.md 'Be.Stateless.Unit.Resources').[IResourceManager](IResourceManager.md 'Be.Stateless.Unit.Resources.IResourceManager')

## IResourceManager.LoadXmlString(string) Method

Loads and deserializes an XML [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') embedded in the calling assembly.

```csharp
string LoadXmlString(string name);
```
#### Parameters

<a name='Be.Stateless.Unit.Resources.IResourceManager.LoadXmlString(string).name'></a>

`name` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The name of the XML [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') resource.

#### Returns
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')  
The deserialized XML [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String').

### Remarks
Contrasting with [LoadString(string)](IResourceManager.LoadString(string).md 'Be.Stateless.Unit.Resources.IResourceManager.LoadString(string)'), this methods strips the XML string from all new-line and indentation
formatting characters.