#### [Be.Stateless.BizTalk.ServiceModel](README.md 'README')
### [Be.Stateless.BizTalk.ServiceModel.Security](Be.Stateless.BizTalk.ServiceModel.Security.md 'Be.Stateless.BizTalk.ServiceModel.Security').[AuthorizationTokenCache](AuthorizationTokenCache.md 'Be.Stateless.BizTalk.ServiceModel.Security.AuthorizationTokenCache')

## AuthorizationTokenCache.AddOrGetExistingAuthorizationToken(string, Func<IAuthorizationToken>) Method

```csharp
public Be.Stateless.BizTalk.ServiceModel.Security.Tokens.IAuthorizationToken AddOrGetExistingAuthorizationToken(string key, System.Func<Be.Stateless.BizTalk.ServiceModel.Security.Tokens.IAuthorizationToken> authorizationTokenFactory);
```
#### Parameters

<a name='Be.Stateless.BizTalk.ServiceModel.Security.AuthorizationTokenCache.AddOrGetExistingAuthorizationToken(string,System.Func_Be.Stateless.BizTalk.ServiceModel.Security.Tokens.IAuthorizationToken_).key'></a>

`key` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

<a name='Be.Stateless.BizTalk.ServiceModel.Security.AuthorizationTokenCache.AddOrGetExistingAuthorizationToken(string,System.Func_Be.Stateless.BizTalk.ServiceModel.Security.Tokens.IAuthorizationToken_).authorizationTokenFactory'></a>

`authorizationTokenFactory` [System.Func&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-1 'System.Func`1')[IAuthorizationToken](IAuthorizationToken.md 'Be.Stateless.BizTalk.ServiceModel.Security.Tokens.IAuthorizationToken')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-1 'System.Func`1')

#### Returns
[IAuthorizationToken](IAuthorizationToken.md 'Be.Stateless.BizTalk.ServiceModel.Security.Tokens.IAuthorizationToken')