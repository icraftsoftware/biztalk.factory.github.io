#### [Be.Stateless.BizTalk.Transform.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.Xml](Be.Stateless.BizTalk.Unit.Xml.md 'Be.Stateless.BizTalk.Unit.Xml')

## ValuednessValidationCallback(object, ValuednessValidationCallbackArgs) Delegate

Represents the callback method that will handle XML valuedness validation events and the [ValuednessValidationCallbackArgs](ValuednessValidationCallbackArgs.md 'Be.Stateless.BizTalk.Unit.Xml.ValuednessValidationCallbackArgs').

```csharp
public delegate void ValuednessValidationCallback(object sender, Be.Stateless.BizTalk.Unit.Xml.ValuednessValidationCallbackArgs e);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Unit.Xml.ValuednessValidationCallback(object,Be.Stateless.BizTalk.Unit.Xml.ValuednessValidationCallbackArgs).sender'></a>

`sender` [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object')

The source of the event.

<a name='Be.Stateless.BizTalk.Unit.Xml.ValuednessValidationCallback(object,Be.Stateless.BizTalk.Unit.Xml.ValuednessValidationCallbackArgs).e'></a>

`e` [ValuednessValidationCallbackArgs](ValuednessValidationCallbackArgs.md 'Be.Stateless.BizTalk.Unit.Xml.ValuednessValidationCallbackArgs')

The event data.

### Remarks
Determine the type of a sender before using it in your code. You cannot assume that the sender is an instance of a
particular type. The sender is also not guaranteed to not be null. Always surround your casts with failure handling
logic.