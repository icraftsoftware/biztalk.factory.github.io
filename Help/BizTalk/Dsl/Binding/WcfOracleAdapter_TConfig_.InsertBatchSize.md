#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfOracleAdapter&lt;TConfig&gt;](WcfOracleAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter<TConfig>')

## WcfOracleAdapter<TConfig>.InsertBatchSize Property

Specifies the batch size for multiple record Insert operations.

```csharp
public int InsertBatchSize { get; set; }
```

#### Property Value
[System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

### Remarks

The default is one. For values of [InsertBatchSize](WcfOracleAdapter_TConfig_.InsertBatchSize.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter<TConfig>.InsertBatchSize') greater than one, the Oracle Database adapter batches
the specified number of records into a single ODP.NET call. If the number of records in the Insert operation is not a
multiple of the batch size, the final batch will contain fewer records than the batch size value. For example, if the
insert message has 10 records and the [InsertBatchSize](WcfOracleAdapter_TConfig_.InsertBatchSize.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter<TConfig>.InsertBatchSize') is set to 1, the adapter reads individual records
and writes them into the Oracle database. So, the adapter performs 10 separate operations on the Oracle database.
Similarly, if the insert message has 10 records and the [InsertBatchSize](WcfOracleAdapter_TConfig_.InsertBatchSize.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter<TConfig>.InsertBatchSize') is set to 5, the adapter will
read and write 5 records at a time into the Oracle database, therefore performing only 2 insert operations.

If the structure of the records is not the same across a batch, a [Microsoft.ServiceModel.Channels.Common.XmlReaderParsingException](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.ServiceModel.Channels.Common.XmlReaderParsingException 'Microsoft.ServiceModel.Channels.Common.XmlReaderParsingException') exception
is thrown and the transaction is rolled back for the entire insert operation. A well-chosen value for [InsertBatchSize](WcfOracleAdapter_TConfig_.InsertBatchSize.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter<TConfig>.InsertBatchSize') can greatly improve adapter performance for multiple record Insert operations.