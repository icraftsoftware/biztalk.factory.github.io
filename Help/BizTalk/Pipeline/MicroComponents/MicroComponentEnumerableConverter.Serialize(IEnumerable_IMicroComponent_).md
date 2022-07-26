#### [Be.Stateless.BizTalk.Pipeline.MicroComponents](README.md 'README')
### [Be.Stateless.BizTalk.MicroComponent](Be.Stateless.BizTalk.MicroComponent.md 'Be.Stateless.BizTalk.MicroComponent').[MicroComponentEnumerableConverter](MicroComponentEnumerableConverter.md 'Be.Stateless.BizTalk.MicroComponent.MicroComponentEnumerableConverter')

## MicroComponentEnumerableConverter.Serialize(IEnumerable<IMicroComponent>) Method

Serializes an [System.Collections.Generic.IEnumerable&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1') of [IMicroComponent](IMicroComponent.md 'Be.Stateless.BizTalk.MicroComponent.IMicroComponent')s to its XML [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')
representation.

```csharp
public static string Serialize(System.Collections.Generic.IEnumerable<Be.Stateless.BizTalk.MicroComponent.IMicroComponent> components);
```
#### Parameters

<a name='Be.Stateless.BizTalk.MicroComponent.MicroComponentEnumerableConverter.Serialize(System.Collections.Generic.IEnumerable_Be.Stateless.BizTalk.MicroComponent.IMicroComponent_).components'></a>

`components` [System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[IMicroComponent](IMicroComponent.md 'Be.Stateless.BizTalk.MicroComponent.IMicroComponent')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')

The [System.Collections.Generic.IEnumerable&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1') of [IMicroComponent](IMicroComponent.md 'Be.Stateless.BizTalk.MicroComponent.IMicroComponent')s to serialize.

#### Returns
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')  
A [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') that represents the [System.Collections.Generic.IEnumerable&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1') of [IMicroComponent](IMicroComponent.md 'Be.Stateless.BizTalk.MicroComponent.IMicroComponent')s.

### See Also
- [Deserialize(string)](MicroComponentEnumerableConverter.Deserialize(string).md 'Be.Stateless.BizTalk.MicroComponent.MicroComponentEnumerableConverter.Deserialize(string)')