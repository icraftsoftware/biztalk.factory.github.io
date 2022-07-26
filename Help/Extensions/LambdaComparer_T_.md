#### [Be.Stateless.Extensions](README.md 'README')
### [Be.Stateless.Linq](Be.Stateless.Linq.md 'Be.Stateless.Linq')

## LambdaComparer<T> Class

Provides a [System.Collections.Generic.IEqualityComparer&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEqualityComparer-1 'System.Collections.Generic.IEqualityComparer`1') wrapper that delegates to lambdas that support the comparison of objects
for equality.

```csharp
public class LambdaComparer<T> : System.Collections.Generic.EqualityComparer<T>
```
#### Type parameters

<a name='Be.Stateless.Linq.LambdaComparer_T_.T'></a>

`T`

The type of objects to compare.

Inheritance [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') &#129106; [System.Collections.Generic.EqualityComparer&lt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.EqualityComparer-1 'System.Collections.Generic.EqualityComparer`1')[T](LambdaComparer_T_.md#Be.Stateless.Linq.LambdaComparer_T_.T 'Be.Stateless.Linq.LambdaComparer<T>.T')[&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.EqualityComparer-1 'System.Collections.Generic.EqualityComparer`1') &#129106; LambdaComparer<T>

### Remarks
It is recommended to derive from the [System.Collections.Generic.EqualityComparer&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.EqualityComparer-1 'System.Collections.Generic.EqualityComparer`1') class instead of implementing the [System.Collections.Generic.IEqualityComparer&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.IEqualityComparer-1 'System.Collections.Generic.IEqualityComparer`1') interface, because the [System.Collections.Generic.EqualityComparer&lt;&gt;](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.Generic.EqualityComparer-1 'System.Collections.Generic.EqualityComparer`1') class tests for equality using
the [IEquatable&lt;T&gt;.Equals(T)](https://docs.microsoft.com/en-us/dotnet/api/System.IEquatable-1.Equals#System_IEquatable_1_Equals__0_ 'System.IEquatable`1.Equals(`0)') method instead of the [Object.Equals(object)](https://docs.microsoft.com/en-us/dotnet/api/System.Object.Equals#System_Object_Equals_System_Object_ 'System.Object.Equals(System.Object)') method.

### See Also
- [http://brendan.enrick.com/blog/linq-your-collections-with-iequalitycomparer-and-lambda-expressions/](http://brendan.enrick.com/blog/linq-your-collections-with-iequalitycomparer-and-lambda-expressions/ 'http://brendan.enrick.com/blog/linq-your-collections-with-iequalitycomparer-and-lambda-expressions/')
- [https://docs.microsoft.com/en-us/dotnet/api/system.collections.generic.iequalitycomparer-1](https://docs.microsoft.com/en-us/dotnet/api/system.collections.generic.iequalitycomparer-1 'https://docs.microsoft.com/en-us/dotnet/api/system.collections.generic.iequalitycomparer-1')
- [https://docs.microsoft.com/en-us/dotnet/api/system.collections.generic.equalitycomparer-1](https://docs.microsoft.com/en-us/dotnet/api/system.collections.generic.equalitycomparer-1 'https://docs.microsoft.com/en-us/dotnet/api/system.collections.generic.equalitycomparer-1')

| Constructors | |
| :--- | :--- |
| [LambdaComparer(Func&lt;T,T,bool&gt;, Func&lt;T,int&gt;)](LambdaComparer_T_.LambdaComparer(Func_T,T,bool_,Func_T,int_).md 'Be.Stateless.Linq.LambdaComparer<T>.LambdaComparer(System.Func<T,T,bool>, System.Func<T,int>)') | |
| [LambdaComparer(Func&lt;T,T,bool&gt;)](LambdaComparer_T_.LambdaComparer(Func_T,T,bool_).md 'Be.Stateless.Linq.LambdaComparer<T>.LambdaComparer(System.Func<T,T,bool>)') | |

| Methods | |
| :--- | :--- |
| [Equals(T, T)](LambdaComparer_T_.Equals(T,T).md 'Be.Stateless.Linq.LambdaComparer<T>.Equals(T, T)') | |
| [GetHashCode(T)](LambdaComparer_T_.GetHashCode(T).md 'Be.Stateless.Linq.LambdaComparer<T>.GetHashCode(T)') | |
