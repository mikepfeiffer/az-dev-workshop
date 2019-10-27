# Lab 9 - Azure Service Bus Messaging with Azure Functions

1. Sign into the Azure portal and create a new Service Bus resource
2. After your Service Bus resource has been created, create a new Queue
3. Open a terminal and create a new folder called **SBConsole** and switch into this directory
4. Use the .NET CLI to create a new console app using the `dotnet new console` command
5. Add the Azure Service Bus nuget package using the `dotnet add package Microsoft.Azure.ServiceBus --version 4.1.0` command
6. Replace the code in Program.cs with the code [in this GitHub Gist](https://gist.github.com/mikepfeiffer/1d1d04f014b9929be7fcbc3382bb78a1)
6. Build your project using the `dotnet build` command
7. Switch to the build output folder `cd bin/Debug/netcoreapp3.0`
8. Run the console application using the following syntax: `dotnet SBConsole.dll -ConnectionString "myConnectionString" -QueueName "myQueueName"` to add messages to your Service Bus Queue (note: you can get the connection string for your Service Bus resource in the Azure portal)
9. Verify that the messages were sent by viewing the queue in the portal
9. Create an Azure Function app
10. Create a new Function in your Function app using the "Azure Service Bus Queue trigger" template
11. Navigate to the properties of your Function and open the log-streaming service window
12. Execute the console app again to watch the Function consume the messages in the queue


### Lifelines:

* [Use Azure portal to create a Service Bus queue](https://docs.microsoft.com/en-us/azure/service-bus-messaging/service-bus-quickstart-portal)


### Navigation:

* [Back to Lab Index](https://github.com/mikepfeiffer/az-dev-workshop)