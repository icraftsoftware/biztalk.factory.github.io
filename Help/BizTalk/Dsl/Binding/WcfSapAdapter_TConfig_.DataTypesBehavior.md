#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfSapAdapter&lt;TConfig&gt;](WcfSapAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfSapAdapter<TConfig>')

## WcfSapAdapter<TConfig>.DataTypesBehavior Property


The SAP system does not enforce correct values to be specified for DATS, TIMS, and NUMC fields. So, if invalid values
are present in the SAP data store for DATS, TIMS, and NUMC fields and a client program tries to read the values using
the SAP adapter, the adapter throws an exception.

Also, the SAP system has special values for representing minimum and maximum values for the DATS, TIMS, and NUMC
fields for which there is no equivalent .NET type. For example, the minimum and maximum values for a DATS field are
00000000 and 99999999 respectively, for which there is no equivalent .NET type [System.DateTime](https://docs.microsoft.com/en-us/dotnet/api/System.DateTime 'System.DateTime'). Moreover,
converting the minimum and maximum values for DATS fields to [DateTime.MinValue](https://docs.microsoft.com/en-us/dotnet/api/System.DateTime.MinValue 'System.DateTime.MinValue')
and [DateTime.MaxValue](https://docs.microsoft.com/en-us/dotnet/api/System.DateTime.MaxValue 'System.DateTime.MaxValue') is not feasible because the minimum or maximum value for
DATS field and minimum or maximum value for a .NET [System.DateTime](https://docs.microsoft.com/en-us/dotnet/api/System.DateTime 'System.DateTime') type are not the same.

```csharp
public Microsoft.Adapters.SAP.SapDataTypesBehavior DataTypesBehavior { get; set; }
```

#### Property Value
[Microsoft.Adapters.SAP.SapDataTypesBehavior](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.Adapters.SAP.SapDataTypesBehavior 'Microsoft.Adapters.SAP.SapDataTypesBehavior')

### Remarks
To enable adapter clients to control the adapter behavior when special values are encountered in the SAP system, you
can set the DataTypesBehavior binding property. This is a complex binding property that has the following
sub-properties:

|[Microsoft.Adapters.SAP.SapDataTypesBehavior](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.Adapters.SAP.SapDataTypesBehavior 'Microsoft.Adapters.SAP.SapDataTypesBehavior')|
|-|
|Specifies the behavior the adapter should follow to send a DATS value when the adapter client sends the value [DateTime.MaxValue](https://docs.microsoft.com/en-us/dotnet/api/System.DateTime.MaxValue 'System.DateTime.MaxValue'), which is "9999-12-31T23:59:59.9999999". You could set this to the following values:  Default is 99991231.|
|Specifies the behavior the adapter should follow to send a TIMS value when the adapter client sends the value [DateTime.MaxValue](https://docs.microsoft.com/en-us/dotnet/api/System.DateTime.MaxValue 'System.DateTime.MaxValue'), which is "9999-12-31T23:59:59.9999999". You could set this to the following values:  Default is 235959.|
|Specifies the behavior the adapter should follow to send a DATS value when the adapter client sends the value [DateTime.MinValue](https://docs.microsoft.com/en-us/dotnet/api/System.DateTime.MinValue 'System.DateTime.MinValue'), which is "0001-01-01T00:00:00". You could set this to the following values:  Default is 00010101.|
|Specifies the behavior the adapter should follow to send a TIMS value when the adapter client sends the value [DateTime.MinValue](https://docs.microsoft.com/en-us/dotnet/api/System.DateTime.MinValue 'System.DateTime.MinValue'), which is "0001-01-01T00:00:00". You could set this to the following values:  Default is 000000.|
|Specifies the behavior the adapter should follow to send a DATS value when the adapter client sends a NULL DateTime value. You could set this to the following values:  Default is "SKIP".|
|             Default is "SKIP".|
|Specifies the behavior the adapter should follow to retrieve a DateTime value when the adapter receives a DATS.MAX value, which is 99999999, from SAP. You could set this to the following values:  Default is "ERROR".|
|Specifies the behavior the adapter should follow to retrieve a DateTime value when the adapter receives a DATS.MIN value, which is 00000000, from SAP. You could set this to the following values:  Default is "ERROR".|
|Specifies the behavior the adapter should follow to retrieve a DateTime value when the adapter receives an empty DATS value from SAP. You could set this to the following values:  Default is 0001-01-01T00:00:00.|
|Specifies the behavior the adapter should follow to retrieve an integer value when the adapter receives an empty NUMC value (all spaces) from SAP. You could set this to the following values:  Default is 0.|
|Specifies the behavior the adapter should follow to retrieve a DateTime value when the adapter receives an empty TIMS value from SAP. You could set this to the following values:  Default is 0001-01-01T00:00:00.|
|Specifies the behavior the adapter should follow to retrieve a DateTime value when the adapter receives an invalid DATS value from SAP. You could set this to the following values:  Default is "ERROR".|
|Specifies the behavior the adapter should follow to retrieve an integer value when the adapter receives an invalid NUMC value from SAP. You could set this to the following values:  Default is 0.|
|Specifies the behavior the adapter should follow to retrieve a DateTime value when the adapter receives a TIMS.MAX value from SAP. You could set this to the following values:  Default is "ERROR".|