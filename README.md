# cShap-snippets

Code snippets are templates that make easier to enter repeating code patterns, such as loops or conditional-statements.

In Visual Studio Code, snippets show in IntelliSense mixed with other suggestions as well as in a dedicated snippet picker.  type a snippet prefix, and press Tab to insert a snippet.

The snippet syntax follows the TextMate snippet syntax with the exceptions of 'interpolated shell code' and the use of \u; both are not supported.

You are going to be able to create In this snippets a Razor Page and Code behind of your Razor Page.

### Configuration
Depending on your platform, your snippets file is copied here: 
* Windows : ``` %APPDATA%\Code\User\snippets\ ```
* macOS : ``` $HOME/Library/Application Support/Code/User/snippets/ ```
* Linux : ``` $HOME/.config/Code/User/snippets/ ```

If you use VSCode:
Open Snippets/csharp.json (in this Report) > copy content of this file > go to VSCode > Click in button Manage > select user Snippets > type CSharp.json and select this file > paste the Snippets content.

### How to use
For generating a Razor Page use this key in your file .cshtml:
> blazor-page 

Your get this code:
```cSharp
@page
@{
    ViewData["Title"] = "Title";
}
<h1>Index</h1>
```

If you want to generate a code behind in your Blazor Page use this key in your file .cshtml.cs:

> blazor-page-code-behind 

Your get this code:
```cSharp
using System;
using Microsoft.AspNetCore.Mvc;
using Microsoft.AspNetCore.Mvc.RazorPages;

namespace NameProject.Pages
{
    public class NamePageModel : PageModel
    {
         public void OnGet()
        {
             
        }
    }
}
```

##### Generating class
type this command in your file, for generating class structure:

> class

Your get this code:
```cSharp
using System;

namespace NameProject
{
    public class MyClass
    {
            
    }
}
```

##### Generating comment
Type this command in the headers of your Function or Methods, for generating a comment:

> comment

Your get this code:
```cSharp
/// <summary>
/// Description
/// </summary>
/// <param name="ParameterName"> Value </param>
/// <returns> string </returns>
```
