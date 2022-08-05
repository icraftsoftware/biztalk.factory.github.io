#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[FileAdapter](FileAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.FileAdapter')

## FileAdapter.NetworkCredentials Property

Credentials to use when host does not have access to network share.

```csharp
public Be.Stateless.BizTalk.Dsl.Binding.Adapter.Credentials NetworkCredentials { get; set; }
```

#### Property Value
[Credentials](Credentials.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.Credentials')

### Remarks
Alternate credentials to access the file folder cannot be supplied while accessing local drive or a mapped network
drive.