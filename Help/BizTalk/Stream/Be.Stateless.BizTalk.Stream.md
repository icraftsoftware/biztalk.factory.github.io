#### [Be.Stateless.BizTalk.Stream](README.md 'README')

## Be.Stateless.BizTalk.Stream Namespace

| Classes | |
| :--- | :--- |
| [CompositeXmlStream](CompositeXmlStream.md 'Be.Stateless.BizTalk.Stream.CompositeXmlStream') | Aggregates, at the stream level, several [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream')s whose contents is XML. |
| [EventingReadStream](EventingReadStream.md 'Be.Stateless.BizTalk.Stream.EventingReadStream') | An eventing read-only stream replacement of [Microsoft.BizTalk.Streaming.EventingReadStream](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Streaming.EventingReadStream 'Microsoft.BizTalk.Streaming.EventingReadStream') that deterministically fires the [Microsoft.BizTalk.Streaming.IProvideReadStreamEvents.AfterLastReadEvent](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Streaming.IProvideReadStreamEvents.AfterLastReadEvent 'Microsoft.BizTalk.Streaming.IProvideReadStreamEvents.AfterLastReadEvent') event. |
| [MultipartFormDataContentStream](MultipartFormDataContentStream.md 'Be.Stateless.BizTalk.Stream.MultipartFormDataContentStream') | |
| [ReadOnlySeekableStream](ReadOnlySeekableStream.md 'Be.Stateless.BizTalk.Stream.ReadOnlySeekableStream') | This stream wraps an underlying stream into a read-only seekable stream. It does so by reusing BizTalk's [Microsoft.BizTalk.Streaming.ReadOnlySeekableStream](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Streaming.ReadOnlySeekableStream 'Microsoft.BizTalk.Streaming.ReadOnlySeekableStream') with a [Microsoft.BizTalk.Streaming.VirtualStream](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Streaming.VirtualStream 'Microsoft.BizTalk.Streaming.VirtualStream'). |
| [ReplicatingReadStream](ReplicatingReadStream.md 'Be.Stateless.BizTalk.Stream.ReplicatingReadStream') | A read-only [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') that replicates itself to another [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') while being read. |
| [XmlEnvelopeDecodingStream](XmlEnvelopeDecodingStream.md 'Be.Stateless.BizTalk.Stream.XmlEnvelopeDecodingStream') | |
| [XmlNamespaceTranslation](XmlNamespaceTranslation.md 'Be.Stateless.BizTalk.Stream.XmlNamespaceTranslation') | |
| [XmlTranslationRequirementsExtensions](XmlTranslationRequirementsExtensions.md 'Be.Stateless.BizTalk.Stream.XmlTranslationRequirementsExtensions') | |
| [XmlTranslationSet](XmlTranslationSet.md 'Be.Stateless.BizTalk.Stream.XmlTranslationSet') | |
| [XmlTranslationSetConverter](XmlTranslationSetConverter.md 'Be.Stateless.BizTalk.Stream.XmlTranslationSetConverter') | |
| [XmlTranslatorStream](XmlTranslatorStream.md 'Be.Stateless.BizTalk.Stream.XmlTranslatorStream') | |
| [ZipInputStream](ZipInputStream.md 'Be.Stateless.BizTalk.Stream.ZipInputStream') | Wraps a zip-decompressing stream around a data stream and ensures that the data stream is exhausted once the decompression is complete. It supports the PK Zip archive format with an entry compressed with the DEFLATE algorithm. |
| [ZipOutputStream](ZipOutputStream.md 'Be.Stateless.BizTalk.Stream.ZipOutputStream') | Wraps a zip-compressing stream around a data stream. |

| Enums | |
| :--- | :--- |
| [XmlTranslationRequirements](XmlTranslationRequirements.md 'Be.Stateless.BizTalk.Stream.XmlTranslationRequirements') | |
