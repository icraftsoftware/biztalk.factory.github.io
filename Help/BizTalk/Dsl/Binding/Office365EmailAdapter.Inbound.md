#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[Office365EmailAdapter](Office365EmailAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter')

## Office365EmailAdapter.Inbound Class

The Office 365 Outlook Email Adapter allows you to receive mails from your Office 365 Outlook Email from Microsoft
BizTalk Server.

```csharp
public class Office365EmailAdapter.Inbound : Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter<Microsoft.BizTalk.Adapter.Office365.Mail.MailRLConfig>,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IInboundAdapter,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter,
Be.Stateless.BizTalk.Dsl.ISupportValidation
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [AdapterBase](AdapterBase.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter&lt;](Office365EmailAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter<TConfig>')[Microsoft.BizTalk.Adapter.Office365.Mail.MailRLConfig](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.Office365.Mail.MailRLConfig 'Microsoft.BizTalk.Adapter.Office365.Mail.MailRLConfig')[&gt;](Office365EmailAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter<TConfig>') &#129106; Inbound

Implements [IInboundAdapter](IInboundAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IInboundAdapter'), [IAdapter](IAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter'), [Be.Stateless.BizTalk.Dsl.ISupportValidation](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.ISupportValidation 'Be.Stateless.BizTalk.Dsl.ISupportValidation')

### See Also
- [Receive email using a receive port](https://docs.microsoft.com/en-us/biztalk/core/office365-mail-adapter#receive-email-using-a-receive-port 'https://docs.microsoft.com/en-us/biztalk/core/office365-mail-adapter#receive-email-using-a-receive-port')

| Constructors | |
| :--- | :--- |
| [Inbound()](Office365EmailAdapter.Inbound.Inbound().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter.Inbound.Inbound()') | |
| [Inbound(Action&lt;Inbound&gt;)](Office365EmailAdapter.Inbound.Inbound(Action_Inbound_).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter.Inbound.Inbound(System.Action<Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter.Inbound>)') | |

| Properties | |
| :--- | :--- |
| [DeliverMime](Office365EmailAdapter.Inbound.DeliverMime.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter.Inbound.DeliverMime') | `true` to fetch an email in its raw `MIME` representation or `false` to process its content, i.e.             to fetch its `MIME`-decoded body instead. |
| [EmailAddress](Office365EmailAdapter.Inbound.EmailAddress.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter.Inbound.EmailAddress') | The email address to fetch emails from. |
| [FolderName](Office365EmailAdapter.Inbound.FolderName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter.Inbound.FolderName') | The folder to fetch emails from. |
| [IncludeAttachments](Office365EmailAdapter.Inbound.IncludeAttachments.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter.Inbound.IncludeAttachments') | Whether to retrieve email's attachments as parts of the BizTalk message. |
| [PostActionTask](Office365EmailAdapter.Inbound.PostActionTask.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter.Inbound.PostActionTask') | The action to be performed after an email is fetched. |
| [StartTime](Office365EmailAdapter.Inbound.StartTime.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter.Inbound.StartTime') | The minimum received TimeStamp of an email in Office 365 Outlook. |
| [UnreadMailsOnly](Office365EmailAdapter.Inbound.UnreadMailsOnly.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter.Inbound.UnreadMailsOnly') | Whether to fetch only unread email. |

| Methods | |
| :--- | :--- |
| [GetAddress()](Office365EmailAdapter.Inbound.GetAddress().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter.Inbound.GetAddress()') | |
| [Validate()](Office365EmailAdapter.Inbound.Validate().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter.Inbound.Validate()') | |
