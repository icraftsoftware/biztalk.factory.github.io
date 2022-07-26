#### [Be.Stateless.Xml](README.md 'README')
### [Be.Stateless.Xml](Be.Stateless.Xml.md 'Be.Stateless.Xml').[XmlBuilderReader](XmlBuilderReader.md 'Be.Stateless.Xml.XmlBuilderReader')

## XmlBuilderReader.GetAttribute(int) Method

Gets the value of the attribute with the specified index.

```csharp
public override string GetAttribute(int i);
```
#### Parameters

<a name='Be.Stateless.Xml.XmlBuilderReader.GetAttribute(int).i'></a>

`i` [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

The index of the attribute. The index is zero-based.

#### Returns
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')  
The value of the specified attribute.

#### Exceptions

[System.ArgumentOutOfRangeException](https://docs.microsoft.com/en-us/dotnet/api/System.ArgumentOutOfRangeException 'System.ArgumentOutOfRangeException')  
[i](XmlBuilderReader.GetAttribute(int).md#Be.Stateless.Xml.XmlBuilderReader.GetAttribute(int).i 'Be.Stateless.Xml.XmlBuilderReader.GetAttribute(int).i') is out of range. It must be non-negative and less than the size of the attribute collection.

### Remarks
This method does not move the reader.