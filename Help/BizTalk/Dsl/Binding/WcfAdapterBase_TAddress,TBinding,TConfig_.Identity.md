#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfAdapterBase&lt;TAddress,TBinding,TConfig&gt;](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')

## WcfAdapterBase<TAddress,TBinding,TConfig>.Identity Property

Specify the identity of the service that this receive location provides.

```csharp
public System.ServiceModel.Configuration.IdentityElement Identity { get; set; }
```

Implements [Identity](IAdapterConfigIdentity.Identity.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigIdentity.Identity')

#### Property Value
[System.ServiceModel.Configuration.IdentityElement](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Configuration.IdentityElement 'System.ServiceModel.Configuration.IdentityElement')

### Example
XML Blob example: 

```csharp
&lt;identity&gt;
  &lt;userPrincipalName value="username@contoso.com" /&gt;
&lt;/identity&gt;
```

### Remarks

The values that can be specified for the Identity property differ according to the security configuration. These
settings enable the client to authenticate this receive location. In the handshake process between the client and
service, the Windows Communication Foundation (WCF) infrastructure will ensure that the identity of the expected
service matches the values of this element.

It defaults to [System.String.Empty](https://docs.microsoft.com/en-us/dotnet/api/System.String.Empty 'System.String.Empty').