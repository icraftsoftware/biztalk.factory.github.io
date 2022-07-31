#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfOracleAdapter&lt;TConfig&gt;](WcfOracleAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter<TConfig>')

## WcfOracleAdapter<TConfig>.UseSchemaInNameSpace Property

Specifies whether the schema name (SCOTT, HR, and so on) is included in the xml namespace for operations and their
associated types.

```csharp
public bool UseSchemaInNameSpace { get; set; }
```

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks

The advantage of not having scheme name included in the namespace is that if there is a table with same name (for
example, EMP) in two different schemas then the same XML can be used to perform the simple SQL operations (Insert,
Update, Delete, Select) on both tables.

For example, if the [UseSchemaInNameSpace](WcfOracleAdapter_TConfig_.UseSchemaInNameSpace.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter<TConfig>.UseSchemaInNameSpace') property is `True`, the namespace for these operations on
the SCOTT.EMP table is "`http://Microsoft.LobServices.OracleDB/2007/03/SCOTT/Table/EMP`"; if it is `False`,
the namespace is "`http://Microsoft.LobServices.OracleDB/2007/03/Table/EMP`".

The message action is not affected by the [UseSchemaInNameSpace](WcfOracleAdapter_TConfig_.UseSchemaInNameSpace.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter<TConfig>.UseSchemaInNameSpace') binding property; it always includes the
schema name.
            It is strongly recommended to set this binding property to `True` while generating metadata. If you set this
            property to `False`, the Oracle schema names (for example, SCOTT) will not be available in the XML namespace of
            the generated schema. So, if there are two tables with the same name in two different Oracle schemas, and they are
            added to the same BizTalk project, the BizTalk project will fail to build and deploy. If you want to include such
            schemas in the same BizTalk project, you must manually edit them to include the Oracle schema name in the XML
            namespace.
            

The default is True; the schema name is included in the namespace.