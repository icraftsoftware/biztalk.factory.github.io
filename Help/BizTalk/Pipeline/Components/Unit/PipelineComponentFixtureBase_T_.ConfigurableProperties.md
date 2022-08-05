#### [Be.Stateless.BizTalk.Pipeline.Components.Unit](README.md 'README')
### [Be.Stateless.BizTalk.Unit.Component](Be.Stateless.BizTalk.Unit.Component.md 'Be.Stateless.BizTalk.Unit.Component').[PipelineComponentFixtureBase&lt;T&gt;](PipelineComponentFixtureBase_T_.md 'Be.Stateless.BizTalk.Unit.Component.PipelineComponentFixtureBase<T>')

## PipelineComponentFixtureBase<T>.ConfigurableProperties Property

All the properties of [Be.Stateless.BizTalk.Component.PipelineComponent](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Component.PipelineComponent 'Be.Stateless.BizTalk.Component.PipelineComponent')[T](PipelineComponentFixtureBase_T_.md#Be.Stateless.BizTalk.Unit.Component.PipelineComponentFixtureBase_T_.T 'Be.Stateless.BizTalk.Unit.Component.PipelineComponentFixtureBase<T>.T') that are to be read and written to an
[Microsoft.BizTalk.Component.Interop.IPropertyBag](https://docs.microsoft.com/en-us/dotnet/api/Microsoft.BizTalk.Component.Interop.IPropertyBag 'Microsoft.BizTalk.Component.Interop.IPropertyBag').

```csharp
protected virtual System.Collections.Generic.IEnumerable<System.Reflection.PropertyInfo> ConfigurableProperties { get; }
```

#### Property Value
[System.Collections.Generic.IEnumerable&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')[System.Reflection.PropertyInfo](https://docs.microsoft.com/en-us/dotnet/api/System.Reflection.PropertyInfo 'System.Reflection.PropertyInfo')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEnumerable-1 'System.Collections.Generic.IEnumerable`1')

### Remarks
Any property that is `public` and optionally qualified by a [[Browsable(true)]](https://docs.microsoft.com/en-us/dotnet/api/System.ComponentModel.BrowsableAttribute 'System.ComponentModel.BrowsableAttribute') attribute is considered to be a configurable [Be.Stateless.BizTalk.Component.PipelineComponent](https://docs.microsoft.com/en-us/dotnet/api/Be.Stateless.BizTalk.Component.PipelineComponent 'Be.Stateless.BizTalk.Component.PipelineComponent') property. Properties explicitly qualified by an [[Browsable(false)]](https://docs.microsoft.com/en-us/dotnet/api/System.ComponentModel.BrowsableAttribute 'System.ComponentModel.BrowsableAttribute') attribute are ignored.