---
services: cognitive-services
author: aahill
manager: nitinme
ms.service: cognitive-services
ms.subservice: language-service
ms.custom: event-tier1-build-2022
ms.topic: include
ms.date: 06/07/2022
ms.author: aahi
---

## Prerequisites

* Azure subscription - [Create one for free](https://azure.microsoft.com/free/cognitive-services)

> [!div class="nextstepaction"]
> <a href="https://microsoft.qualtrics.com/jfe/form/SV_0Cl5zkG3CnDjq6O?PLanguage=Language-studio&Pillar=Language&Product=Custom-named-entity-recognition&Page=quickstart&Section=Prerequisites" target="_target">I ran into an issue</a>

## Create a new Azure Language resource and Azure storage account

Before you can use custom NER, you'll need to create an Azure Language resource, which will give you the credentials that you need to create a project and start training a model. You'll also need an Azure storage account, where you can upload your dataset that will be used to build your model.

> [!IMPORTANT]
> To quickly get started, we recommend creating a new Azure Language resource using the steps provided in this article. Using the steps in this article will let you create the Language resource and storage account at the same time, which is easier than doing it later.
>
> If you have a pre-existing resource that you'd like to use, you will need to connect it to storage account. See [guidance to using a pre-existing resource](../../how-to/create-project.md#using-a-pre-existing-language-resource) for information.

[!INCLUDE [create a new resource from the Azure portal](../resource-creation-azure-portal.md)]

> [!div class="nextstepaction"]
> <a href="https://microsoft.qualtrics.com/jfe/form/SV_0Cl5zkG3CnDjq6O?PLanguage=Language-studio&Pillar=Language&Product=Custom-named-entity-recognition&Page=quickstart&Section=Create-a-new-azure-language-resource-and-storage-account" target="_target">I ran into an issue</a>

## Upload sample data to blob container

[!INCLUDE [Uploading sample data for custom NER](blob-storage-upload.md)]

> [!div class="nextstepaction"]
> <a href="https://microsoft.qualtrics.com/jfe/form/SV_0Cl5zkG3CnDjq6O?PLanguage=Language-studio&Pillar=Language&Product=Custom-named-entity-recognition&Page=quickstart&Section=Upload-sample-data-to-blob-container" target="_target">I ran into an issue</a>

## Create a custom named entity recognition project

Once your resource and storage account are configured, create a new custom NER project. A project is a work area for building your custom ML models based on your data. Your project can only be accessed by you and others who have access to the Language resource being used.

[!INCLUDE [Create custom NER project](../language-studio/create-project.md)]

> [!div class="nextstepaction"]
> <a href="https://microsoft.qualtrics.com/jfe/form/SV_0Cl5zkG3CnDjq6O?PLanguage=Language-studio&Pillar=Language&Product=Custom-named-entity-recognition&Page=quickstart&Section=Create-custom-named-entity-recognition-project" target="_target">I ran into an issue</a>

## Train your model

Typically after you create a project, you go ahead and start [tagging the documents](../../how-to/tag-data.md) you have in the container connected to your project. For this quickstart, you have imported a sample tagged dataset and initialized your project with the sample JSON tags file.

[!INCLUDE [Train a model using Language Studio](../language-studio/train-model.md)]

> [!div class="nextstepaction"]
> <a href="https://microsoft.qualtrics.com/jfe/form/SV_0Cl5zkG3CnDjq6O?PLanguage=Language-studio&Pillar=Language&Product=Custom-named-entity-recognition&Page=quickstart&Section=Train-model" target="_target">I ran into an issue</a>

## Deploy your model

Generally after training a model you would review its [evaluation details](../../how-to/view-model-evaluation.md) and [make improvements](../../how-to/view-model-evaluation.md) if necessary. In this quickstart, you will just deploy your model, and make it available for you to try in Language studio, or you can call the [prediction API](https://aka.ms/ct-runtime-swagger).

[!INCLUDE [Deploy a model using Language Studio](../language-studio/deploy-model.md)]

> [!div class="nextstepaction"]
> <a href="https://microsoft.qualtrics.com/jfe/form/SV_0Cl5zkG3CnDjq6O?PLanguage=Language-studio&Pillar=Language&Product=Custom-named-entity-recognition&Page=quickstart&Section=Deploy-model" target="_target">I ran into an issue</a>


## Test your model

After your model is deployed, you can start using it to extract entities from your text via [Prediction API](https://aka.ms/ct-runtime-swagger). For this quickstart, you will use the [Language Studio](https://aka.ms/LanguageStudio) to submit the custom entity recognition task and visualize the results. In the sample dataset you downloaded earlier, you can find some test documents that you can use in this step.

[!INCLUDE [Test a model using Language Studio](../language-studio/test-model.md)]

> [!div class="nextstepaction"]
> <a href="https://microsoft.qualtrics.com/jfe/form/SV_0Cl5zkG3CnDjq6O?PLanguage=Language-studio&Pillar=Language&Product=Custom-named-entity-recognition&Page=quickstart&Section=Test-model" target="_target">I ran into an issue</a>

## Clean up resources

[!INCLUDE [Delete project using Language Studio](../language-studio/delete-project.md)]

> [!div class="nextstepaction"]
> <a href="https://microsoft.qualtrics.com/jfe/form/SV_0Cl5zkG3CnDjq6O?PLanguage=Language-studio&Pillar=Language&Product=Custom-named-entity-recognition&Page=quickstart&Section=Clean-up-projects" target="_target">I ran into an issue</a>
