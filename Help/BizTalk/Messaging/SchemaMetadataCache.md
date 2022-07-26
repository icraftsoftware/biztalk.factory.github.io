#### [Be.Stateless.BizTalk.Messaging](README.md 'README')
### [Be.Stateless.BizTalk.Runtime.Caching](Be.Stateless.BizTalk.Runtime.Caching.md 'Be.Stateless.BizTalk.Runtime.Caching')

## SchemaMetadataCache Class

Runtime memory cache for the [ISchemaMetadata](ISchemaMetadata.md 'Be.Stateless.BizTalk.Schema.ISchemaMetadata') associated to [Microsoft.XLANGs.BaseTypes.SchemaBase](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.XLANGs.BaseTypes.SchemaBase 'Microsoft.XLANGs.BaseTypes.SchemaBase')-derived types.

```csharp
public class SchemaMetadataCache : Be.Stateless.Runtime.Caching.SlidingCache<System.Type, Be.Stateless.BizTalk.Schema.ISchemaMetadata>
```

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [Be.Stateless.Runtime.Caching.Cache&lt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.Runtime.Caching.Cache-2 'Be.Stateless.Runtime.Caching.Cache`2')[System.Type](https://docs.microsoft.com/en-us/dotnet/api/System.Type 'System.Type')[,](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.Runtime.Caching.Cache-2 'Be.Stateless.Runtime.Caching.Cache`2')[ISchemaMetadata](ISchemaMetadata.md 'Be.Stateless.BizTalk.Schema.ISchemaMetadata')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.Runtime.Caching.Cache-2 'Be.Stateless.Runtime.Caching.Cache`2') &#129106; [Be.Stateless.Runtime.Caching.SlidingCache&lt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.Runtime.Caching.SlidingCache-2 'Be.Stateless.Runtime.Caching.SlidingCache`2')[System.Type](https://docs.microsoft.com/en-us/dotnet/api/System.Type 'System.Type')[,](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.Runtime.Caching.SlidingCache-2 'Be.Stateless.Runtime.Caching.SlidingCache`2')[ISchemaMetadata](ISchemaMetadata.md 'Be.Stateless.BizTalk.Schema.ISchemaMetadata')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.Runtime.Caching.SlidingCache-2 'Be.Stateless.Runtime.Caching.SlidingCache`2') &#129106; SchemaMetadataCache

### See Also
- [Be.Stateless.Runtime.Caching.Cache&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.Runtime.Caching.Cache-2 'Be.Stateless.Runtime.Caching.Cache`2')
- [Be.Stateless.Runtime.Caching.SlidingCache&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.Runtime.Caching.SlidingCache-2 'Be.Stateless.Runtime.Caching.SlidingCache`2')

| Properties | |
| :--- | :--- |
| [Instance](SchemaMetadataCache.Instance.md 'Be.Stateless.BizTalk.Runtime.Caching.SchemaMetadataCache.Instance') | Singleton [SchemaMetadataCache](SchemaMetadataCache.md 'Be.Stateless.BizTalk.Runtime.Caching.SchemaMetadataCache') instance. |
