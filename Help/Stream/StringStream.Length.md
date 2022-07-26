#### [Be.Stateless.Stream](README.md 'README')
### [Be.Stateless.IO](Be.Stateless.IO.md 'Be.Stateless.IO').[StringStream](StringStream.md 'Be.Stateless.IO.StringStream')

## StringStream.Length Property

When overridden in a derived class, gets the length in bytes of the stream.

```csharp
public override long Length { get; }
```

#### Property Value
[System.Int64](https://docs.microsoft.com/en-us/dotnet/api/System.Int64 'System.Int64')

#### Exceptions

[System.NotSupportedException](https://docs.microsoft.com/en-us/dotnet/api/System.NotSupportedException 'System.NotSupportedException')  
A class derived from Stream does not support seeking.

[System.ObjectDisposedException](https://docs.microsoft.com/en-us/dotnet/api/System.ObjectDisposedException 'System.ObjectDisposedException')  
Methods were called after the stream was closed.

### Remarks
The length of the string multiplied by two, since a [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') is a series of Unicode UTF-16 code points and each code point is 2 bytes. Notice the
length will also account for the extra 2-byte BOM preamble.

### See Also
- [http://msdn.microsoft.com/en-us/magazine/cc163768.aspx](http://msdn.microsoft.com/en-us/magazine/cc163768.aspx 'http://msdn.microsoft.com/en-us/magazine/cc163768.aspx')