# Azure Cognitive Search .NET Samples

This repository contains C# sample code used in Azure Cognitive Search quickstarts, tutorials, and examples. All samples run on the shared (free) Azure Cognitive Search service.  

## Quickstart

This .NET Core console app uses the Azure Cognitive Search .NET SDK to create an index, load it with documents, and execute a few queries. The index is modeled on a subset of the Hotels dataset, reduced for readability and comprehension. Index definition and documents are included in the code.

## Create your first app

This MVC sample is a collection of projects that demonstrate a user experience using fictitious hotels data. The first project creates a basic search page. Additional projects build on the first, adding results handling, and typeahead. The index is pre-built and hosted so that you can focus on the application itself.

## Multiple data sources

This .NET Core console app uses Azure Cognitive Search indexers and the .NET SDK to import data from Azure Cosmos DB and Azure Blob storage, combing data from two sources into one search index.

## Backup and restore an index

This .NET Core console app uses the .NET SDK and Azure Cognitive Search REST API to backup an index (schema and documents) to your computer and then uses the stored back up to recreate the index in a target search service that you specify. This tool is useful if you want to move an index into a different pricing tier. For example, you may use the Basic or Free pricing tier to develop your index, and then want to move it to the Standard or higher tier for production use. You can also use it to backup the index to your computer, so you can restore it at a later time, if needed.

**IMPORTANT** Search indexes are different from other datastores because they are constantly ranking and scoring results and data may shift. It is possible to miss some data during data extraction. This sample code also only works for indexes with less than 100,000 documents. However, it can be amended for larger indexes. See the README in the index-backup-restore folder for more details.

