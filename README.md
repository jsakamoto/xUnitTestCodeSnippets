# xUnit Test Code Snippets

## Summary

This is "code snippets" for Microsoft Visual Studio 2012 or higher.

If you use these "code snippets", you can save time to coding/typing to create unit test code based on xUnit framework.

## How to install

1. Download "xUnitTestCodeSnippets... .vsix" (Microsoft Visual Studio Extension) file from "Visual Studio Gallery" site.  
URL: [https://visualstudiogallery.msdn.microsoft.com/032cd260-d4cd-4849-adff-648ea9a28265](https://visualstudiogallery.msdn.microsoft.com/032cd260-d4cd-4849-adff-648ea9a28265)
2. Open (double click on Explorer) the downloaded "xUnitTestCodeSnippets... .vsix" file.
3. Then, "VSIX Installer" was launched. Please click "Install".

## How to use

### Insert xUnit Fact

On C# source code in Visual Studio, you can insert **xUnit Fact method** by following key typing.

- `xtestm` [Tab]  
or
- `fact` [Tab]

Then, this snippet expanded following C# code.

```csharp
[Fact]
public void MyTestMethod()
{

}
```

### Insert xUnit Theory

And you can also insert **xUnit Theory method**.  
if you type following keys,

`theory`

Then, this snippet expanded following C# code.

```csharp
[Theory]
public void MyTheory()
{

}
```

### Insert xUnit Test Class

And you can also insert **xUnit test class**.  
if you type following keys,

`xtestc`

Then, this snippet expanded following C# code.

```csharp
public class MyTestClass
{
    [Fact]
    public void MyTestFact()
    {

    }
}
```

## Release Note
- v.1.2.0
 - Add `theory` and `xtestc` snippets.
- v.1.1.0
 - Add `fact` snippet.
- v.1.0.0
 - 1st release, it contains `xtestm` snippet.
