# Lab 7 - Deploying an Azure SQL Database and Performing an Entity Framework Migration

1. Login to the Azure portal and click on "Create a resource" > search for "web app sql" > use this template to create an App Service Web App and Managed Azure SQL database (note: make sure you provision all resources in the same region)
2. Clone the MovieApp repo to your local machine (note: this app uses .NET Core 3.0)
3. Update the "RazorPagesMovieContext" in appsettings.json with your Azure SQL database connection string (note: you can find this in the Azure portal in the properties of your DB)
4. Configure your Azure SQL server firewall settings to allow traffic from your developer machine
5. Switch to the application directory and run `dotnet ef database update` to update the database
6. Run the app locally and navigate to https://localhost:5001/movies to validate
7. Update the "Movie" class and add a "Description" property (This model is defined in MovieDateRatingDA.cs)
8. Use the `dotnet ef migrations add addDescription` command to add a migration
9. Run `dotnet ef database update` to update the database (note: you can use the Query editor in the Azure portal to validate)
10. Bonus: Deploy the app from Visual Studio or VS Code (note: You'll need the "Azure Account" and "App Service" extentions installed in VS Code, or the Azure workload installed in Visual Studio)

### Lifelines:

* [Build an ASP.NET Core and SQL Database app in Azure App Service](https://docs.microsoft.com/en-us/azure/app-service/app-service-web-tutorial-dotnetcore-sqldb)

* [Entity Framework Migrations](https://docs.microsoft.com/en-us/ef/core/managing-schemas/migrations/)


### Navigation:

* [Back to Lab Index](https://github.com/mikepfeiffer/az-dev-workshop)