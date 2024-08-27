# Azure AI Contents Generation

## Introduction

In this demo, we will show you some marketing contents generation use case with Azure AI.

## Design

- Prepare various dataset(pdf, video, image, text)
- Preprocess each data type.
- Generate marketing content based on user's request(request is defined as prompt for GPT model)

## Prerequisites

- An Azure subscription. If you don't have an Azure subscription, [create a free account](https://aka.ms/AMLFree) before you begin.
- Azure AI Search resource, resource can be created via Azure Portal. [Read here](hhttps://learn.microsoft.com/eu-es/azure/search/search-create-service-portal)
- Azure OpenAI Service resource and model, recource can be created via Azure Portal. Model can be deployed via Azure OpenAI Studio. [Read here](https://learn.microsoft.com/eu-es/azure/ai-services/openai/how-to/create-resource?pivots=web-portal)
- Azure AI Vision resource, resource can be created via Azure Portal as multi-service resource for Azure AI services. [Read here](https://learn.microsoft.com/en-us/azure/ai-services/multi-service-resource?tabs=linux&pivots=azportal)
- Azure Storage Account and blob container, these can be created via Azure Portal. [Read here](https://learn.microsoft.com/eu-es/azure/storage/blobs/blob-containers-portal)
- Azure AI Document Intelligence resource, , recource can be created via Azure Portal. [Read here](https://learn.microsoft.com/en-us/azure/ai-services/document-intelligence/how-to-guides/use-sdk-rest-api?view=doc-intel-4.0.0&tabs=windows&pivots=programming-language-python)
- Once you have created above resources, you need to set `.env` and define the following variables. These variables can be found in Azure Portal and Azure OpenAI Studio.
  - `AZURE_OPENAI_ENDPOINT`
  - `AZURE_OPENAI_API_KEY`
  - `AZURE_OPENAI_DEPLOYMENT`
  - `AZURE_OPENAI_API_VERSION`
  - `AZURE_SEARCH_ENDPOINT`
  - `AZURE_SEARCH_ADMIN_KEY`
  - `AZURE_AI_VISION_ENDPOINT`
  - `AZURE_AI_VISION_API_KEY`
  - `AZURE_DOCUMENT_INTELLIGENCE_ENDPOINT`
  - `AZURE_DOCUMENT_INTELLIGENCE_KEY`
  - `BLOB_CONNECTION_STRING`
  - `BLOB_CONTAINER_NAME`