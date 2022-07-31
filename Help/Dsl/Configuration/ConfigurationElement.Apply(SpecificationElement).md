#### [Be.Stateless.Dsl.Configuration](README.md 'README')
### [Be.Stateless.Dsl.Configuration](Be.Stateless.Dsl.Configuration.md 'Be.Stateless.Dsl.Configuration').[ConfigurationElement](ConfigurationElement.md 'Be.Stateless.Dsl.Configuration.ConfigurationElement')

## ConfigurationElement.Apply(SpecificationElement) Method

Apply the children [SpecificationElement](SpecificationElement.md 'Be.Stateless.Dsl.Configuration.SpecificationElement')s of the [SpecificationElement](SpecificationElement.md 'Be.Stateless.Dsl.Configuration.SpecificationElement')[specificationElement](ConfigurationElement.Apply(SpecificationElement).md#Be.Stateless.Dsl.Configuration.ConfigurationElement.Apply(Be.Stateless.Dsl.Configuration.SpecificationElement).specificationElement 'Be.Stateless.Dsl.Configuration.ConfigurationElement.Apply(Be.Stateless.Dsl.Configuration.SpecificationElement).specificationElement') to the children of the current [ConfigurationElement](ConfigurationElement.md 'Be.Stateless.Dsl.Configuration.ConfigurationElement') while transforming
—rewriting in place— the [SpecificationElement](SpecificationElement.md 'Be.Stateless.Dsl.Configuration.SpecificationElement')s into their inverse —undo— [SpecificationElement](SpecificationElement.md 'Be.Stateless.Dsl.Configuration.SpecificationElement')s on the fly.

```csharp
public void Apply(Be.Stateless.Dsl.Configuration.SpecificationElement specificationElement);
```
#### Parameters

<a name='Be.Stateless.Dsl.Configuration.ConfigurationElement.Apply(Be.Stateless.Dsl.Configuration.SpecificationElement).specificationElement'></a>

`specificationElement` [SpecificationElement](SpecificationElement.md 'Be.Stateless.Dsl.Configuration.SpecificationElement')

The [SpecificationElement](SpecificationElement.md 'Be.Stateless.Dsl.Configuration.SpecificationElement') whose children [SpecificationElement](SpecificationElement.md 'Be.Stateless.Dsl.Configuration.SpecificationElement')s will be applied to the
current [ConfigurationElement](ConfigurationElement.md 'Be.Stateless.Dsl.Configuration.ConfigurationElement').

#### Exceptions

[System.InvalidOperationException](https://docs.microsoft.com/en-us/dotnet/api/System.InvalidOperationException 'System.InvalidOperationException')  
If a child [SpecificationElement](SpecificationElement.md 'Be.Stateless.Dsl.Configuration.SpecificationElement') of the [specificationElement](ConfigurationElement.Apply(SpecificationElement).md#Be.Stateless.Dsl.Configuration.ConfigurationElement.Apply(Be.Stateless.Dsl.Configuration.SpecificationElement).specificationElement 'Be.Stateless.Dsl.Configuration.ConfigurationElement.Apply(Be.Stateless.Dsl.Configuration.SpecificationElement).specificationElement') cannot be applied
because it conflicts with an existing child of the current  [ConfigurationElement](ConfigurationElement.md 'Be.Stateless.Dsl.Configuration.ConfigurationElement').

### Remarks

The children of the [SpecificationElement](SpecificationElement.md 'Be.Stateless.Dsl.Configuration.SpecificationElement')[specificationElement](ConfigurationElement.Apply(SpecificationElement).md#Be.Stateless.Dsl.Configuration.ConfigurationElement.Apply(Be.Stateless.Dsl.Configuration.SpecificationElement).specificationElement 'Be.Stateless.Dsl.Configuration.ConfigurationElement.Apply(Be.Stateless.Dsl.Configuration.SpecificationElement).specificationElement') being applied are
crawled according to a depth-first search path. Then, for each child [SpecificationElement](SpecificationElement.md 'Be.Stateless.Dsl.Configuration.SpecificationElement') being
applied, its processing will happen according to its [Operation](SpecificationElement.Operation.md 'Be.Stateless.Dsl.Configuration.SpecificationElement.Operation') and whether the
current [ConfigurationElement](ConfigurationElement.md 'Be.Stateless.Dsl.Configuration.ConfigurationElement') has a child [ConfigurationElement](ConfigurationElement.md 'Be.Stateless.Dsl.Configuration.ConfigurationElement') satisfying or equating
this child [SpecificationElement](SpecificationElement.md 'Be.Stateless.Dsl.Configuration.SpecificationElement').

If the current [ConfigurationElement](ConfigurationElement.md 'Be.Stateless.Dsl.Configuration.ConfigurationElement') has no child [ConfigurationElement](ConfigurationElement.md 'Be.Stateless.Dsl.Configuration.ConfigurationElement') that satisfies or
equates the child [SpecificationElement](SpecificationElement.md 'Be.Stateless.Dsl.Configuration.SpecificationElement') being applied and the [SpecificationElement.Operation](SpecificationElement.Operation.md 'Be.Stateless.Dsl.Configuration.SpecificationElement.Operation') is
- an [INSERT](Specification.Annotations.Operation.INSERT.md 'Be.Stateless.Dsl.Configuration.Specification.Annotations.Operation.INSERT') or [UPSERT](Specification.Annotations.Operation.UPSERT.md 'Be.Stateless.Dsl.Configuration.Specification.Annotations.Operation.UPSERT') operation, then a new [ConfigurationElement](ConfigurationElement.md 'Be.Stateless.Dsl.Configuration.ConfigurationElement') with the specified name and attributes will be inserted and the child [SpecificationElement](SpecificationElement.md 'Be.Stateless.Dsl.Configuration.SpecificationElement') being applied will be transformed into its inverse [SpecificationElement](SpecificationElement.md 'Be.Stateless.Dsl.Configuration.SpecificationElement')
  with a [DELETE](Specification.Annotations.Operation.DELETE.md 'Be.Stateless.Dsl.Configuration.Specification.Annotations.Operation.DELETE') operation.
- an [UPDATE](Specification.Annotations.Operation.UPDATE.md 'Be.Stateless.Dsl.Configuration.Specification.Annotations.Operation.UPDATE') operation, then an [System.InvalidOperationException](https://docs.microsoft.com/en-us/dotnet/api/System.InvalidOperationException 'System.InvalidOperationException') will be thrown.
- a [DELETE](Specification.Annotations.Operation.DELETE.md 'Be.Stateless.Dsl.Configuration.Specification.Annotations.Operation.DELETE') operation, then no child [ConfigurationElement](ConfigurationElement.md 'Be.Stateless.Dsl.Configuration.ConfigurationElement') will be deleted and
  the child [SpecificationElement](SpecificationElement.md 'Be.Stateless.Dsl.Configuration.SpecificationElement') being applied will be transformed into its inverse [SpecificationElement](SpecificationElement.md 'Be.Stateless.Dsl.Configuration.SpecificationElement') with a [NONE](Specification.Annotations.Operation.NONE.md 'Be.Stateless.Dsl.Configuration.Specification.Annotations.Operation.NONE') operation.

If the current [ConfigurationElement](ConfigurationElement.md 'Be.Stateless.Dsl.Configuration.ConfigurationElement') has one child [ConfigurationElement](ConfigurationElement.md 'Be.Stateless.Dsl.Configuration.ConfigurationElement') that equates the
child [SpecificationElement](SpecificationElement.md 'Be.Stateless.Dsl.Configuration.SpecificationElement') being applied and the [SpecificationElement.Operation](SpecificationElement.Operation.md 'Be.Stateless.Dsl.Configuration.SpecificationElement.Operation') is
- an [INSERT](Specification.Annotations.Operation.INSERT.md 'Be.Stateless.Dsl.Configuration.Specification.Annotations.Operation.INSERT') operation, then the equating child [ConfigurationElement](ConfigurationElement.md 'Be.Stateless.Dsl.Configuration.ConfigurationElement') will be
  left untouched and the child [SpecificationElement](SpecificationElement.md 'Be.Stateless.Dsl.Configuration.SpecificationElement') being applied will be transformed into its inverse
  [SpecificationElement](SpecificationElement.md 'Be.Stateless.Dsl.Configuration.SpecificationElement') with a [NONE](Specification.Annotations.Operation.NONE.md 'Be.Stateless.Dsl.Configuration.Specification.Annotations.Operation.NONE') operation.
- an [UPDATE](Specification.Annotations.Operation.UPDATE.md 'Be.Stateless.Dsl.Configuration.Specification.Annotations.Operation.UPDATE') or [UPSERT](Specification.Annotations.Operation.UPSERT.md 'Be.Stateless.Dsl.Configuration.Specification.Annotations.Operation.UPSERT') operation, then, depending on whether
  attributes of the equating child [ConfigurationElement](ConfigurationElement.md 'Be.Stateless.Dsl.Configuration.ConfigurationElement') would have to be scrapped or not, the child
  [SpecificationElement](SpecificationElement.md 'Be.Stateless.Dsl.Configuration.SpecificationElement') being applied will be transformed into its inverse [SpecificationElement](SpecificationElement.md 'Be.Stateless.Dsl.Configuration.SpecificationElement') with either an [UPDATE](Specification.Annotations.Operation.UPDATE.md 'Be.Stateless.Dsl.Configuration.Specification.Annotations.Operation.UPDATE') or a [NONE](Specification.Annotations.Operation.NONE.md 'Be.Stateless.Dsl.Configuration.Specification.Annotations.Operation.NONE')
  operation.
- a [DELETE](Specification.Annotations.Operation.DELETE.md 'Be.Stateless.Dsl.Configuration.Specification.Annotations.Operation.DELETE') operation, then the equating child [ConfigurationElement](ConfigurationElement.md 'Be.Stateless.Dsl.Configuration.ConfigurationElement') will be
  deleted and the child [SpecificationElement](SpecificationElement.md 'Be.Stateless.Dsl.Configuration.SpecificationElement') being applied will be transformed into its inverse [SpecificationElement](SpecificationElement.md 'Be.Stateless.Dsl.Configuration.SpecificationElement') with a [INSERT](Specification.Annotations.Operation.INSERT.md 'Be.Stateless.Dsl.Configuration.Specification.Annotations.Operation.INSERT') operation.
If the current [ConfigurationElement](ConfigurationElement.md 'Be.Stateless.Dsl.Configuration.ConfigurationElement') has one child [ConfigurationElement](ConfigurationElement.md 'Be.Stateless.Dsl.Configuration.ConfigurationElement') that satisfies
but does not equate the child [SpecificationElement](SpecificationElement.md 'Be.Stateless.Dsl.Configuration.SpecificationElement') being applied and the [SpecificationElement.Operation](SpecificationElement.Operation.md 'Be.Stateless.Dsl.Configuration.SpecificationElement.Operation') is
- an [INSERT](Specification.Annotations.Operation.INSERT.md 'Be.Stateless.Dsl.Configuration.Specification.Annotations.Operation.INSERT') or a [DELETE](Specification.Annotations.Operation.DELETE.md 'Be.Stateless.Dsl.Configuration.Specification.Annotations.Operation.DELETE') operation, then an [System.InvalidOperationException](https://docs.microsoft.com/en-us/dotnet/api/System.InvalidOperationException 'System.InvalidOperationException') will be thrown.
- an [UPDATE](Specification.Annotations.Operation.UPDATE.md 'Be.Stateless.Dsl.Configuration.Specification.Annotations.Operation.UPDATE') or [UPSERT](Specification.Annotations.Operation.UPSERT.md 'Be.Stateless.Dsl.Configuration.Specification.Annotations.Operation.UPSERT') operation, then, depending on whether
  attributes of the equating child [ConfigurationElement](ConfigurationElement.md 'Be.Stateless.Dsl.Configuration.ConfigurationElement') would have to be updated or not, the child [SpecificationElement](SpecificationElement.md 'Be.Stateless.Dsl.Configuration.SpecificationElement') being applied will be transformed into its inverse [SpecificationElement](SpecificationElement.md 'Be.Stateless.Dsl.Configuration.SpecificationElement')
  with either an [UPDATE](Specification.Annotations.Operation.UPDATE.md 'Be.Stateless.Dsl.Configuration.Specification.Annotations.Operation.UPDATE') or a [NONE](Specification.Annotations.Operation.NONE.md 'Be.Stateless.Dsl.Configuration.Specification.Annotations.Operation.NONE') operation.

### See Also
- [IsEquatedBy(ConfigurationElement)](SpecificationElement.IsEquatedBy(ConfigurationElement).md 'Be.Stateless.Dsl.Configuration.SpecificationElement.IsEquatedBy(Be.Stateless.Dsl.Configuration.ConfigurationElement)')
- [IsSatisfiedBy(ConfigurationElement)](SpecificationElement.IsSatisfiedBy(ConfigurationElement).md 'Be.Stateless.Dsl.Configuration.SpecificationElement.IsSatisfiedBy(Be.Stateless.Dsl.Configuration.ConfigurationElement)')