# Azure AI Foundry: Image Generation with Black Forest Labs' FLUX models

This repo demonstrates how to use **FLUX** image-generation models from _Black Forest Labs_ in Azure AI Foundry. The provided Jupyter notebook showcases how to create high-quality images from textual prompts.

This demo utilises the `requests` library for direct API interaction and the `azure-identity` library for secure Azure Entra ID authentication.

## 📑 Table of Contents:
- [Part 1: Configuring Solution Environment](#part-1-configuring-solution-environment)
- [Part 2: Generating Images with FLUX Models](#part-2-generating-images-with-flux-models)
- [Part 3: Model Comparison - V1.1 Pro vs. V2 Pro]()

## Part 1: Configuring Solution Environment
To use the notebook, set up your Azure AI Foundry environment and install the necessary Python packages.

### 1.1 Azure AI Foundry Setup
Ensure you have an Azure AI Foundry project with the FLUX-1.1-pro or FLUX-2-pro models deployed.

### 1.2 Authentication
This demo uses **Azure Entra ID** authentication via `DefaultAzureCredential` from `azure.identity`. This credential type automatically handles various authentication methods.

To make it work, ensure your environment is set up for Azure authentication, e.g., by logging in via `az login` (Azure CLI) or setting relevant environment variables for service principals.

> [!NOTE]
> More detailed information about supported credential types can be found [here](https://learn.microsoft.com/en-us/dotnet/api/azure.identity.defaultazurecredential).

### 1.3 Environment Variables
Set the following environment variables to point to your Azure AI Foundry endpoint and deployments:

| Environment Variable       |  Description                                                                               |
| -------------------------- | ------------------------------------------------------------------------------------------ |
| AZURE_FOUNDRY_ENDPOINT_BFL | Your Azure AI Foundry endpoint URL (e.g., https://<YOUR_RESOURCE>.services.ai.azure.com/). |
| FLUX_v1_DEPLOYMENT         | The name of your FLUX 1.1 Pro deployment.                                                  |
| FLUX_v2_DEPLOYMENT         | The name of your FLUX 2 Pro deployment.                                                    |

### 1.4 Install Required Python packages

``` PowerShell
pip install requests pillow azure-identity
```

## Part 2: Generating Images with FLUX Models



## Part 3: Model Comparison - V1.1 Pro vs. V2 Pro

