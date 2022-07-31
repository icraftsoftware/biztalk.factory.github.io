#### [Be.Stateless.BizTalk.Activity.Monitoring](README.md 'README')
### [Be.Stateless.BizTalk.Extensions](Be.Stateless.BizTalk.Extensions.md 'Be.Stateless.BizTalk.Extensions').[StringExtensions](StringExtensions.md 'Be.Stateless.BizTalk.Extensions.StringExtensions')

## StringExtensions.ToFriendlyProcessName(this string) Method

Returns a process friendly, or short, name made from the concatenation of the Project/Area/Process tokens in a
comprehensive process name.

```csharp
public static string ToFriendlyProcessName(this string processName);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Extensions.StringExtensions.ToFriendlyProcessName(thisstring).processName'></a>

`processName` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The comprehensive process name.

#### Returns
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')  
The concatenated Project/Area/Process tokens.

### Example
Given the following comprehensive process names
- `Be.Stateless.BizTalk.Factory.Areas.Default.Failed`
- `Be.Stateless.BizTalk.Factory.Areas.Default.Unidentified`
- `Be.Stateless.BizTalk.Factory.Areas.Batch.Aggregate`
- `Be.Stateless.BizTalk.Factory.Areas.Batch.Release`
- `Be.Stateless.BizTalk.Factory.Areas.Claim.Check`
- `Be.Stateless.Accounting.Orchestrations.Invoicing.UpdateLedger`
- `Be.Stateless.Accounting.Orchestrations.UpdateMasterData`
the friendly names are respectively
- `Factory/Failed` where
- `Factory/Unidentified` where
- `Factory/Batch/Aggregate` where
- `Factory/Batch/Release` where
- `Factory/Claim/Check` where
- `Accounting/Invoicing/UpdateLedger` where
- `Accounting/UpdateMasterData` where

### Remarks
Tokens are isolated via a regular expression. Any Area named `Default` is skipped or equivalent to a
`null`, non-existing, area.