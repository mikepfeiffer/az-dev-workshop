# Lab 3 - Working with the Azure App Configuration Service

1. Create an app configuration store in the Azure portal (search the marketplace for "App Configuration")
2. Select Configuration Explorer > + Create to add a key-value pair:
 * Key = BackgroundColor
 * Value = #000000;
3. Use the .NET CLI to create a new ASP.NET Core web app `dotnet new webapp`
4. Next, use the .NET Core User Secrets tool to store the connection string for our new App Configuration service `dotnet user-secrets set ConnectionStrings:AppConfig <YOUR CONNECTION STRING>` (note: you can find your connection string in the Access Keys setting section of your App Configuration resource)
4. Add a reference to the AzureAppConfiguration provider for .NET Core `dotnet add package Microsoft.Extensions.Configuration.AzureAppConfiguration --version 1.0.0-preview-007830001`
5. Update your program.cs file as shown in step 5 of [this quickstart](https://docs.microsoft.com/en-us/azure/azure-app-configuration/quickstart-aspnet-core-app#connect-to-an-app-configuration-store)
6. Update your index.cshtml page as shown in step 6 of [this quickstart](https://docs.microsoft.com/en-us/azure/azure-app-configuration/quickstart-aspnet-core-app#connect-to-an-app-configuration-store) to retrieve the value of **BackgroundColor** key. Use this value to override the background color of the page.
7. Run the app and validate that it works.

### Lifelines:

* [Quickstart: Create an ASP.NET Core app with Azure App Configuration](https://docs.microsoft.com/en-us/azure/azure-app-configuration/quickstart-aspnet-core-app#connect-to-an-app-configuration-store)

* [Understanding Azure's New App Configuration Service](https://www.petri.com/preview-azures-new-app-configuration-service)

### Navigation:

* [Back to Lab Index](https://github.com/mikepfeiffer/az-dev-workshop)