#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Adapter](Be.Stateless.BizTalk.Dsl.Binding.Adapter.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter').[WcfOracleAdapter&lt;TConfig&gt;](WcfOracleAdapter_TConfig_.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter<TConfig>')

## WcfOracleAdapter<TConfig>.SkipNilNodes Property

Specifies whether the Oracle Database adapter will skip inserting or updating values for nodes that are marked as
'nil' in the request XML.

```csharp
public bool SkipNilNodes { get; set; }
```

#### Property Value
[System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean')

### Remarks

This property is applicable for inserting or updating records in a table and for RECORD type parameters in stored
procedures. Default is `True`, which means the adapter will skip passing values for nodes that are marked as
'nil'. In this case, the default value in Oracle (if specified) is taken into account for nodes that are marked as
'nil'. If set to `False`, the adapter explicitly passes a null value for these nodes.

Notice that:
- For nodes that are not present in the request XML, the adapter always skips passing values, irrespective of the value
  of the [SkipNilNodes](WcfOracleAdapter_TConfig_.SkipNilNodes.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter<TConfig>.SkipNilNodes') property.
- For PL/SQL tables of RECORDS, the adapter always passes a null value for nodes that are either marked as 'nil' or not
  present in the request XML, irrespective of the value of the [SkipNilNodes](WcfOracleAdapter_TConfig_.SkipNilNodes.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter<TConfig>.SkipNilNodes') property.
The following example explains the difference in the adapter configuration based on the value you set for this
property. Assume an XML request as follows: 

```csharp
<EMPNO>1000</EMPNO>
<ENAME>John</ENAME>
<SAL nil='true'></SAL>
``` If [SkipNilNodes](WcfOracleAdapter_TConfig_.SkipNilNodes.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter<TConfig>.SkipNilNodes') is set to `True`, the adapter executes the following command:

```csharp
INSERT INTO EMP (EMPNO, ENAME) VALUES (1000, 'John');
```

If [SkipNilNodes](WcfOracleAdapter_TConfig_.SkipNilNodes.md 'Be.Stateless.BizTalk.Dsl.Binding.Adapter.WcfOracleAdapter<TConfig>.SkipNilNodes') is set to `False`, the adapter executes the following command:

```csharp
INSERT INTO EMP (EMPNO, ENAME, SAL) VALUES (1000, 'John', null);
```
Note that in the second statement, the adapter explicitly inserts a null value for the parameter 'SAL'.