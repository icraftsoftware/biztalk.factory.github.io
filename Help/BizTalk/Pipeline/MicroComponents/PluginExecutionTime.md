#### [Be.Stateless.BizTalk.Pipeline.MicroComponents](README.md 'README')
### [Be.Stateless.BizTalk](Be.Stateless.BizTalk.md 'Be.Stateless.BizTalk')

## PluginExecutionTime Enum

The time at which a micro component's plugin will be executed. A plugin can take various forms ranging, for instance,
from an [IMessageBodyStreamFactory](IMessageBodyStreamFactory.md 'Be.Stateless.BizTalk.MicroComponent.IMessageBodyStreamFactory') to an [IContextBuilder](IContextBuilder.md 'Be.Stateless.BizTalk.MicroComponent.IContextBuilder').

```csharp
public enum PluginExecutionTime
```
### Fields

<a name='Be.Stateless.BizTalk.PluginExecutionTime.Deferred'></a>

`Deferred` 1

Executes the plugin only after the message stream has been exhausted.

<a name='Be.Stateless.BizTalk.PluginExecutionTime.Immediate'></a>

`Immediate` 0

Executes the plugin as soon as its hosting micro component starts being executed.

### Remarks
The execution time can either be [Immediate](PluginExecutionTime.md#Be.Stateless.BizTalk.PluginExecutionTime.Immediate 'Be.Stateless.BizTalk.PluginExecutionTime.Immediate'), in which case the plugin will be executed as soon as its
hosting micro component —e.g. the [ContextBuilder](ContextBuilder.md 'Be.Stateless.BizTalk.MicroComponent.ContextBuilder') or the [MessageBodyStreamFactory](MessageBodyStreamFactory.md 'Be.Stateless.BizTalk.MicroComponent.MessageBodyStreamFactory')— starts being executed, or [Deferred](PluginExecutionTime.md#Be.Stateless.BizTalk.PluginExecutionTime.Deferred 'Be.Stateless.BizTalk.PluginExecutionTime.Deferred'), in which case its hosting
micro component will wait for the message stream to be exhausted to execute the plugin.