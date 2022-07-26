#### [Be.Stateless.Stream.Unit](README.md 'README')
### [Be.Stateless.Unit.IO](Be.Stateless.Unit.IO.md 'Be.Stateless.Unit.IO')

## TextStreamDummy Class

Text [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') whose content is dynamically generated up to a rounded-up size limit.

```csharp
public class TextStreamDummy : Be.Stateless.IO.EnumerableStream
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [System.MarshalByRefObject](https://docs.microsoft.com/en-us/dotnet/api/System.MarshalByRefObject 'System.MarshalByRefObject') &#129106; [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') &#129106; [Be.Stateless.IO.EnumerableStream](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.IO.EnumerableStream 'Be.Stateless.IO.EnumerableStream') &#129106; TextStreamDummy

### Remarks
The generated stream's text content, which is made of concatenated [System.Guid](https://docs.microsoft.com/en-us/dotnet/api/System.Guid 'System.Guid') string representations, may come
come in handy in compression-related scenarios (e.g. claim-check) due to the pseudo-random nature of [System.Guid](https://docs.microsoft.com/en-us/dotnet/api/System.Guid 'System.Guid')s
which exhibit a poor compression ratio.

| Properties | |
| :--- | :--- |
| [Length](TextStreamDummy.Length.md 'Be.Stateless.Unit.IO.TextStreamDummy.Length') | |

| Methods | |
| :--- | :--- |
| [Create(int)](TextStreamDummy.Create(int).md 'Be.Stateless.Unit.IO.TextStreamDummy.Create(int)') | |
