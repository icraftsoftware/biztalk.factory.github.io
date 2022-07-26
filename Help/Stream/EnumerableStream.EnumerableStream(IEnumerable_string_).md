#### [Be.Stateless.Stream](README.md 'README')
### [Be.Stateless.IO](Be.Stateless.IO.md 'Be.Stateless.IO').[EnumerableStream](EnumerableStream.md 'Be.Stateless.IO.EnumerableStream')

## EnumerableStream(IEnumerable<string>) Constructor

Transform an [System.Collections.Generic.IEnumerable&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1') of [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')s into a [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream').

```csharp
public EnumerableStream(System.Collections.Generic.IEnumerable<string> enumerable);
```
#### Parameters

<a name='Be.Stateless.IO.EnumerableStream.EnumerableStream(System.Collections.Generic.IEnumerable_string_).enumerable'></a>

`enumerable` [System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')

The [System.Collections.Generic.IEnumerable&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1') over the [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')s.

### Remarks
The [System.Text.Encoding.Unicode](https://docs.microsoft.com/en-us/dotnet/api/System.Text.Encoding.Unicode 'System.Text.Encoding.Unicode') encoding will be assumed to transform the [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')s into their
[System.Byte](https://docs.microsoft.com/en-us/dotnet/api/System.Byte 'System.Byte') equivalent.