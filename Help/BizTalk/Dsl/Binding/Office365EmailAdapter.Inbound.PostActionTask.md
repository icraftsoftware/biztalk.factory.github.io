#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[Office365EmailAdapter](Office365EmailAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter').[Inbound](Office365EmailAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter.Inbound')

## Office365EmailAdapter.Inbound.PostActionTask Property

The action to be performed after an email is fetched.

```csharp
public Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter.PostActionTask PostActionTask { get; set; }
```

#### Property Value
[PostActionTask](Office365EmailAdapter.PostActionTask.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter.PostActionTask')

### Remarks

- [None](Office365EmailAdapter.PostActionTask.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter.PostActionTask.None 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter.PostActionTask.None') is the default and does nothing after email is received by
              Microsoft BizTalk Server.
- [MarkAsRead](Office365EmailAdapter.PostActionTask.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter.PostActionTask.MarkAsRead 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter.PostActionTask.MarkAsRead') implies, that after an email is received by
              Microsoft BizTalk Server, the email in your mailbox is marked as read.
- [Delete](Office365EmailAdapter.PostActionTask.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter.PostActionTask.Delete 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Office365EmailAdapter.PostActionTask.Delete') implies, that after an email is received by Microsoft
              BizTalk Server, the email in your mailbox is deleted.

Post actions are performed on a best-effort basis.