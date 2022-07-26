#### [Be.Stateless.BizTalk.Stream.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.Stream.Extensions](Be.Stateless.BizTalk.Unit.Stream.Extensions.md 'Be.Stateless.BizTalk.Unit.Stream.Extensions').[StreamExtensions](StreamExtensions.md 'Be.Stateless.BizTalk.Unit.Stream.Extensions.StreamExtensions')

## StreamExtensions.IsValidZipArchive(this Stream) Method

This extension method uses [System.IO.Compression.ZipArchive](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Compression.ZipArchive 'System.IO.Compression.ZipArchive') constructor to check if the stream contains the data of a valid
Zip Archive.

```csharp
public static bool IsValidZipArchive(this System.IO.Stream stream);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Unit.Stream.Extensions.StreamExtensions.IsValidZipArchive(thisSystem.IO.Stream).stream'></a>

`stream` [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')

The stream to check if it is the in zip archive format

#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')  
true if the stream is in the zip archive format, false otherwise

### Remarks
This is an adaptation of an accepted way to check that a Zip File is valid by leveraging the [System.IO.InvalidDataException](https://docs.microsoft.com/en-us/dotnet/api/System.IO.InvalidDataException 'System.IO.InvalidDataException'), see the following article: <a href="https://stackoverflow.com/questions/38970926/validating-zip-files-using-system-io-compression">Validating zip
files using System.IO.Compression</a>.