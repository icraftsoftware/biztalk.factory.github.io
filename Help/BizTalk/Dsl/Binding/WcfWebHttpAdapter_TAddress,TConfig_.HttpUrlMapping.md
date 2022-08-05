#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfWebHttpAdapter&lt;TAddress,TConfig&gt;](WcfWebHttpAdapter_TAddress,TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter<TAddress,TConfig>')

## WcfWebHttpAdapter<TAddress,TConfig>.HttpUrlMapping Property

BTS Operation Mapping allows users to map incoming HTTP requests to BTS Operation in the message context, based on
the incoming HTTP Method and the URL sub-path.

```csharp
public string HttpUrlMapping { get; set; }
```

#### Property Value
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

### Remarks

The incoming HTTP Method and the URL sub-path are matched against a set of HTTP method and the URI Template. If a
match is found, the adapter promotes the [BTS.Operation](https://docs.microsoft.com/en-us/dotnet/api/BTS.Operation 'BTS.Operation') property to the BizTalk
Message Context with the value specified in the message.

You can specify HTTP method to URL mapping as a singular format or a multi-mapping format. The multi-mapping format
resembles the following: 

```csharp
<BtsHttpUrlMapping>
  <Operation Name = "DeleteCustomer" Method="DELETE" Url="/Customer/12345"/>
</BtsHttpUrlMapping>
```

In the above snippet, notice that the customer ID is provided as a constant value, which is 12345. However, there
could be scenarios when the customer ID, or any other query variable, must be determined at runtime. To enable such
scenarios, you must provide the variable component of the URL within curly brackets `{``}`. For example,
in the above snippet, if you specify the customer ID as a variable, it would look like: 

```csharp
<BtsHttpUrlMapping>
  <Operation Name = "DeleteCustomer" Method="DELETE" Url="/Customer/{ID}"/>
</BtsHttpUrlMapping>
```

In such a case, you must also specify where the value for the variable `ID` must be picked from at runtime. You
specify that using [VariableMapping](WcfWebHttpAdapter_TAddress,TConfig_.VariableMapping.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfWebHttpAdapter<TAddress,TConfig>.VariableMapping').

### See Also
- [Be.Stateless.BizTalk.Adapter.Metadata.HttpUrlMapping](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Adapter.Metadata.HttpUrlMapping 'Be.Stateless.BizTalk.Adapter.Metadata.HttpUrlMapping')
- [Be.Stateless.BizTalk.Adapter.Metadata.HttpUrlMappingOperation](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Adapter.Metadata.HttpUrlMappingOperation 'Be.Stateless.BizTalk.Adapter.Metadata.HttpUrlMappingOperation')