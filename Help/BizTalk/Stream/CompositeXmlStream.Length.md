#### [Be.Stateless.BizTalk.Stream](README.md 'README')
### [Be.Stateless.BizTalk.Stream](Be.Stateless.BizTalk.Stream.md 'Be.Stateless.BizTalk.Stream').[CompositeXmlStream](CompositeXmlStream.md 'Be.Stateless.BizTalk.Stream.CompositeXmlStream')

## CompositeXmlStream.Length Property

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