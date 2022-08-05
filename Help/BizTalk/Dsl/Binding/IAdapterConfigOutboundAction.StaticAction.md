#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[IAdapterConfigOutboundAction](IAdapterConfigOutboundAction.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapterConfigOutboundAction')

## IAdapterConfigOutboundAction.StaticAction Property

Specify the SOAPAction header field for outgoing messages. This property can also be set through the message context
property [WCF.Action](https://docs.microsoft.com/en-us/dotnet/api/WCF.Action 'WCF.Action') in a pipeline or orchestration.

```csharp
string StaticAction { get; set; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Example
1. How to configure a static action corresponding to single constant SOAP action: — 
  
  ```csharp
  adapter.StaticAction = "http://services.stateless.be/biztalk/factory/mail/1.1/IMailService/SendMessage";
  ```
2. How to configure action mapping from operations to SOAP actions: — 
  
  ```csharp
  using Be.Stateless.BizTalk.Adapter.Metadata;
  
  ...
  
  adapter.StaticAction = new ActionMapping {
    new ActionMappingOperation(
      "UpdateIntervention",
      "http://Microsoft.LobServices.OracleDB/2007/03/TICKETING/Procedure/UPDATE_INTERVENTION"),
    new ActionMappingOperation(
      "UpdateOperation",
      "http://Microsoft.LobServices.OracleDB/2007/03/TICKETING/Procedure/UPDATE_OPERATION")
  };
  ```

### Remarks

You can specify this value in two different ways: the single action format and the action mapping format.

If you set this property in the single action format — for example,
http://contoso.com/svc/operation1—the SOAPAction header for outgoing messages is always set to the
value specified in this property.

If you set this property in the action mapping format, the outgoing SOAPAction header is determined by the [BTS.Operation](https://docs.microsoft.com/en-us/dotnet/api/BTS.Operation 'BTS.Operation') context property. For example, if this property is set to the following XML format and the
[BTS.Operation](https://docs.microsoft.com/en-us/dotnet/api/BTS.Operation 'BTS.Operation') property is set to `operation1`, the WCF send adapter uses
http://contoso.com/svc/operation1 for the outgoing SOAPAction header.

```csharp
<BtsActionMapping>
  <Operation Name="operation1" Action="http://contoso.com/svc/operation1"/>
  <Operation Name="operation2" Action="http://contoso.com/svc/operation2"/>
</BtsActionMapping>
```

If outgoing messages come from an orchestration port, orchestration instances dynamically set the BTS.Operation
property with the operation name of the port. If outgoing messages are routed with content-based routing, you can set
the [BTS.Operation](https://docs.microsoft.com/en-us/dotnet/api/BTS.Operation 'BTS.Operation') property in pipeline components.

It defaults to an [System.String.Empty](https://docs.microsoft.com/en-us/dotnet/api/System.String.Empty 'System.String.Empty') string.