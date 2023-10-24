# ukgovaihackathon

# Prerequisites - Ready, Set, GO!

## Introduction

Thank you for participating in the Cross Government Generative AI Hack. Before you can hack, you will need to set up some prerequisites.

## Common Prerequisites

We have compiled a list of common tools and software that will come in handy to complete most Azure-based hacks!

You might not need all of them for the hack you are participating in. However, if you work with Azure on a regular basis, these are all things you should consider having in your toolbox.

- [Azure Environment](000-HowToHack/Common-Prerequisites.md#azure-environment)
- [Windows Subsystem for Linux](000-HowToHack/Common-Prerequisites.md#windows-subsystem-for-linux)
- [Managing Cloud Resources](000-HowToHack/Common-Prerequisites.md#managing-cloud-resources)
  - [Azure Portal](000-HowToHack/Common-Prerequisites.md#azure-portal)
  - [Azure CLI](000-HowToHack/Common-Prerequisites.md#azure-cli)
    - [Note for Windows Users](000-HowToHack/Common-Prerequisites.md#note-for-windows-users)
    - [Azure PowerShell CmdLets](000-HowToHack/Common-Prerequisites.md#azure-powershell-cmdlets)
  - [Azure Cloud Shell](000-HowToHack/Common-Prerequisites.md#azure-cloud-shell)
- [Visual Studio Code](https://code.visualstudio.com/)
- [Azure Storage Explorer](https://azure.microsoft.com/en-us/products/storage/storage-explorer/)


## Hack Environment

A hacking environment has been made available to you. 

For a diagram of the architecture of the environment see [Azure Environment Diagram](https://azurediagrams.com/fc5Q6FTZ)
Feel free to use this diagram in your hack solution to describe your resources and architecture.


Each team will be designated a team name, which will be used to tag resources for you to work with.

## Shared Resources
For each team, the following **shared** resources have been created within a pre-configured Azure Tenant:
- Azure OpenAI Service model deployments:
  - gpt-35-turbo-16k
  - text-embedding-ada-002
- Azure Machine Learning Service

## Per-team Resource Group
  Within your team's Resource Group, you are able to create the Azure Services you require to host resources and solutions for your hack (i.e. storage accounts, Cosmos DB etc.)

## Access to the Tenant
To access the Azure Tenant you will have been assigned a Microsoft Account (MSA) and a temporary password

Please have the developers in your team complete the following steps to access the Azure Tenant:
- Once onboarded please confirm you are able to access
  - Azure Tenant (https://portal.azure.com)
  - Azure ML Workspace (https://ml.azure.com/home?tid=3b707db1-4728-46ea-a4c5-c690d2c28113)

## Azure ML Workspace 
- Your team will be able to create a notebook within the shared Azure Machine Learning Studio Workspace
- Please prefix the notebook with your team name


## Accessing Azure OpenAI Service
- Within your team's workspace you will be able to access the Azure OpenAI Service, via an API Call. 
  - A Sample Notebook demonstrating this can be found here [AOAI Sample Notebook](https://ml.azure.com/fileexplorerAzNB?wsid=/subscriptions/9e6f9ad9-f736-42de-97f2-0fa34e6314ce/resourcegroups/genai-workspace-xfpdf-rg/providers/Microsoft.MachineLearningServices/workspaces/genai-ws-xfpdf&tid=3b707db1-4728-46ea-a4c5-c690d2c28113&activeFilePath=Users/luked/AOAI_Test.ipynb)
  
  - Amend the Sample Notebook to use your teamname in the API call to:
    - apim_gateway_url = 'https://aoaiapim.azure-api.net'
    - team_name = 'TeamName'

Within your notebook, you will be be able to attach to a compute instance and work with AOAI APIs set up in the Azure Tenant and/or call services setup within your team Resource Group.


## Success Criteria

## Learning Resources
- Azure OpenAI Service API
  - [Sample notebook](https://ml.azure.com/fileexplorerAzNB?wsid=/subscriptions/9e6f9ad9-f736-42de-97f2-0fa34e6314ce/resourcegroups/genai-workspace-xfpdf-rg/providers/Microsoft.MachineLearningServices/workspaces/genai-ws-xfpdf&tid=3b707db1-4728-46ea-a4c5-c690d2c28113&activeFilePath=Users/luked/AOAI_Test.ipynb)

- Azure Machine Learning
  - [Documentation](https://learn.microsoft.com/en-us/azure/machine-learning/?view=azureml-api-2)
  - [How to use Azure OpenAI models in Azure Machine Learning](https://learn.microsoft.com/en-us/azure/machine-learning/how-to-use-openai-models-in-azure-ml?view=azureml-api-2)
  - [Creating Azure Machine Learning Data Stores](https://learn.microsoft.com/en-us/azure/machine-learning/how-to-datastore?view=azureml-api-2&tabs=sdk-identity-based-access%2Csdk-adls-identity-access%2Csdk-azfiles-accountkey%2Csdk-adlsgen1-identity-access)
  - [Retrevial Augmented Generation using Prompt Flow](https://learn.microsoft.com/en-us/azure/machine-learning/concept-retrieval-augmented-generation?view=azureml-api-2)

- Cognitive Services
  - [Documentation](https://www.microsoft.com/cognitive-services)
- Cosmos DB
  - [Documentation](https://docs.microsoft.com/en-us/azure/cosmos-db)
- Azure Search
  - [Documentation](https://azure.microsoft.com/en-us/services/search)
