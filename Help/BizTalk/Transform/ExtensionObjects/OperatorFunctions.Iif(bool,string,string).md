#### [Be.Stateless.BizTalk.Transform.ExtensionObjects](README.md 'README')
### [Be.Stateless.BizTalk.Transform.ExtensionObjects](Be.Stateless.BizTalk.Transform.ExtensionObjects.md 'Be.Stateless.BizTalk.Transform.ExtensionObjects').[OperatorFunctions](OperatorFunctions.md 'Be.Stateless.BizTalk.Transform.ExtensionObjects.OperatorFunctions')

## OperatorFunctions.Iif(bool, string, string) Method

Returns one of two values depending on the value of a Boolean [condition](OperatorFunctions.Iif(bool,string,string).md#Be.Stateless.BizTalk.Transform.ExtensionObjects.OperatorFunctions.Iif(bool,string,string).condition 'Be.Stateless.BizTalk.Transform.ExtensionObjects.OperatorFunctions.Iif(bool, string, string).condition').

```csharp
public string Iif(bool condition, string then, string @else);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Transform.ExtensionObjects.OperatorFunctions.Iif(bool,string,string).condition'></a>

`condition` [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

The Boolean expression to evaluate as the condition.

<a name='Be.Stateless.BizTalk.Transform.ExtensionObjects.OperatorFunctions.Iif(bool,string,string).then'></a>

`then` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The value to be returned if [condition](OperatorFunctions.Iif(bool,string,string).md#Be.Stateless.BizTalk.Transform.ExtensionObjects.OperatorFunctions.Iif(bool,string,string).condition 'Be.Stateless.BizTalk.Transform.ExtensionObjects.OperatorFunctions.Iif(bool, string, string).condition') evaluates to `true`.

<a name='Be.Stateless.BizTalk.Transform.ExtensionObjects.OperatorFunctions.Iif(bool,string,string).else'></a>

`else` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

The value to be returned if [condition](OperatorFunctions.Iif(bool,string,string).md#Be.Stateless.BizTalk.Transform.ExtensionObjects.OperatorFunctions.Iif(bool,string,string).condition 'Be.Stateless.BizTalk.Transform.ExtensionObjects.OperatorFunctions.Iif(bool, string, string).condition') evaluates to `false`.

#### Returns
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')  
Either [then](OperatorFunctions.Iif(bool,string,string).md#Be.Stateless.BizTalk.Transform.ExtensionObjects.OperatorFunctions.Iif(bool,string,string).then 'Be.Stateless.BizTalk.Transform.ExtensionObjects.OperatorFunctions.Iif(bool, string, string).then') or [else](OperatorFunctions.Iif(bool,string,string).md#Be.Stateless.BizTalk.Transform.ExtensionObjects.OperatorFunctions.Iif(bool,string,string).else 'Be.Stateless.BizTalk.Transform.ExtensionObjects.OperatorFunctions.Iif(bool, string, string).else') value depending on the Boolean value of [condition](OperatorFunctions.Iif(bool,string,string).md#Be.Stateless.BizTalk.Transform.ExtensionObjects.OperatorFunctions.Iif(bool,string,string).condition 'Be.Stateless.BizTalk.Transform.ExtensionObjects.OperatorFunctions.Iif(bool, string, string).condition').