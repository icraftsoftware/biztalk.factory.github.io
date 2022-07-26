#### [Be.Stateless.BizTalk.Pipeline.MicroComponents](README.md 'README')
### [Be.Stateless.BizTalk.MicroComponent](Be.Stateless.BizTalk.MicroComponent.md 'Be.Stateless.BizTalk.MicroComponent').[XsltRunner](XsltRunner.md 'Be.Stateless.BizTalk.MicroComponent.XsltRunner')

## XsltRunner.Encoding Property

Encoding to use for output and, if Unicode, whether to emit a byte order mark.

```csharp
public System.Text.Encoding Encoding { get; set; }
```

#### Property Value
[System.Text.Encoding](https://docs.microsoft.com/en-us/dotnet/api/System.Text.Encoding 'System.Text.Encoding')

### Remarks
It defaults to [System.Text.UTF8Encoding](https://docs.microsoft.com/en-us/dotnet/api/System.Text.UTF8Encoding 'System.Text.UTF8Encoding') with a BOM preamble.