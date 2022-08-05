#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[Pop3Adapter](Pop3Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter').[Inbound](Pop3Adapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.Inbound')

## Pop3Adapter.Inbound.UserName Property

Specify the user name to use for authentication with the POP3 server. This property requires a value.

```csharp
public string UserName { get; set; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks
The account specified for the [UserName](Pop3Adapter.Inbound.UserName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.Inbound.UserName') property must have the ability to logon to the network. The
POP3 adapter connects to the mailbox associated with the account specified for the [UserName](Pop3Adapter.Inbound.UserName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.Inbound.UserName')
property. Therefore it is not possible to use the POP3 Adapter to connect to a mailbox other than the mailbox
assigned to the specified account. For example, even if multiple accounts have Read permissions to the mailbox
associated with a particular account, only the actual account name can be specified for [UserName](Pop3Adapter.Inbound.UserName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.Inbound.UserName').