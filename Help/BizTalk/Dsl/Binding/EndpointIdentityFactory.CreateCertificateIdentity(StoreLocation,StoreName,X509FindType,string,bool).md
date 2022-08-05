#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.ServiceModel.Configuration](Be.Stateless.BizTalk.Dsl.Binding.ServiceModel.Configuration.md 'Be.Stateless.BizTalk.Dsl.Binding.ServiceModel.Configuration').[EndpointIdentityFactory](EndpointIdentityFactory.md 'Be.Stateless.BizTalk.Dsl.Binding.ServiceModel.Configuration.EndpointIdentityFactory')

## EndpointIdentityFactory.CreateCertificateIdentity(StoreLocation, StoreName, X509FindType, string, bool) Method

```csharp
public static System.ServiceModel.Configuration.IdentityElement CreateCertificateIdentity(System.Security.Cryptography.X509Certificates.StoreLocation storeLocation, System.Security.Cryptography.X509Certificates.StoreName storeName, System.Security.Cryptography.X509Certificates.X509FindType findType, string findValue, bool isChainIncluded=false);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Dsl.Binding.ServiceModel.Configuration.EndpointIdentityFactory.CreateCertificateIdentity(System.Security.Cryptography.X509Certificates.StoreLocation,System.Security.Cryptography.X509Certificates.StoreName,System.Security.Cryptography.X509Certificates.X509FindType,string,bool).storeLocation'></a>

`storeLocation` [System.Security.Cryptography.X509Certificates.StoreLocation](https://docs.microsoft.com/en-us/dotnet/api/System.Security.Cryptography.X509Certificates.StoreLocation 'System.Security.Cryptography.X509Certificates.StoreLocation')

<a name='Be.Stateless.BizTalk.Dsl.Binding.ServiceModel.Configuration.EndpointIdentityFactory.CreateCertificateIdentity(System.Security.Cryptography.X509Certificates.StoreLocation,System.Security.Cryptography.X509Certificates.StoreName,System.Security.Cryptography.X509Certificates.X509FindType,string,bool).storeName'></a>

`storeName` [System.Security.Cryptography.X509Certificates.StoreName](https://docs.microsoft.com/en-us/dotnet/api/System.Security.Cryptography.X509Certificates.StoreName 'System.Security.Cryptography.X509Certificates.StoreName')

<a name='Be.Stateless.BizTalk.Dsl.Binding.ServiceModel.Configuration.EndpointIdentityFactory.CreateCertificateIdentity(System.Security.Cryptography.X509Certificates.StoreLocation,System.Security.Cryptography.X509Certificates.StoreName,System.Security.Cryptography.X509Certificates.X509FindType,string,bool).findType'></a>

`findType` [System.Security.Cryptography.X509Certificates.X509FindType](https://docs.microsoft.com/en-us/dotnet/api/System.Security.Cryptography.X509Certificates.X509FindType 'System.Security.Cryptography.X509Certificates.X509FindType')

<a name='Be.Stateless.BizTalk.Dsl.Binding.ServiceModel.Configuration.EndpointIdentityFactory.CreateCertificateIdentity(System.Security.Cryptography.X509Certificates.StoreLocation,System.Security.Cryptography.X509Certificates.StoreName,System.Security.Cryptography.X509Certificates.X509FindType,string,bool).findValue'></a>

`findValue` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

<a name='Be.Stateless.BizTalk.Dsl.Binding.ServiceModel.Configuration.EndpointIdentityFactory.CreateCertificateIdentity(System.Security.Cryptography.X509Certificates.StoreLocation,System.Security.Cryptography.X509Certificates.StoreName,System.Security.Cryptography.X509Certificates.X509FindType,string,bool).isChainIncluded'></a>

`isChainIncluded` [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

#### Returns
[System.ServiceModel.Configuration.IdentityElement](https://docs.microsoft.com/en-us/dotnet/api/System.ServiceModel.Configuration.IdentityElement 'System.ServiceModel.Configuration.IdentityElement')