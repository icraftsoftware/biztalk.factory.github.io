#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[Pop3Adapter](Pop3Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter')

## Pop3Adapter.Inbound Class

You use the Post Office Protocol 3 (POP3) adapter to retrieve data from a server that houses POP3 mailboxes into a
server running Microsoft BizTalk Server by means of the POP3 protocol.

```csharp
public class Pop3Adapter.Inbound : Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IInboundAdapter,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter,
Be.Stateless.BizTalk.Dsl.ISupportValidation
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [AdapterBase](AdapterBase.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase') &#129106; [LegacyAdapterBase](LegacyAdapterBase.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.LegacyAdapterBase') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.LegacyAdapterBase&lt;](LegacyAdapterBase_TValidator_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.LegacyAdapterBase<TValidator>')[Microsoft.BizTalk.Adapter.POP3.POP3AdapterManagement](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Adapter.POP3.POP3AdapterManagement 'Microsoft.BizTalk.Adapter.POP3.POP3AdapterManagement')[&gt;](LegacyAdapterBase_TValidator_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.LegacyAdapterBase<TValidator>') &#129106; [Pop3Adapter](Pop3Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter') &#129106; Inbound

Implements [IInboundAdapter](IInboundAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IInboundAdapter'), [IAdapter](IAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter'), [Be.Stateless.BizTalk.Dsl.ISupportValidation](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Dsl.ISupportValidation 'Be.Stateless.BizTalk.Dsl.ISupportValidation')

### Remarks
The POP3 receive adapter retrieves e-mail from a specified mailbox on a specified POP3 server. By default, the POP3
receive adapter applies MIME processing to the e-mail messages that it downloads and submits these messages to
BizTalk Server as multi-part BizTalk messages. The POP3 receive adapter can receive and process e-mail in the
following formats:
- Plain text
- MIME encoded
- MIME encrypted
- MIME encoded and signed
- MIME encrypted and signed

The POP3 receive adapter does not support batching.

The following authentication methods are supported for use with the POP3 adapter:
- Basic. The POP3 server uses user provided credentials for authentication. These credentials are sent in clear text.
- Digest (APOP). The POP3 server uses a digest string for authentication.
- Secure Password Authentication (SPA). The POP3 server uses current process credentials for authentication.

### See Also
- [What Is the POP3 Adapter?](https://docs.microsoft.com/en-us/biztalk/core/what-is-the-pop3-adapter 'https://docs.microsoft.com/en-us/biztalk/core/what-is-the-pop3-adapter')
- [POP3 Adapter](https://docs.microsoft.com/en-us/biztalk/core/pop3-adapter 'https://docs.microsoft.com/en-us/biztalk/core/pop3-adapter')
- [How to Configure a POP3 Receive Handler](https://docs.microsoft.com/en-us/biztalk/core/how-to-configure-a-pop3-receive-handler 'https://docs.microsoft.com/en-us/biztalk/core/how-to-configure-a-pop3-receive-handler')
- [How to Configure a POP3 Receive Location](https://docs.microsoft.com/en-us/biztalk/core/how-to-configure-a-pop3-receive-location 'https://docs.microsoft.com/en-us/biztalk/core/how-to-configure-a-pop3-receive-location')
- [POP3 Adapter Property Schema and Properties](https://docs.microsoft.com/en-us/biztalk/core/pop3-adapter-property-schema-and-properties 'https://docs.microsoft.com/en-us/biztalk/core/pop3-adapter-property-schema-and-properties')

| Constructors | |
| :--- | :--- |
| [Inbound()](Pop3Adapter.Inbound.Inbound().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.Inbound.Inbound()') | |
| [Inbound(Action&lt;Inbound&gt;)](Pop3Adapter.Inbound.Inbound(Action_Inbound_).md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.Inbound.Inbound(System.Action<Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.Inbound>)') | |

| Properties | |
| :--- | :--- |
| [ApplyMimeDecoding](Pop3Adapter.Inbound.ApplyMimeDecoding.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.Inbound.ApplyMimeDecoding') | Specify whether to apply MIME decoding to messages received by the POP3 adapter. MIME decoding is used to parse the incoming message and any attachments into a multi-part BizTalk message. |
| [AuthenticationScheme](Pop3Adapter.Inbound.AuthenticationScheme.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.Inbound.AuthenticationScheme') | Specify the type of authentication to use with the destination server. |
| [BodyPartContentType](Pop3Adapter.Inbound.BodyPartContentType.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.Inbound.BodyPartContentType') | Specify the body part content type of the incoming e-mail message to submit to BizTalk Server. This is an optional setting. |
| [BodyPartIndex](Pop3Adapter.Inbound.BodyPartIndex.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.Inbound.BodyPartIndex') | Specify the body part of the incoming e-mail message to submit to BizTalk Server. |
| [ErrorThreshold](Pop3Adapter.Inbound.ErrorThreshold.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.Inbound.ErrorThreshold') | Specify the maximum number of network or protocol errors to wait before shutting down the adapter. Specify a value of 0 to prevent the adapter from shutting down. |
| [MailServer](Pop3Adapter.Inbound.MailServer.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.Inbound.MailServer') | Specify the POP3 mail server that houses the mailbox that will be polled by the POP3 adapter. |
| [Password](Pop3Adapter.Inbound.Password.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.Inbound.Password') | Specify the user password to use for authentication with the POP3 server. |
| [PollingInterval](Pop3Adapter.Inbound.PollingInterval.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.Inbound.PollingInterval') | Specify the interval between attempts to retrieve messages from the POP3 server. |
| [Port](Pop3Adapter.Inbound.Port.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.Inbound.Port') | Specify the port for the POP3 mail server. |
| [UserName](Pop3Adapter.Inbound.UserName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.Inbound.UserName') | Specify the user name to use for authentication with the POP3 server. This property requires a value. |
| [UseSsl](Pop3Adapter.Inbound.UseSsl.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.Inbound.UseSsl') | Specify whether to use Secure Sockets Layer (SSL) to communicate with the destination server. |
| [XmlAliasedPollingInterval](Pop3Adapter.Inbound.XmlAliasedPollingInterval.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.Inbound.XmlAliasedPollingInterval') | |
| [XmlAliasedPollingUnitOfMeasure](Pop3Adapter.Inbound.XmlAliasedPollingUnitOfMeasure.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.Inbound.XmlAliasedPollingUnitOfMeasure') | |

| Methods | |
| :--- | :--- |
| [GetAddress()](Pop3Adapter.Inbound.GetAddress().md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Pop3Adapter.Inbound.GetAddress()') | |
