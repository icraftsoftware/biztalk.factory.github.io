#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfSapAdapter](WcfSapAdapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter').[Inbound](WcfSapAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter.Inbound')

## WcfSapAdapter.Inbound.TidDatabaseConnectionString Property

Specifies the database connection string for the SQL Server database that the SAP adapter uses to store
Transaction Ids (TIDs) if the adapter should operate in TRFC server mode.

```csharp
public string TidDatabaseConnectionString { get; set; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks

You must set this property to enable inbound tRFC server calls for receiving IDocs or RFCs from SAP. The default
is `null`; tRFC server calls are not enabled.

You can specify the connection string in the following format:

```csharp
Data Source=<myServerAddress>;Initial Catalog=<myDataBase>;User Id=<myUsername>;Password=<myPassword>;
```

The BizTalk Adapter Pack setup wizard installs some SQL scripts that must be run by the SQL Server administrator
against an existing database to create the SQL Server objects that are used by the adapter to store TIDs to enable
inbound transactional RFC (tRFC) server calls. For more information about the SQL scripts, refer to the BizTalk
Adapter Pack installation guide available at `<installation drive>:\Program Files\Microsoft BizTalk
            Adapter Pack\Documents`.