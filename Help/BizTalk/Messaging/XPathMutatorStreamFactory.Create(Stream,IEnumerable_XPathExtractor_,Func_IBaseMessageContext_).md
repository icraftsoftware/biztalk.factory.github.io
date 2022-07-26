#### [Be.Stateless.BizTalk.Messaging](README.md 'README')
### [Be.Stateless.BizTalk.Stream](Be.Stateless.BizTalk.Stream.md 'Be.Stateless.BizTalk.Stream').[XPathMutatorStreamFactory](XPathMutatorStreamFactory.md 'Be.Stateless.BizTalk.Stream.XPathMutatorStreamFactory')

## XPathMutatorStreamFactory.Create(Stream, IEnumerable<XPathExtractor>, Func<IBaseMessageContext>) Method

```csharp
public static Microsoft.BizTalk.Streaming.XPathMutatorStream Create(System.IO.Stream stream, System.Collections.Generic.IEnumerable<Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor> extractors, System.Func<Microsoft.BizTalk.Message.Interop.IBaseMessageContext> messageContextAccessor);
```
#### Parameters

<a name='Be.Stateless.BizTalk.Stream.XPathMutatorStreamFactory.Create(System.IO.Stream,System.Collections.Generic.IEnumerable_Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor_,System.Func_Microsoft.BizTalk.Message.Interop.IBaseMessageContext_).stream'></a>

`stream` [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')

<a name='Be.Stateless.BizTalk.Stream.XPathMutatorStreamFactory.Create(System.IO.Stream,System.Collections.Generic.IEnumerable_Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor_,System.Func_Microsoft.BizTalk.Message.Interop.IBaseMessageContext_).extractors'></a>

`extractors` [System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[XPathExtractor](XPathExtractor.md 'Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')

<a name='Be.Stateless.BizTalk.Stream.XPathMutatorStreamFactory.Create(System.IO.Stream,System.Collections.Generic.IEnumerable_Be.Stateless.BizTalk.Schema.Annotation.XPathExtractor_,System.Func_Microsoft.BizTalk.Message.Interop.IBaseMessageContext_).messageContextAccessor'></a>

`messageContextAccessor` [System.Func&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-1 'System.Func`1')[Microsoft.BizTalk.Message.Interop.IBaseMessageContext](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessageContext 'Microsoft.BizTalk.Message.Interop.IBaseMessageContext')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Func-1 'System.Func`1')

#### Returns
[Microsoft.BizTalk.Streaming.XPathMutatorStream](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Streaming.XPathMutatorStream 'Microsoft.BizTalk.Streaming.XPathMutatorStream')