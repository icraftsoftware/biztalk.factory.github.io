#### [Be.Stateless.BizTalk.Activity.Tracking](README.md 'README')
### [Be.Stateless.BizTalk.Factory.Areas](Be.Stateless.BizTalk.Factory.Areas.md 'Be.Stateless.BizTalk.Factory.Areas')

## Claim Class

BizTalk Factory's process names.

```csharp
public class Claim : Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessName<Be.Stateless.BizTalk.Factory.Areas.Claim>
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessName&lt;](ProcessName_T_.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessName<T>')[Claim](Claim.md 'Be.Stateless.BizTalk.Factory.Areas.Claim')[&gt;](ProcessName_T_.md 'Be.Stateless.BizTalk.Activity.Tracking.Messaging.ProcessName<T>') &#129106; Claim

### Remarks

By convention, the token that precedes the 'Areas' or the 'Orchestrations' token of the CLR namespace 
denotes the LOB/project to which a process belongs. The area is represented by the token that follows 
'Areas' or 'Orchestrations', and the process name itself is the next token.
For instance `Be.Stateless.ECommerce.Areas.Shopping.CustomerRegistration`,
`Be.Stateless.ECommerce.Areas.Shopping.Invoicing`, and `Be.Stateless.ECommerce.Areas.Shopping.Shipping`
cover 3 different business processes (`CustomerRegistration`, `Invoicing`, and `Shipping`) 
in the `Shopping` area if the `ECommerce` LOB/project.
<seealso cref="T:Be.Stateless.BizTalk.Factory.Areas.Default"/>

These tokens are of importance for the monitoring web site accompanying BizTalk Factory.

| Properties | |
| :--- | :--- |
| [Check](Claim.Check.md 'Be.Stateless.BizTalk.Factory.Areas.Claim.Check') | Name of the claim check messaging-only process/flow. |
