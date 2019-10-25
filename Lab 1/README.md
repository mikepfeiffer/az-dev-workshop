# Lab 1 - Azure Subscription and Developer Workstation Setup

***Note: This lab can be performed on your local machine if you do not want to create an Azure VM and have full rights to install your own software***

1. Sign into **portal.azure.com**
2. Create a new "developer" virtual machine in the Azure portal -- search the Azure Marketplace for "***Visual Studio 2019 Latest***" -- and make sure to select "**Visual Studio 2019 Community (latest release) on Windows Server 2019 (x64)**" for the VM image
3. Make sure you can connect remotely via Remote Desktop Protocol (RDP)
4. Install [.NET Core 2.2](https://dotnet.microsoft.com/download/thank-you/dotnet-sdk-2.2.402-windows-x64-installer) on your developer VM
5. Startup and initialize your Cloud Shell environment at **shell.azure.com** (if you haven't done so already)
5. Open Visual Studio code and install the ***Azure Account*** extension
6. Launch the Cloud Shell inside your VS Code terminal
7. Enable Azure CLI interactive mode using the **az interactive** command
8. Use the **az find** command to search for CLI hints (e.g. "az find account")
9. Use the Azure CLI to list your subcription id(s)
10. Challenge: Use the CLI with the --Query parameter to return only the display names for the valid Azure regions available to your account

### Lifelines:

* [Create a Windows Virtual Machine in the Azure Portal](https://docs.microsoft.com/en-us/azure/virtual-machines/windows/quick-create-portal)
* [Quickstart for Bash in Azure Cloud Shell](https://docs.microsoft.com/en-us/azure/cloud-shell/quickstart)
* [Quickstart for PowerShell in Azure Cloud Shell](https://docs.microsoft.com/en-us/azure/cloud-shell/quickstart-powershell)

### Navigation:

* [Back to Lab Index](https://github.com/mikepfeiffer/az-dev-workshop)
