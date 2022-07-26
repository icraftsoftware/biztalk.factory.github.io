#### [Be.Stateless.Extensions](README.md 'README')
### [Be.Stateless.IO.Extensions](Be.Stateless.IO.Extensions.md 'Be.Stateless.IO.Extensions').[PathExtensions](PathExtensions.md 'Be.Stateless.IO.Extensions.PathExtensions')

## PathExtensions.GetCommonPath(this string[], char[]) Method

Returns a string representing that part of the path tree that is common to all the paths.

```csharp
public static string GetCommonPath(this string[] paths, params char[] separators);
```
#### Parameters

<a name='Be.Stateless.IO.Extensions.PathExtensions.GetCommonPath(thisstring[],char[]).paths'></a>

`paths` [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')[[]](https://docs.microsoft.com/en-us/dotnet/api/System.Array 'System.Array')

The set of paths describing the path tree to extract the longest common path from.

<a name='Be.Stateless.IO.Extensions.PathExtensions.GetCommonPath(thisstring[],char[]).separators'></a>

`separators` [System.Char](https://docs.microsoft.com/en-us/dotnet/api/System.Char 'System.Char')[[]](https://docs.microsoft.com/en-us/dotnet/api/System.Array 'System.Array')

Path separators; it defaults to both [System.IO.Path.DirectorySeparatorChar](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Path.DirectorySeparatorChar 'System.IO.Path.DirectorySeparatorChar') and `, `[System.IO.Path.AltDirectorySeparatorChar](https://docs.microsoft.com/en-us/dotnet/api/System.IO.Path.AltDirectorySeparatorChar 'System.IO.Path.AltDirectorySeparatorChar')`]`.

#### Returns
[System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String')  
The longest common path of the set of [paths](PathExtensions.GetCommonPath(thisstring[],char[]).md#Be.Stateless.IO.Extensions.PathExtensions.GetCommonPath(thisstring[],char[]).paths 'Be.Stateless.IO.Extensions.PathExtensions.GetCommonPath(this string[], char[]).paths').

### Remarks
The resultant path is a valid path and not just the longest common string; that is to say that no path segment will
be truncated.

### See Also
- [Longest Common Prefix with C# and LINQ](http://blogs.microsoft.co.il/yuvmaz/2013/05/10/longest-common-prefix-with-c-and-linq/ 'http://blogs.microsoft.co.il/yuvmaz/2013/05/10/longest-common-prefix-with-c-and-linq/')
- [Longest Common Prefix](https://miafish.wordpress.com/2015/02/17/leetcode-oj-c-longest-common-prefix/ 'https://miafish.wordpress.com/2015/02/17/leetcode-oj-c-longest-common-prefix/')
- [Find common directory path](https://www.rosettacode.org/wiki/Find_common_directory_path 'https://www.rosettacode.org/wiki/Find_common_directory_path')
- [Find common prefix of strings](https://stackoverflow.com/questions/2070356/find-common-prefix-of-strings 'https://stackoverflow.com/questions/2070356/find-common-prefix-of-strings')
- [Get common prefix of two string](https://stackoverflow.com/questions/33709165/get-common-prefix-of-two-string 'https://stackoverflow.com/questions/33709165/get-common-prefix-of-two-string')