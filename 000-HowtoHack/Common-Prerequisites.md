# What The Hack: Common Prerequisites

Thanks for participating in a What The Hack! We have compiled a list of common tools and software that will come in handy to complete these Azure based hacks!

You might not need all of them for the hack you are participating in. However, if you work with Azure on a regular basis, these are all things you should consider having in your toolbox.

- [Azure Subscription](#azure-subscription)
- [Windows Subsystem for Linux](#windows-subsystem-for-linux)
- [Managing Cloud Resources](#managing-cloud-resources)
  - [Azure Portal](#azure-portal)
  - [Azure CLI](#azure-cli)
    - [Note for Windows Users](#note-for-windows-users)
  - [Azure PowerShell CmdLets](#azure-powershell-cmdlets)
  - [Azure Cloud Shell](#azure-cloud-shell)
- [Visual Studio Code](#visual-studio-code)
  - [Visual Studio Code plugins for ARM Templates](#visual-studio-code-plugins-for-arm-templates)
- [Azure Storage Explorer](#azure-storage-explorer)

## Azure Subscription

You will need an Azure subscription to complete this hackathon. If you don't have one...

[Sign Up for Azure HERE](https://azure.microsoft.com/en-us/free/)

Our goal in the hackathon is limiting the cost of using Azure services.

If you've never used Azure, you will get:

- $200 free credits for use for up to 30 days
- 12 months of popular free services (includes storage, Linux VMs)
- Then there are services that are free up to a certain quota

Details can be found here on [free services](https://azure.microsoft.com/en-us/free/).

If you have used Azure before, we will still try to limit cost of services by suspending, shutting down services, or destroy services before end of the hackathon. You will still be able to use the free services (up to their quotas) like App Service, or Functions.

## Managing Cloud Resources

We can manage cloud resources via the following ways:

- Web Interface/Dashboard
  - [Azure Portal](https://portal.azure.com/)
- CLI
  - [Azure CLI](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli)
  - [Azure PowerShell Cmdlets](https://docs.microsoft.com/en-us/powershell/azure/install-azurerm-ps)
- CLI within Web Interface
  - [Azure Cloud Shell (Bash)](https://shell.azure.com/bash)
  - [Azure Cloud Shell (PowerShell)](https://shell.azure.com/powershell)

### Azure Portal

Build, manage, and monitor everything from simple web apps to complex cloud applications in a single, unified console.

Manage your resources via a web interface (i.e. GUI) at [https://portal.azure.com/](https://portal.azure.com/)

The Azure Portal is a great tool for quick prototyping, proof of concepts, and testing things out in Azure by deploying resources manually. However, when deploying production resources to Azure, it is highly recommended that you use an automation tool, templates, or scripts instead of the portal.

### Azure CLI

The Azure CLI is a cross-platform command-line tool providing a great experience for managing Azure resources. The CLI is designed to make scripting easy, query data in flexible ways, support long-running operations as non-blocking processes, and more. It is available on Windows, Mac, and Linux.

The Azure CLI will be the preferred (and supported) approach for this event, so please install the Azure CLI on your workstation. If you are not able to install the Azure CLI, or are using a workstation that is not your own, you can use the Azure CLI in the browser via the Azure Cloud Shell from the Azure Portal.

For Windows users, see the note below about how & where to install the Azure CLI!

- [Install on Windows](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli-windows?view=azure-cli-latest)
- [Install on macOS](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli-macos?view=azure-cli-latest)
- Install on Linux or Windows Subsystem for Linux (WSL)
  - [Install with apt on Debian or Ubuntu](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli-apt?view=azure-cli-latest)
  - [Install with yum on RHEL, Fedora, or CentOS](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli-yum?view=azure-cli-latest)
  - [Install from script](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli-linux?view=azure-cli-latest)
- [Run in Docker container](https://docs.microsoft.com/en-us/cli/azure/run-azure-cli-docker?view=azure-cli-latest)

### Azure Cloud Shell

The Azure Cloud Shell is a free interactive Bash or PowerShell shell that you can use to run the Azure CLI or PowerShell Cmdlets needed to complete the hackathon challenges. It has common Azure tools pre-installed and configured to use with your account. Just click the **Copy** button to copy the code, paste it into the Cloud Shell, and then press enter to run it. There are a few ways to launch the Cloud Shell:

|                                                                                                                  |                                                                                           |
| ---------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| Click **Try It** in the upper right corner of a code block.                                                      | ![Cloud Shell in this article](images/try-it-button.png)                                  |
| Click the **Cloud Shell** button on the menu in the upper right of the [Azure portal](https://portal.azure.com). | [![https://portal.azure.com/](images/portal-shell-button.png)](https://portal.azure.com/) |
| Open Cloud Shell in your browser.                                                                                | [Open Cloud Shell in the browser](https://shell.azure.com/bash)                           |
|                                                                                                                  |                                                                                           |

**NOTE:** If you use the Azure CLI or PowerShell from the Azure Cloud Shell, you will need to copy the template files you will be creating and editing on your workstation during the hackathon to the Cloud Shell environment.

## Visual Studio Code

Visual Studio Code is a lightweight but powerful source code editor which runs on your desktop and is available for Windows, macOS and Linux. It comes with built-in support for JavaScript, TypeScript and Node.js and has a rich ecosystem of extensions for other languages (such as C++, C#, Java, Python, PHP, Go) and runtimes (such as .NET and Unity).

[Install Visual Studio Code](https://code.visualstudio.com/)

VS Code runs on Windows, Mac, and Linux. It's a quick install, NOT a 2 hour install like its namesake full-fledged IDE on Windows.

## Azure Storage Explorer

Azure Storage Explorer is a cross-platform tool that lets you manage and access Azure Storage account resources in a GUI similar to Windows File Explorer or Finder on Mac. Like VS Code, Azure Storage Explorer can be installed on Windows, Mac, or Linux.

ARM templates and any resources they depend on (nested templates, script files, etc) need to be staged in a location where the Azure Resource Manager can access them via an HTTP endpoint. We will be using Azure Storage explorer during the hackathon to copy files to/from Azure Blob storage for staging purposes.

[Install Azure Storage Explorer](https://azure.microsoft.com/en-us/features/storage-explorer/)
