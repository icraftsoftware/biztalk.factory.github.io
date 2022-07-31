#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfBasicHttpAdapter](WcfBasicHttpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpAdapter').[Inbound](WcfBasicHttpAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBasicHttpAdapter.Inbound')

## WcfBasicHttpAdapter.Inbound.UseSSO Property

Specify whether to use Enterprise Single Sign-On (SSO) to retrieve client credentials to issue an SSO ticket.

```csharp
public bool UseSSO { get; set; }
```

Implements [UseSSO](IAdapterConfigSSO.UseSSO.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSSO.UseSSO')

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks

For more information about the security configurations supporting SSO, see the section "Enterprise Single Sign-On
Supportability for the WCF-BasicHttp Receive Adapter" in [WCF-BasicHttp
            Transport Properties Dialog Box, Receive, Security Tab](https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-basichttp-transport-properties-dialog-box-receive-security-tab 'https://docs.microsoft.com/en-us/biztalk/core/technical-reference/wcf-basichttp-transport-properties-dialog-box-receive-security-tab').

It defaults to `False`.