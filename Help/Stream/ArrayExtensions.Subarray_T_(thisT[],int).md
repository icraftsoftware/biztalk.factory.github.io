#### [Be.Stateless.Stream](README.md 'README')
### [Be.Stateless.Extensions](Be.Stateless.Extensions.md 'Be.Stateless.Extensions').[ArrayExtensions](ArrayExtensions.md 'Be.Stateless.Extensions.ArrayExtensions')

## ArrayExtensions.Subarray<T>(this T[], int) Method

Retrieves a subarray, from this [array](ArrayExtensions.Subarray_T_(thisT[],int).md#Be.Stateless.Extensions.ArrayExtensions.Subarray_T_(thisT[],int).array 'Be.Stateless.Extensions.ArrayExtensions.Subarray<T>(this T[], int).array'), that starts at a specified position.

```csharp
public static T[] Subarray<T>(this T[] array, int startIndex);
```
#### Type parameters

<a name='Be.Stateless.Extensions.ArrayExtensions.Subarray_T_(thisT[],int).T'></a>

`T`

The type of this [array](ArrayExtensions.Subarray_T_(thisT[],int).md#Be.Stateless.Extensions.ArrayExtensions.Subarray_T_(thisT[],int).array 'Be.Stateless.Extensions.ArrayExtensions.Subarray<T>(this T[], int).array')'s elements.
#### Parameters

<a name='Be.Stateless.Extensions.ArrayExtensions.Subarray_T_(thisT[],int).array'></a>

`array` [T](ArrayExtensions.Subarray_T_(thisT[],int).md#Be.Stateless.Extensions.ArrayExtensions.Subarray_T_(thisT[],int).T 'Be.Stateless.Extensions.ArrayExtensions.Subarray<T>(this T[], int).T')[[]](https://docs.microsoft.com/en-us/dotnet/api/System.Array 'System.Array')

This array.

<a name='Be.Stateless.Extensions.ArrayExtensions.Subarray_T_(thisT[],int).startIndex'></a>

`startIndex` [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32')

The zero-based starting position of a subarray in this [array](ArrayExtensions.Subarray_T_(thisT[],int).md#Be.Stateless.Extensions.ArrayExtensions.Subarray_T_(thisT[],int).array 'Be.Stateless.Extensions.ArrayExtensions.Subarray<T>(this T[], int).array').

#### Returns
[T](ArrayExtensions.Subarray_T_(thisT[],int).md#Be.Stateless.Extensions.ArrayExtensions.Subarray_T_(thisT[],int).T 'Be.Stateless.Extensions.ArrayExtensions.Subarray<T>(this T[], int).T')[[]](https://docs.microsoft.com/en-us/dotnet/api/System.Array 'System.Array')  
An [System.Array](https://docs.microsoft.com/en-us/dotnet/api/System.Array 'System.Array') of [T](ArrayExtensions.Subarray_T_(thisT[],int).md#Be.Stateless.Extensions.ArrayExtensions.Subarray_T_(thisT[],int).T 'Be.Stateless.Extensions.ArrayExtensions.Subarray<T>(this T[], int).T') that is equivalent to the subarray that begins at [startIndex](ArrayExtensions.Subarray_T_(thisT[],int).md#Be.Stateless.Extensions.ArrayExtensions.Subarray_T_(thisT[],int).startIndex 'Be.Stateless.Extensions.ArrayExtensions.Subarray<T>(this T[], int).startIndex') in this [array](ArrayExtensions.Subarray_T_(thisT[],int).md#Be.Stateless.Extensions.ArrayExtensions.Subarray_T_(thisT[],int).array 'Be.Stateless.Extensions.ArrayExtensions.Subarray<T>(this T[], int).array'), or `null` if [startIndex](ArrayExtensions.Subarray_T_(thisT[],int).md#Be.Stateless.Extensions.ArrayExtensions.Subarray_T_(thisT[],int).startIndex 'Be.Stateless.Extensions.ArrayExtensions.Subarray<T>(this T[], int).startIndex') is equal
to the length of this [array](ArrayExtensions.Subarray_T_(thisT[],int).md#Be.Stateless.Extensions.ArrayExtensions.Subarray_T_(thisT[],int).array 'Be.Stateless.Extensions.ArrayExtensions.Subarray<T>(this T[], int).array').