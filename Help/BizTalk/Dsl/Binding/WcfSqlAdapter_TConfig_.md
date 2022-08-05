#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter')

## WcfSqlAdapter<TConfig> Class

```csharp
public abstract class WcfSqlAdapter<TConfig> : Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfLobAdapterBase<Microsoft.Adapters.Sql.SqlAdapterConnectionUri, Microsoft.Adapters.Sql.SqlAdapterBindingConfigurationElement, TConfig>,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigBizTalkCompatibilityMode,
Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigPerformanceCounters
    where TConfig : Microsoft.BizTalk.Adapter.Wcf.Config.AdapterConfig, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigAddress, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigIdentity, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigBinding, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigEndpointBehavior, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigInboundMessageMarshalling, Microsoft.BizTalk.Adapter.Wcf.Config.IAdapterConfigOutboundMessageMarshalling, new()
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter_TConfig_.TConfig'></a>

`TConfig`

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [AdapterBase](AdapterBase.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.AdapterBase') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase&lt;](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[Microsoft.Adapters.Sql.SqlAdapterConnectionUri](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.Adapters.Sql.SqlAdapterConnectionUri 'Microsoft.Adapters.Sql.SqlAdapterConnectionUri')[,](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[Microsoft.Adapters.Sql.SqlAdapterBindingConfigurationElement](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.Adapters.Sql.SqlAdapterBindingConfigurationElement 'Microsoft.Adapters.Sql.SqlAdapterBindingConfigurationElement')[,](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>')[TConfig](WcfSqlAdapter_TConfig_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter_TConfig_.TConfig 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter<TConfig>.TConfig')[&gt;](WcfAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfAdapterBase<TAddress,TBinding,TConfig>') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase&lt;](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>')[Microsoft.Adapters.Sql.SqlAdapterConnectionUri](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.Adapters.Sql.SqlAdapterConnectionUri 'Microsoft.Adapters.Sql.SqlAdapterConnectionUri')[,](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>')[Microsoft.Adapters.Sql.SqlAdapterBindingConfigurationElement](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.Adapters.Sql.SqlAdapterBindingConfigurationElement 'Microsoft.Adapters.Sql.SqlAdapterBindingConfigurationElement')[,](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>')[TConfig](WcfSqlAdapter_TConfig_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter_TConfig_.TConfig 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter<TConfig>.TConfig')[&gt;](WcfBindingCentricAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfBindingCentricAdapterBase<TAddress,TBinding,TConfig>') &#129106; [Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfLobAdapterBase&lt;](WcfLobAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfLobAdapterBase<TAddress,TBinding,TConfig>')[Microsoft.Adapters.Sql.SqlAdapterConnectionUri](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.Adapters.Sql.SqlAdapterConnectionUri 'Microsoft.Adapters.Sql.SqlAdapterConnectionUri')[,](WcfLobAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfLobAdapterBase<TAddress,TBinding,TConfig>')[Microsoft.Adapters.Sql.SqlAdapterBindingConfigurationElement](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.Adapters.Sql.SqlAdapterBindingConfigurationElement 'Microsoft.Adapters.Sql.SqlAdapterBindingConfigurationElement')[,](WcfLobAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfLobAdapterBase<TAddress,TBinding,TConfig>')[TConfig](WcfSqlAdapter_TConfig_.md#Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter_TConfig_.TConfig 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter<TConfig>.TConfig')[&gt;](WcfLobAdapterBase_TAddress,TBinding,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfLobAdapterBase<TAddress,TBinding,TConfig>') &#129106; WcfSqlAdapter<TConfig>

Derived  
&#8627; [Inbound](WcfSqlAdapter.Inbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter.Inbound')  
&#8627; [Outbound](WcfSqlAdapter.Outbound.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter.Outbound')

Implements [IAdapterConfigBizTalkCompatibilityMode](IAdapterConfigBizTalkCompatibilityMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigBizTalkCompatibilityMode'), [IAdapterConfigPerformanceCounters](IAdapterConfigPerformanceCounters.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigPerformanceCounters')

| Properties | |
| :--- | :--- |
| [EnableBizTalkCompatibilityMode](WcfSqlAdapter_TConfig_.EnableBizTalkCompatibilityMode.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter<TConfig>.EnableBizTalkCompatibilityMode') | |
| [EnablePerformanceCounters](WcfSqlAdapter_TConfig_.EnablePerformanceCounters.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter<TConfig>.EnablePerformanceCounters') | |
| [Encrypt](WcfSqlAdapter_TConfig_.Encrypt.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter<TConfig>.Encrypt') | Determines whether SQL Server uses SSL encryption for all data sent between the client and server if the server has a certificate installed. |
| [MaxConnectionPoolSize](WcfSqlAdapter_TConfig_.MaxConnectionPoolSize.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter<TConfig>.MaxConnectionPoolSize') | The maximum number of connections allowed in the connection pool for a particular connection URI. |
| [UseAmbientTransaction](WcfSqlAdapter_TConfig_.UseAmbientTransaction.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter<TConfig>.UseAmbientTransaction') | Determines whether the adapter performs the operations on the SQL Server within the context of the ambient transaction. In BizTalk Server, the same transaction is used to publish/delete messages from the MessageBox. |
| [UseDatabaseNameInXsdNamespace](WcfSqlAdapter_TConfig_.UseDatabaseNameInXsdNamespace.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter<TConfig>.UseDatabaseNameInXsdNamespace') | Determines whether the database name should be used in the XSD namespaces. |
| [WorkstationId](WcfSqlAdapter_TConfig_.WorkstationId.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter<TConfig>.WorkstationId') | Gets or sets the value for WorkstationId which is the name of the workstation connecting to SQL Server. |
| [XmlStoredProcedureRootNodeName](WcfSqlAdapter_TConfig_.XmlStoredProcedureRootNodeName.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter<TConfig>.XmlStoredProcedureRootNodeName') | Gets or sets the name of the root node which will be used for executing FOR XML stored procedures. |
| [XmlStoredProcedureRootNodeNamespace](WcfSqlAdapter_TConfig_.XmlStoredProcedureRootNodeNamespace.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSqlAdapter<TConfig>.XmlStoredProcedureRootNodeNamespace') | Gets or sets the namespace of the root node which will be used for executing FOR XML stored procedures. |