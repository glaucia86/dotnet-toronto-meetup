# Power up with Azure Functions & .NET Core - Demo

[![Dot-Net-Bot-Bit.png](https://i.postimg.cc/fTw454HR/Dot-Net-Bot-Bit.png)](https://postimg.cc/t7mmCcQK)

Repository responsible for the demos during the meetup event: **[Metro Toronto .NET User Group](https://aka.ms/AA6xcx9)**

## Resources/Tools Used 💻

- **[.NET Core 3.x](https://dotnet.microsoft.com/download?WT.mc_id=javascript-0000-gllemos)**
- **[Visual Studio Code](https://code.visualstudio.com/?WT.mc_id=javascript-0000-gllemos)**
- **[C# Extension - Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.csharp&WT.mc_id=javascript-0000-gllemos)**
- **[Azure Functions Extension](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-azurefunctions&WT.mc_id=javascript-0000-gllemos)**
- **[Blazor](https://dotnet.microsoft.com/apps/aspnet/web-apps/blazor?WT.mc_id=javascript-0000-gllemos)**
- **[Azure Functions Core Tools](https://docs.microsoft.com/azure/azure-functions/functions-run-local?WT.mc_id=javascript-0000-gllemos)**

## Azure For Students Account ⭐️

If you are a student at a College or University, you can create your [Azure for Students account](https://azure.microsoft.com/free/students/?WT.mc_id=javascript-0000-gllemos). This account will give you the benefit of having a $ 100 credit to use the Azure Services for free, without having a credit card and free developer tools as well. To activate this account, just access the link [HERE](https://azure.microsoft.com/free/students/?WT.mc_id=javascript-0000-gllemos).

## How to run the Application locally? 🚀

1. Install the **[.NET Core 3.1 SDK](https://dotnet.microsoft.com/download/dotnet-core/3.1?WT.mc_id=javascript-0000-gllemos)**.

2. Install the **[.NET Core 3.1 or later (Preview) SDK](https://dotnet.microsoft.com/download?WT.mc_id=javascript-0000-gllemos)**.

3. Run the following command in a command shell. The **[Microsoft.AspNetCore.Blazor.Templates](https://www.nuget.org/packages/Microsoft.AspNetCore.Blazor.Templates/)** package has a preview version while Blazor WebAssembly is in preview.

4. Install Blazor in your machine as follow below: 

```bash
> dotnet new -i Microsoft.AspNetCore.Blazor.Templates::3.1.0-preview4.19579.2
```

3. Now go to the `FunctionApp` and create a file called `local.settings.json`. Include the code below:

```json
{
    "IsEncrypted": false,
    "Values": {
        "AzureWebJobsStorage": "",
        "FUNCTIONS_WORKER_RUNTIME": "dotnet"
    },
    "Host": {
      "LocalHttpPort": 7071,
      "CORS": "*"
    }
}
```

4. Now execute the command: (inside in the folder: `FunctionApp` )

```bash
> func host start
```

This command will generate a Endpoint API: `http://localhost:7071/api/Hello`

5. Now, go to the `BlazorApp` folder and execute the command:

```bash
> dotnet run
```

And vòilá! The application will be running correctly!

## Next Steps 🏃

Learn more about serverless with a Free Training!

- ✅ **[Serverless Free Courses](https://docs.microsoft.com/learn/browse/?term=azure&WT.mc_id=javascript-0000-gllemos functions&WT.mc_id=javascript-0000-gllemos)**

- ✅ **[Free Courses - .NET Core C# ](https://docs.microsoft.com/learn/browse/?products=dotnet&WT.mc_id=javascript-0000-gllemos)**

## Important Resources ⭐️

-   ✅ **[Azure Functions documentation](https://docs.microsoft.com/azure/azure-functions/?WT.mc_id=javascript-0000-gllemos)**
-   ✅ **[Publish an ASP.NET Core app to Azure with Visual Studio Code](https://docs.microsoft.com/aspnet/core/tutorials/publish-to-azure-webapp-using-vscode?view=aspnetcore-3.1&viewFallbackFrom=aspnetcore-3.0&WT.mc_id=javascript-0000-gllemos)**
-   ✅ **[Create your first function using Visual Studio](https://docs.microsoft.com/azure/azure-functions/functions-create-your-first-function-visual-studio?WT.mc_id=javascript-0000-gllemos)**
-   ✅ **[Introduction to ASP.NET Core Blazor](https://docs.microsoft.com/aspnet/core/blazor/?view=aspnetcore-3.1&WT.mc_id=javascript-0000-gllemos)**
-   ✅ **[Host and deploy ASP.NET Core](https://docs.microsoft.com/aspnet/core/host-and-deploy/?view=aspnetcore-3.0&WT.mc_id=javascript-0000-gllemos)**
-   ✅ **[Blazor for ASP.NET Web Forms Developers](https://docs.microsoft.com/dotnet/architecture/blazor-for-web-forms-developers/?WT.mc_id=javascript-0000-gllemos)**
-   ✅ **[Announcing .NET Core 3.0](https://devblogs.microsoft.com/dotnet/announcing-net-core-3-0/?WT.mc_id=javascript-0000-gllemos)**

## Questions? Comments? ❓

If you have any questions about the challenges, feel free to open an **[ISSUE HERE](https://github.com/glaucia86/dotnet-toronto-meetup/issues)**. We'll get back to you soon!
