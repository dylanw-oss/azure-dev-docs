---
title: Select Azure app hosting for JavaScript
description: Hosting options and deployment scenarios include several services and tools for Azure. Publish your app and serve it on Azure.  
ms.topic: how-to
ms.date: 08/19/2021
ms.custom: seo-javascript-september2019, seo-javascript-october2019, devx-track-js, contperf-fy21q2
---

# Deploy and host your JavaScript apps on Azure

Hosting options and deployment scenarios include several services and tools for Azure. Azure has many options for hosting and many tools to help you move your app from a local or cloud repository to Azure. 

## Choose a recommended Azure host provider

Use the following table to select a hosting service for most common app needs. 

For a complete overview of different hosting options, see [Decision tree for Azure compute services](/azure/architecture/guide/technology-choices/compute-decision-tree) and the [Core Cloud Services - Azure compute options](/training/modules/intro-to-azure-compute) module.


| Service |App type supported| Suggested for |
|--|--|--|
|[*App service](/azure/app-service/overview) - **recommended**|Client, Server, Client/Server, API, Server-render|Host your app from code or a container. This allows you to **fully configure and manage the web server** without needing to manage the underlying environment.<br><br>[**Quickstart**: Create a Node.js web app in Azure](/azure/app-service/quickstart-nodejs?pivots=platform-linux)|
|[Static Web apps](/azure/static-web-apps/)|Static front-end, Pre-render, JAM-stack, Static front end with serverless APIs|Deploy and dynamically scale your **static client app and serverless APIs**.<br><br>[**Quickstart**: Building your first static site with Azure Static Web Apps](/azure/static-web-apps/getting-started?tabs=vanilla-javascript) |
|[Functions](/azure/azure-functions/)|Serverless APIs, triggered background processes|Host your **serverless API endpoints**. Azure provides many templates known as triggers to bootstrap common scenarios.<br><br>[**Quickstart**: Create a JavaScript function in Azure using Visual Studio Code](/azure/azure-functions/create-first-function-vs-code-node)|
|[Azure Web PubSub (Preview)](/azure/azure-web-pubsub/overview)|Sockets, real-time message.|Build real-time messaging web applications using WebSockets and the publish-subscribe pattern.<br><br>[**Quickstart**: Publish messages using the service SDK for the Azure Web PubSub instance](/azure/azure-web-pubsub/quickstart-use-sdk?tabs=javascript)|


## Host web apps with more control and flexibility

The following choices give you more control of your application environment. 

| Service | Suggested for |
|--|--|
|[Virtual Machines](/azure/virtual-machines) (VMs)|Full control of a Windows or Linux VM. [Find an endorsed Linux Distribution](/azure/virtual-machines/linux/endorsed-distros?toc=/azure/virtual-machines/linux/toc.json) or [learn how to find](/azure/virtual-machines/linux/cli-ps-findimage) Linux VM images in the Azure Marketplace.|
|[Container Instances](/azure/container-instances/)|Quickly set up a single container.|
|Multiple apps|Use an [App Service plan](/azure/app-service/overview-hosting-plans) running multiple [app services](/azure/app-service/). |  

## Ultimate control with microservices on Azure

For enterprise scale systems, use one of the following microservice platforms. 

| Service | Suggested for |
|--|--|
|[Kubernetes Service](/azure/aks/)|Deploy a production ready Kubernetes cluster in Azure.|
|[Service Fabric](/azure/service-fabric/)| A distributed systems platform that makes it easy to package, deploy, and manage scalable and reliable microservices and containers|

## Alternative web app hosting choices on Azure

These choices are tailored to specific use cases. 

| Service | Suggested for |
|--|--|
|[Storage](/azure/storage/blobs/storage-blob-static-website-how-to?tabs=azure-portal)|Azure Storage can also host a static web app. This is helpful if you need tight integration between robust Storage and your client application.|
|[Content Delivery Network](/azure/cdn/) (CDN)|Deliver pre-rendered websites. Cache static objects loaded from Azure Blob storage, a web application, or any publicly accessible web server, by using the closest point of presence (POP) server. Azure CDN can also accelerate dynamic content, which cannot be cached, by using various network and routing optimizations.|

## Next steps

* [Cofigure app settings](configure-web-app-settings.md)
