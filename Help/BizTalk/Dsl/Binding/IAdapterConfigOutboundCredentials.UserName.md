#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[IAdapterConfigOutboundCredentials](IAdapterConfigOutboundCredentials.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigOutboundCredentials')

## IAdapterConfigOutboundCredentials.UserName Property

Specify the user name to use for authentication with the destination server when the [UseSSO](IAdapterConfigSSO.UseSSO.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigSSO.UseSSO') property is set to `False`.

```csharp
string UserName { get; set; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks

You do not have to use the domain\user format for this property.

It defaults to [System.String.Empty](https://docs.microsoft.com/en-us/dotnet/api/System.String.Empty 'System.String.Empty').