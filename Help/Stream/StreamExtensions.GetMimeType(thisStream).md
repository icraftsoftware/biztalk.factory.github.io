#### [Be.Stateless.Stream](README.md 'README')
### [Be.Stateless.IO.Extensions](Be.Stateless.IO.Extensions.md 'Be.Stateless.IO.Extensions').[StreamExtensions](StreamExtensions.md 'Be.Stateless.IO.Extensions.StreamExtensions')

## StreamExtensions.GetMimeType(this Stream) Method

Determines the MIME type from the data stream provided.

```csharp
public static string GetMimeType(this System.IO.Stream stream);
```
#### Parameters

<a name='Be.Stateless.IO.Extensions.StreamExtensions.GetMimeType(thisSystem.IO.Stream).stream'></a>

`stream` [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')

The stream that contains the data to be sniffed.

#### Returns
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks
MIME type detection, or "data sniffing," refers to the process of determining an appropriate MIME type from binary data. The final result depends on a
combination of server-supplied MIME type headers, file name extension, and/or the data itself. Usually, only the first 256 bytes of data are significant. For
more information and a complete list of recognized MIME types, see <a href="http://msdn.microsoft.com/en-us/library/ms775147(v=vs.85).aspx">MIME Type Detection
in Internet Explorer.</a>

### See Also
- [http://msdn.microsoft.com/en-us/library/ms775107(v=vs.85).aspx](http://msdn.microsoft.com/en-us/library/ms775107(v=vs.85).aspx 'http://msdn.microsoft.com/en-us/library/ms775107(v=vs.85).aspx')
- [Microsoft.Practices.ESB.ExceptionHandling.PipelineComponents.SafeNativeMethods.GetMimeType(Stream)](Microsoft.Practices.ESB.ExceptionHandling.PipelineComponents.SafeNativeMethods.GetMimeType(Stream) 'Microsoft.Practices.ESB.ExceptionHandling.PipelineComponents.SafeNativeMethods.GetMimeType(Stream)')
- [http://forums.asp.net/t/1041821.aspx/1?Determine+Mime+Type+for+server+side+file](http://forums.asp.net/t/1041821.aspx/1?Determine+Mime+Type+for+server+side+file 'http://forums.asp.net/t/1041821.aspx/1?Determine+Mime+Type+for+server+side+file')