#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk](Be.Stateless.BizTalk.md 'Be.Stateless.BizTalk')

## ClaimStoreSsoSettings Class

Single access point for all BizTalk Factory settings coming either from the BizTalkFactory Management Database or SSO
Database.

```csharp
public static class ClaimStoreSsoSettings
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; ClaimStoreSsoSettings

### Remarks
It's purpose is twofold: avoid the dissemination of magic stings all around, on one side, and support mocking and unit
testing, on the other side.

| Properties | |
| :--- | :--- |
| [ClaimStoreCheckInDirectory](ClaimStoreSsoSettings.ClaimStoreCheckInDirectory.md 'Be.Stateless.BizTalk.ClaimStoreSsoSettings.ClaimStoreCheckInDirectory') | |
| [ClaimStoreCheckOutDirectory](ClaimStoreSsoSettings.ClaimStoreCheckOutDirectory.md 'Be.Stateless.BizTalk.ClaimStoreSsoSettings.ClaimStoreCheckOutDirectory') | |
