#### [Be.Stateless.BizTalk.Dsl.Binding](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding](Be.Stateless.BizTalk.Dsl.Binding.md 'Be.Stateless.BizTalk.Dsl.Binding').[ISendPort&lt;TNamingConvention&gt;](ISendPort_TNamingConvention_.md 'Be.Stateless.BizTalk.Dsl.Binding.ISendPort<TNamingConvention>')

## ISendPort<TNamingConvention>.Filter Property

Define conditions based on message context's promoted properties that determine which messages are routed to
the send port.

```csharp
Be.Stateless.BizTalk.Dsl.Binding.Subscription.Filter Filter { get; set; }
```

#### Property Value
[Filter](Filter.md 'Be.Stateless.BizTalk.Dsl.Binding.Subscription.Filter')

### Example

```csharp
Filter = new Be.Stateless.BizTalk.Dsl.Binding.Subscription.Filter(
              () => BtsProperties.MessageType == Schema<SomeSchema>.MessageType && BizTalkFactoryProperties.EnvironmentTag == 'ONE'
                || BtsProperties.MessageType == Schema<OtherSchema>.MessageType && BizTalkFactoryProperties.EnvironmentTag == 'TWO'
            );
```