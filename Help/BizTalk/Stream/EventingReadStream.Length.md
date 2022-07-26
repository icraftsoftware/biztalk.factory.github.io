#### [Be.Stateless.BizTalk.Stream](README.md 'README')
### [Be.Stateless.BizTalk.Stream](Be.Stateless.BizTalk.Stream.md 'Be.Stateless.BizTalk.Stream').[EventingReadStream](EventingReadStream.md 'Be.Stateless.BizTalk.Stream.EventingReadStream')

## EventingReadStream.Length Property

This property returns the inner stream length in bytes.

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
The [Length](EventingReadStream.Length.md 'Be.Stateless.BizTalk.Stream.EventingReadStream.Length') will be computed while the stream is being read and will consequently only be available and
known accurately once the whole stream has been exhausted. While being read, [Length](EventingReadStream.Length.md 'Be.Stateless.BizTalk.Stream.EventingReadStream.Length') will therefore
throw a [System.NotSupportedException](https://docs.microsoft.com/en-us/dotnet/api/System.NotSupportedException 'System.NotSupportedException') exception.

### See Also
- [InnerStream](EventingReadStream.InnerStream.md 'Be.Stateless.BizTalk.Stream.EventingReadStream.InnerStream')
- [CanSeek](EventingReadStream.CanSeek.md 'Be.Stateless.BizTalk.Stream.EventingReadStream.CanSeek')