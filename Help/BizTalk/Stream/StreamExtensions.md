#### [Be.Stateless.BizTalk.Stream](README.md 'README')
### [Be.Stateless.BizTalk.Stream.Extensions](Be.Stateless.BizTalk.Stream.Extensions.md 'Be.Stateless.BizTalk.Stream.Extensions')

## StreamExtensions Class

Provides dependency injection support to [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') extension methods through various categories of
dedicated extension interfaces.

```csharp
public static class StreamExtensions
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; StreamExtensions

### Remarks
The purpose of this factory is to make [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') extension methods amenable to mocking, [http://blogs.clariusconsulting.net/kzu/how-to-mock-extension-methods/](http://blogs.clariusconsulting.net/kzu/how-to-mock-extension-methods/ 'http://blogs.clariusconsulting.net/kzu/how-to-mock-extension-methods/').

### See Also
- [http://blogs.clariusconsulting.net/kzu/how-extension-methods-ruined-unit-testing-and-oop-and-a-way-forward/](http://blogs.clariusconsulting.net/kzu/how-extension-methods-ruined-unit-testing-and-oop-and-a-way-forward/ 'http://blogs.clariusconsulting.net/kzu/how-extension-methods-ruined-unit-testing-and-oop-and-a-way-forward/')
- [http://blogs.clariusconsulting.net/kzu/making-extension-methods-amenable-to-mocking/](http://blogs.clariusconsulting.net/kzu/making-extension-methods-amenable-to-mocking/ 'http://blogs.clariusconsulting.net/kzu/making-extension-methods-amenable-to-mocking/')

| Methods | |
| :--- | :--- |
| [AsMarkable(this Stream)](StreamExtensions.AsMarkable(thisStream).md 'Be.Stateless.BizTalk.Stream.Extensions.StreamExtensions.AsMarkable(this System.IO.Stream)') | Ensure the [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') is wrapped in a [Microsoft.BizTalk.Streaming.MarkableForwardOnlyEventingReadStream](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Streaming.MarkableForwardOnlyEventingReadStream 'Microsoft.BizTalk.Streaming.MarkableForwardOnlyEventingReadStream') and thereby ready for probing, see [Probe(this Stream)](StreamExtensions.Probe(thisStream).md 'Be.Stateless.BizTalk.Stream.Extensions.StreamExtensions.Probe(this System.IO.Stream)'). |
| [EnsureMarkable(this Stream)](StreamExtensions.EnsureMarkable(thisStream).md 'Be.Stateless.BizTalk.Stream.Extensions.StreamExtensions.EnsureMarkable(this System.IO.Stream)') | Ensure the [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') is wrapped in a [Microsoft.BizTalk.Streaming.MarkableForwardOnlyEventingReadStream](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Streaming.MarkableForwardOnlyEventingReadStream 'Microsoft.BizTalk.Streaming.MarkableForwardOnlyEventingReadStream') and thereby ready for probing, see [Probe(this Stream)](StreamExtensions.Probe(thisStream).md 'Be.Stateless.BizTalk.Stream.Extensions.StreamExtensions.Probe(this System.IO.Stream)'). |
| [Probe(this Stream)](StreamExtensions.Probe(thisStream).md 'Be.Stateless.BizTalk.Stream.Extensions.StreamExtensions.Probe(this System.IO.Stream)') | Support for [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') probing. |
| [Transform(this Stream)](StreamExtensions.Transform(thisStream).md 'Be.Stateless.BizTalk.Stream.Extensions.StreamExtensions.Transform(this System.IO.Stream)') | Support for [Microsoft.XLANGs.BaseTypes.TransformBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.TransformBase 'Microsoft.XLANGs.BaseTypes.TransformBase')-derived transforms directly applied to one [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream'). |
| [Transform(this Stream[])](StreamExtensions.Transform(thisStream[]).md 'Be.Stateless.BizTalk.Stream.Extensions.StreamExtensions.Transform(this System.IO.Stream[])') | Support for [Microsoft.XLANGs.BaseTypes.TransformBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.TransformBase 'Microsoft.XLANGs.BaseTypes.TransformBase')-derived transforms directly applied to several [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')s. |
