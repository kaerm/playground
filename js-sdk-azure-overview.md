---
title: Azure SDK for JavaScript
description: Overview of the features and capabilities of the Azure SDK for JavaScript that helps developers be more productive when working with Azure services.
author: kraigb
ms.author: kraigb
manager: barbkess
ms.service: multiple
ms.date: 10/30/2019
ms.topic: conceptual
ms.devlang: javascript
---

# Azure SDK for JavaScript

The Azure SDK for JavaScript simplifies using and managing Azure resources from JavaScript application code.

You install the SDK by installing any of its individual component libraries by using `npm install @azure/<library>`. You can see the list of libraries on the [Azure SDK for JavaScript package index](https://github.com/Azure/azure-sdk-for-js/blob/master/packages.md).


> [!TIP]
> For information on changes in the SDK, see the [SDK release notes](https://azure.github.io/azure-sdk/).

## Connect and use Azure services

A number of *client libraries* in the SDK help you connect to existing Azure resources and use them in your apps, such as uploading files, accessing table data, or working with the various Azure Cognitive Services. With the SDK you work with those resources using familiar JavaScript programming paradigms rather than using the service's generic REST API.

For example, suppose you want to upload a blob to an Azure Storage account that you've previously provisioned. The first step is to install the appropriate library:

```bash
npm install @azure/storage-blob
```

Next, import the library in your code:

```js
[MISSING INFO]
```

Finally, use the library's API to connect to and upload the data. In this example, the connection string and container name are already provisioned in your storage account. The blob name is the name you assign to the uploaded data:

```js
[MISSING INFO]
```

For details on working with each specific library, see the *README.md* or *README.rst* file located in the library's project folder in our [GitHub repository](https://github.com/Azure/azure-sdk-for-js/tree/master/sdk). Also refer to the available [Azure Samples](https://docs.microsoft.com/en-us/samples/browse/?languages=javascript%2Cnodejs).

You can also find additional code snippets in the [reference documentation](javascript/api/overview/azure/?view=azure-node-latest)

### The Azure Core library

We are currently updating our JavaScript client libraries to share core functionality such as retries, logging, transport protocols, authentication protocols, etc. This shared functionality is contained in the [azure-core](https://github.com/Azure/azure-sdk-for-js/tree/master/sdk/core/) libraries. For details on the library and its guidelines, see the [JavaScript Guidelines: Introduction](https://azure.github.io/azure-sdk/typescript_introduction.html).

The libraries that currently work with the Core library are as follows:

- `@azure/storage-blob`
- `@azure/storage-queue`
- `@azure/keyvault-keys`
- `@azure/keyvault-secrets`

## Manage Azure resources

The Azure SDK for JavaScript also includes many libraries to help you create, provision, and otherwise manage Azure resources themselves. We refer to these as *management libraries*. Each management library is named `@azure/arm-<service name>`. With the management libraries, you can write JavaScript code to accomplish the same tasks that you can using the [Azure portal](https://portal.azure.com) or the [Azure CLI](https://docs.microsoft.com/cli/azure/install-azure-cli).

For example, suppose you want to create a SQL Server instance. First, install the appropriate management library:

```bash
npm install @azure/arm-sql
```

In your JavaScript code, import the library:

```js
[MISSING INFO]

```

Next, create the management client object using your credentials and Azure subscription ID:

```js
[MISSING INFO]
```

Finally, use that client object to create the resource, using an appropriate resource group name, server name, location, and administrator credentials:

```node
[MISSING INFO]
```

As with the client libraries, you can find details on working with each management library in the *README.md* or *README.rst* file located in the library's project folder in our [GitHub repository](https://github.com/Azure/azure-sdk-for-js/tree/master/sdk).

You can also find additional code snippets in the [reference documentation](/javascript/api/overview/azure/?view=azure-node-latest).

## Get help and give feedback

- Visit the [Azure SDK for JavaScript documentation](https://aka.ms/js-docs)
- Post questions to the community on [Stack Overflow](https://stackoverflow.com/questions/tagged/azure-sdk-js)
- Open issues against the SDK on [GitHub](https://github.com/Azure/azure-sdk-for-js/issues)
- Tweet at [@AzureSDK](https://twitter.com/AzureSdk/)