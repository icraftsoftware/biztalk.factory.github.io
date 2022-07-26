#### [Be.Stateless.Stream](README.md 'README')
### [Be.Stateless.IO](Be.Stateless.IO.md 'Be.Stateless.IO').[EnumerableStream](EnumerableStream.md 'Be.Stateless.IO.EnumerableStream')

## EnumerableStream(IEnumerable<byte[]>) Constructor

Transform an [System.Collections.Generic.IEnumerable&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1') of arrays of [System.Byte](https://docs.microsoft.com/en-us/dotnet/api/System.Byte 'System.Byte')s into a [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream').

```csharp
public EnumerableStream(System.Collections.Generic.IEnumerable<byte[]> enumerable);
```
#### Parameters

<a name='Be.Stateless.IO.EnumerableStream.EnumerableStream(System.Collections.Generic.IEnumerable_byte[]_).enumerable'></a>

`enumerable` [System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[System.Byte](https://docs.microsoft.com/en-us/dotnet/api/System.Byte 'System.Byte')[[]](https://docs.microsoft.com/en-us/dotnet/api/System.Array 'System.Array')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')

The [System.Collections.Generic.IEnumerable&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1') over the arrays of [System.Byte](https://docs.microsoft.com/en-us/dotnet/api/System.Byte 'System.Byte')s.