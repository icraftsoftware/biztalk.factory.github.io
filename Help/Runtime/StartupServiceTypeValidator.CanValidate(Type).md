#### [Be.Stateless.Runtime](README.md 'README')
### [Be.Stateless.Runtime.Configuration.Validators](Be.Stateless.Runtime.Configuration.Validators.md 'Be.Stateless.Runtime.Configuration.Validators').[StartupServiceTypeValidator](StartupServiceTypeValidator.md 'Be.Stateless.Runtime.Configuration.Validators.StartupServiceTypeValidator')

## StartupServiceTypeValidator.CanValidate(Type) Method

Determines whether the type of the object can be validated.

```csharp
public override bool CanValidate(System.Type type);
```
#### Parameters

<a name='Be.Stateless.Runtime.Configuration.Validators.StartupServiceTypeValidator.CanValidate(System.Type).type'></a>

`type` [System.Type](https://docs.microsoft.com/en-us/dotnet/api/System.Type 'System.Type')

The type of object.

#### Returns
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')  
`true` if the [type](StartupServiceTypeValidator.CanValidate(Type).md#Be.Stateless.Runtime.Configuration.Validators.StartupServiceTypeValidator.CanValidate(System.Type).type 'Be.Stateless.Runtime.Configuration.Validators.StartupServiceTypeValidator.CanValidate(System.Type).type') parameter is a [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String'); otherwise, `false`.