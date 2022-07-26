#### [Be.Stateless.BizTalk.Pipeline.MicroComponents](README.md 'README')

## Be.Stateless.BizTalk.MicroComponent Namespace

| Classes | |
| :--- | :--- |
| [ContextBuilder](ContextBuilder.md 'Be.Stateless.BizTalk.MicroComponent.ContextBuilder') | Delegates building of message context to a [IContextBuilder](IContextBuilder.md 'Be.Stateless.BizTalk.MicroComponent.IContextBuilder') component plugin. |
| [ContextPropertyExtractor](ContextPropertyExtractor.md 'Be.Stateless.BizTalk.MicroComponent.ContextPropertyExtractor') | This component allows to manipulate the message context by either clearing, demoting, writing or promoting property values. These values can either be constant or extracted out of an XML message by defining XPath expressions. Notice that these XPath expressions are less restrictive than the traditional canonical XPath expressions supported by BizTalk Server; limitations are however still present and relatively strong. |
| [DirectoryCreator](DirectoryCreator.md 'Be.Stateless.BizTalk.MicroComponent.DirectoryCreator') | |
| [FailedMessageRoutingEnabler](FailedMessageRoutingEnabler.md 'Be.Stateless.BizTalk.MicroComponent.FailedMessageRoutingEnabler') | Enables routing of failed messages and prevents routing failure reports from being generated. |
| [MessageBodyStreamFactory](MessageBodyStreamFactory.md 'Be.Stateless.BizTalk.MicroComponent.MessageBodyStreamFactory') | Micro component that replaces the [System.IO.Stream](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Stream 'System.IO.Stream') of the current message's [Microsoft.BizTalk.Message.Interop.IBaseMessage.BodyPart](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Message.Interop.IBaseMessage.BodyPart 'Microsoft.BizTalk.Message.Interop.IBaseMessage.BodyPart') by a new one whose creation is delegated to either a contextual or statically configurable [IMessageBodyStreamFactory](IMessageBodyStreamFactory.md 'Be.Stateless.BizTalk.MicroComponent.IMessageBodyStreamFactory') plugin. |
| [MessageConsumer](MessageConsumer.md 'Be.Stateless.BizTalk.MicroComponent.MessageConsumer') | Drain and consume the pipeline message. |
| [MessageTypeExtractor](MessageTypeExtractor.md 'Be.Stateless.BizTalk.MicroComponent.MessageTypeExtractor') | Probe the current message for its type and write it in the [BizTalkFactoryProperties.MessageType](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.BizTalkFactoryProperties.MessageType 'Be.Stateless.BizTalk.ContextProperties.BizTalkFactoryProperties.MessageType') context property. |
| [MicroComponentEnumerableConverter](MicroComponentEnumerableConverter.md 'Be.Stateless.BizTalk.MicroComponent.MicroComponentEnumerableConverter') | Converts an [System.Collections.Generic.IEnumerable&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1') of [IMicroComponent](IMicroComponent.md 'Be.Stateless.BizTalk.MicroComponent.IMicroComponent')s back and forth to an XML [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String'). |
| [MicroComponentXmlWriter](MicroComponentXmlWriter.md 'Be.Stateless.BizTalk.MicroComponent.MicroComponentXmlWriter') | |
| [MicroPipeline](MicroPipeline.md 'Be.Stateless.BizTalk.MicroComponent.MicroPipeline') | Runs a sequence of micro components, i.e. components implementing [IMicroComponent](IMicroComponent.md 'Be.Stateless.BizTalk.MicroComponent.IMicroComponent'), similarly to what a regular Microsoft BizTalk Server pipeline would do if the micro components were regular pipeline components. |
| [MultipartFormDataContentEncoder](MultipartFormDataContentEncoder.md 'Be.Stateless.BizTalk.MicroComponent.MultipartFormDataContentEncoder') | Wraps the original message stream by a [Be.Stateless.BizTalk.Stream.MultipartFormDataContentStream](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Stream.MultipartFormDataContentStream 'Be.Stateless.BizTalk.Stream.MultipartFormDataContentStream'). |
| [SBMessagingContextPropagator](SBMessagingContextPropagator.md 'Be.Stateless.BizTalk.MicroComponent.SBMessagingContextPropagator') | Propagates message type and correlation id over inbound and outbound Azure ServiceBus queues. |
| [TransportRetriesDisabler](TransportRetriesDisabler.md 'Be.Stateless.BizTalk.MicroComponent.TransportRetriesDisabler') | Prevent Microsoft BizTalk Server's SendPort Transport from performing any retries to send the message in case of failures provided the property [Be.Stateless.BizTalk.ContextProperties.BizTalkFactoryProperties.DisableTransportRetries](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.ContextProperties.BizTalkFactoryProperties.DisableTransportRetries 'Be.Stateless.BizTalk.ContextProperties.BizTalkFactoryProperties.DisableTransportRetries') is present in the message's context and has a value of `true`. |
| [XmlEnvelopeDecoder](XmlEnvelopeDecoder.md 'Be.Stateless.BizTalk.MicroComponent.XmlEnvelopeDecoder') | |
| [XmlTranslator](XmlTranslator.md 'Be.Stateless.BizTalk.MicroComponent.XmlTranslator') | This component moves elements (and optionally attributes) from one namespace to another in the XML stream constituting the body of the message. |
| [XsltRunner](XsltRunner.md 'Be.Stateless.BizTalk.MicroComponent.XsltRunner') | Pipeline component that applies an XSL Transformation on messages along their way in the pipeline. |
| [ZipDecoder](ZipDecoder.md 'Be.Stateless.BizTalk.MicroComponent.ZipDecoder') | Pipeline component which decompresses the first entry of a Zip Archive. The component wraps the message's original stream in the zip decompressing stream [Be.Stateless.BizTalk.Stream.ZipInputStream](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Stream.ZipInputStream 'Be.Stateless.BizTalk.Stream.ZipInputStream'). |
| [ZipEncoder](ZipEncoder.md 'Be.Stateless.BizTalk.MicroComponent.ZipEncoder') | Pipeline component which compresses the incoming data into a Zip Archive. The component wraps the message's original stream in the zip-compressing stream [Be.Stateless.BizTalk.Stream.ZipOutputStream](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Stream.ZipOutputStream 'Be.Stateless.BizTalk.Stream.ZipOutputStream'). |

| Interfaces | |
| :--- | :--- |
| [IContextBuilder](IContextBuilder.md 'Be.Stateless.BizTalk.MicroComponent.IContextBuilder') | |
| [IMessageBodyStreamFactory](IMessageBodyStreamFactory.md 'Be.Stateless.BizTalk.MicroComponent.IMessageBodyStreamFactory') | |
| [IMicroComponent](IMicroComponent.md 'Be.Stateless.BizTalk.MicroComponent.IMicroComponent') | |