#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[FtpAdapter](FtpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter').[Inbound](FtpAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FtpAdapter.Inbound')

## FtpAdapter.Inbound.MaximumNumberOfFiles Property

Specify the maximum number of files per BizTalk Server batch.

```csharp
public uint MaximumNumberOfFiles { get; set; }
```

#### Property Value
[System.UInt32](https://docs.microsoft.com/en-us/dotnet/api/System.UInt32 'System.UInt32')

### Remarks

Zero (`0`) indicates no limit.

It defaults to zero (`0`).