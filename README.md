# xUnit Test Code Snippets

## Summary

This is "code snippets" for Microsoft Visual Studio 2012 or higher.

If you use these "code snippets", you can save time to coding/typing to create unit test code based on xUnit framework.

![introduce movie](https://raw.githubusercontent.com/jsakamoto/xUnitTestCodeSnippets/master/.assets/movie-001.gif)

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

#### with Display Name

- `dfact` [Tab]

```csharp
[Fact(DisplayName = "")]
public void MyTestMethod()
{

}
```

### Insert xUnit Theory

And you can also insert **xUnit Theory method**.  
if you type following keys,

- `theory` [Tab]

Then, this snippet expanded following C# code.

```csharp
[Theory]
public void MyTheory()
{

}
```

#### with Display Name

- `dtheory` [Tab]

```csharp
[Theory(DisplayName = "")]
public void MyTheory()
{

}
```

### Insert xUnit Test Class

And you can also insert **xUnit test class**.  
if you type following keys,

- `xtestc` [Tab]

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

## and, "async" versions

- `afact`

```csharp
[Fact]
public async Task MyTestFact()
{

}
```

- `dafact`

```csharp
[Fact(DisplayName = "")]
public async Task MyTestFact()
{

}
```

- `atheory`

```csharp
[Theory]
public async Task MyTheory()
{

}
```

- `datheory`

```csharp
[Theory(DisplayName = "")]
public async Task MyTheory()
{

}
```

## Release Note
- v.1.4.0
 - Add suuport for Visual Studio 2019.
 - Snippets with "DisplayName" are added (`dfact`, `dafact`, `dtheory`, `datheory`).
- v.1.3.0
 - Add `afact` and `atheory` snippets to insert "async Task ..." methods.
- v.1.2.0
 - Add `theory` and `xtestc` snippets.
- v.1.1.0
 - Add `fact` snippet.
- v.1.0.0
 - 1st release, it contains `xtestm` snippet.


## License

[GNU GPL v.3](LICENSE.txt)
