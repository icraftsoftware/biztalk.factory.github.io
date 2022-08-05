#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[HttpAdapter](HttpAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter').[Inbound](HttpAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.HttpAdapter.Inbound')

## HttpAdapter.Inbound.UseSSO Property

Specifies whether the HTTP adapter will issue the SSO ticket to messages that arrive on this receive location.

```csharp
public bool UseSSO { get; set; }
```

Implements [UseSSO](IAdapterConfigSSO.UseSSO.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSSO.UseSSO')

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks

If this option is enabled then you must also enable the option to Allow Tickets at the SSO System level. The Allow
Tickets option is configurable on the Options tab of the SSO System Properties dialog box available in the SSO
Administration MMC interface. If this option is enabled and the Allow Tickets option at the SSO System level is
not enabled then any messages received by this receive location will be suspended.

It defaults to `False`.