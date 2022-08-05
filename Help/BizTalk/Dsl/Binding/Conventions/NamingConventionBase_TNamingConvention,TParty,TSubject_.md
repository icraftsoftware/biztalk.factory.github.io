#### [Be.Stateless.BizTalk.Dsl.Binding.Conventions](README.md 'README')
### [Be.Stateless.BizTalk.Dsl.Binding.Convention](Be.Stateless.BizTalk.Dsl.Binding.Convention.md 'Be.Stateless.BizTalk.Dsl.Binding.Convention')

## NamingConventionBase<TNamingConvention,TParty,TSubject> Class

```csharp
public abstract class NamingConventionBase<TNamingConvention,TParty,TSubject>
    where TNamingConvention : Be.Stateless.BizTalk.Dsl.Binding.Convention.NamingConventionBase<TNamingConvention, TParty, TSubject>, Be.Stateless.BizTalk.Dsl.Binding.Convention.INamingConvention<TNamingConvention>
```
#### Type parameters

<a name='Be.Stateless.BizTalk.Dsl.Binding.Convention.NamingConventionBase_TNamingConvention,TParty,TSubject_.TNamingConvention'></a>

`TNamingConvention`

<a name='Be.Stateless.BizTalk.Dsl.Binding.Convention.NamingConventionBase_TNamingConvention,TParty,TSubject_.TParty'></a>

`TParty`

<a name='Be.Stateless.BizTalk.Dsl.Binding.Convention.NamingConventionBase_TNamingConvention,TParty,TSubject_.TSubject'></a>

`TSubject`

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; NamingConventionBase<TNamingConvention,TParty,TSubject>

Derived  
&#8627; [NamingConvention&lt;TParty,TSubject&gt;](NamingConvention_TParty,TSubject_.md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.Detailed.NamingConvention<TParty,TSubject>')  
&#8627; [NamingConvention](NamingConvention.md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.Simple.NamingConvention')

| Properties | |
| :--- | :--- |
| [ApplicationName](NamingConventionBase_TNamingConvention,TParty,TSubject_.ApplicationName.md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.NamingConventionBase<TNamingConvention,TParty,TSubject>.ApplicationName') | |
| [MessageFormat](NamingConventionBase_TNamingConvention,TParty,TSubject_.MessageFormat.md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.NamingConventionBase<TNamingConvention,TParty,TSubject>.MessageFormat') | |
| [Party](NamingConventionBase_TNamingConvention,TParty,TSubject_.Party.md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.NamingConventionBase<TNamingConvention,TParty,TSubject>.Party') | |
| [Subject](NamingConventionBase_TNamingConvention,TParty,TSubject_.Subject.md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.NamingConventionBase<TNamingConvention,TParty,TSubject>.Subject') | |

| Methods | |
| :--- | :--- |
| [ComputeAdapterName(IAdapter)](NamingConventionBase_TNamingConvention,TParty,TSubject_.ComputeAdapterName(IAdapter).md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.NamingConventionBase<TNamingConvention,TParty,TSubject>.ComputeAdapterName(Be.Stateless.BizTalk.Dsl.Binding.Adapter.IAdapter)') | |
| [ComputeAggregateName(Type)](NamingConventionBase_TNamingConvention,TParty,TSubject_.ComputeAggregateName(Type).md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.NamingConventionBase<TNamingConvention,TParty,TSubject>.ComputeAggregateName(System.Type)') | |
| [ComputeApplicationName(IApplicationBinding&lt;TNamingConvention&gt;)](NamingConventionBase_TNamingConvention,TParty,TSubject_.ComputeApplicationName(IApplicationBinding_TNamingConvention_).md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.NamingConventionBase<TNamingConvention,TParty,TSubject>.ComputeApplicationName(Be.Stateless.BizTalk.Dsl.Binding.IApplicationBinding<TNamingConvention>)') | |
| [ComputeReceiveLocationName(IReceiveLocation&lt;TNamingConvention&gt;)](NamingConventionBase_TNamingConvention,TParty,TSubject_.ComputeReceiveLocationName(IReceiveLocation_TNamingConvention_).md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.NamingConventionBase<TNamingConvention,TParty,TSubject>.ComputeReceiveLocationName(Be.Stateless.BizTalk.Dsl.Binding.IReceiveLocation<TNamingConvention>)') | |
| [ComputeReceivePortName(IReceivePort&lt;TNamingConvention&gt;)](NamingConventionBase_TNamingConvention,TParty,TSubject_.ComputeReceivePortName(IReceivePort_TNamingConvention_).md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.NamingConventionBase<TNamingConvention,TParty,TSubject>.ComputeReceivePortName(Be.Stateless.BizTalk.Dsl.Binding.IReceivePort<TNamingConvention>)') | |
| [ComputeSendPortName(ISendPort&lt;TNamingConvention&gt;)](NamingConventionBase_TNamingConvention,TParty,TSubject_.ComputeSendPortName(ISendPort_TNamingConvention_).md 'Be.Stateless.BizTalk.Dsl.Binding.Convention.NamingConventionBase<TNamingConvention,TParty,TSubject>.ComputeSendPortName(Be.Stateless.BizTalk.Dsl.Binding.ISendPort<TNamingConvention>)') | |
