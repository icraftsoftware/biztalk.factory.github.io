#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[FtpAdapter](FtpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter').[Inbound](FtpAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound')

## FtpAdapter.Inbound.BeforeGet Property

Specify the FTP commands to run before the file `GET`. Separate commands with a semicolon (`;`).

```csharp
public string BeforeGet { get; set; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks
`QUIT` command is not supported before the file `GET`.