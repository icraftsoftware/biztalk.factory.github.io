#### [Be.Stateless.BizTalk.Pipeline.MicroComponents](README.md 'README')
### [Be.Stateless.BizTalk.MicroComponent](Be.Stateless.BizTalk.MicroComponent.md 'Be.Stateless.BizTalk.MicroComponent').[MicroComponentEnumerableConverter](MicroComponentEnumerableConverter.md 'Be.Stateless.BizTalk.MicroComponent.MicroComponentEnumerableConverter')

## MicroComponentEnumerableConverter.Deserialize(string) Method

Deserializes an [System.Collections.Generic.IEnumerable&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1') of [IMicroComponent](IMicroComponent.md 'Be.Stateless.BizTalk.MicroComponent.IMicroComponent')s from its XML serialization [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String').

```csharp
public static System.Collections.Generic.IEnumerable<Be.Stateless.BizTalk.MicroComponent.IMicroComponent> Deserialize(string xml);
```
#### Parameters

<a name='Be.Stateless.BizTalk.MicroComponent.MicroComponentEnumerableConverter.Deserialize(string).xml'></a>

`xml` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')

A [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') denoting the XML serialization of an [System.Collections.Generic.IEnumerable&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1') of [IMicroComponent](IMicroComponent.md 'Be.Stateless.BizTalk.MicroComponent.IMicroComponent')s.

#### Returns
[System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[IMicroComponent](IMicroComponent.md 'Be.Stateless.BizTalk.MicroComponent.IMicroComponent')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')  
The deserialized [System.Collections.Generic.IEnumerable&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1') of [IMicroComponent](IMicroComponent.md 'Be.Stateless.BizTalk.MicroComponent.IMicroComponent')s.

### See Also
- [Serialize(IEnumerable&lt;IMicroComponent&gt;)](MicroComponentEnumerableConverter.Serialize(IEnumerable_IMicroComponent_).md 'Be.Stateless.BizTalk.MicroComponent.MicroComponentEnumerableConverter.Serialize(System.Collections.Generic.IEnumerable<Be.Stateless.BizTalk.MicroComponent.IMicroComponent>)')