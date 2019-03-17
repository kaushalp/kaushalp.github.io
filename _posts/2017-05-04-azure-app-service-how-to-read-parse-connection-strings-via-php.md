---
id: 1595
title: 'Azure App Service: How to read &#038; parse connection strings via PHP'
date: 2017-05-04T13:20:52+00:00
author: kaushal
layout: post
guid: https://blogs.msdn.microsoft.com/kaushal/?p=1595
permalink: /2017/05/04/azure-app-service-how-to-read-parse-connection-strings-via-php/
opengraph_tags:
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Azure App Service: How to read &amp; parse connection strings via PHP" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2017/05/04/azure-app-service-how-to-read-parse-connection-strings-via-php/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="On Azure App Service, developers have the ability to configure the connection strings as key-value pair under App Settings section. Here is a sample screenshot: At runtime, Azure App Service retrieves this key-value pair for you and makes them available to your hosted application. These are provided to the web app as Environment Variables. Here..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2017/05/image_thumb52.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Azure App Service: How to read &amp; parse connection strings via PHP" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2017/05/04/azure-app-service-how-to-read-parse-connection-strings-via-php/" />
    <meta name="twitter:description" content="On Azure App Service, developers have the ability to configure the connection strings as key-value pair under App Settings section. Here is a sample screenshot: At runtime, Azure App Service retrieves this key-value pair for you and makes them available to your hosted application. These are provided to the web app as Environment Variables. Here..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2017/05/image_thumb52.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Azure App Service: How to read &amp; parse connection strings via PHP" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2017/05/04/azure-app-service-how-to-read-parse-connection-strings-via-php/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="On Azure App Service, developers have the ability to configure the connection strings as key-value pair under App Settings section. Here is a sample screenshot: At runtime, Azure App Service retrieves this key-value pair for you and makes them available to your hosted application. These are provided to the web app as Environment Variables. Here..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2017/05/image_thumb52.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Azure App Service: How to read &amp; parse connection strings via PHP" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2017/05/04/azure-app-service-how-to-read-parse-connection-strings-via-php/" />
    <meta name="twitter:description" content="On Azure App Service, developers have the ability to configure the connection strings as key-value pair under App Settings section. Here is a sample screenshot: At runtime, Azure App Service retrieves this key-value pair for you and makes them available to your hosted application. These are provided to the web app as Environment Variables. Here..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2017/05/image_thumb52.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Azure App Service: How to read &amp; parse connection strings via PHP" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2017/05/04/azure-app-service-how-to-read-parse-connection-strings-via-php/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="On Azure App Service, developers have the ability to configure the connection strings as key-value pair under App Settings section. Here is a sample screenshot: At runtime, Azure App Service retrieves this key-value pair for you and makes them available to your hosted application. These are provided to the web app as Environment Variables. Here..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2017/05/image_thumb52.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Azure App Service: How to read &amp; parse connection strings via PHP" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2017/05/04/azure-app-service-how-to-read-parse-connection-strings-via-php/" />
    <meta name="twitter:description" content="On Azure App Service, developers have the ability to configure the connection strings as key-value pair under App Settings section. Here is a sample screenshot: At runtime, Azure App Service retrieves this key-value pair for you and makes them available to your hosted application. These are provided to the web app as Environment Variables. Here..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2017/05/image_thumb52.png" />
    
categories:
  - App Settings
  - Azure App Service
  - Azure Web App
  - Azure Websites
  - Connection Strings
  - PHP
---
On **Azure App Service**, developers have the ability to configure the connection strings as key-value pair under **App Settings** section. Here is a sample screenshot:

> [<img title="image" style="padding-top: 0px;padding-left: 0px;padding-right: 0px;border-width: 0px" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/2017/05/image_thumb52.png" width="718" height="244" />](https://msdnshared.blob.core.windows.net/media/2017/05/image49.png)

At runtime, **Azure App Service** retrieves this key-value pair for you and makes them available to your hosted application. These are provided to the web app as **Environment Variables**.

Here is a good article on how to these work internally: [How Application Strings and Connection Strings Work](https://azure.microsoft.com/en-in/blog/windows-azure-web-sites-how-application-strings-and-connection-strings-work/ "https://azure.microsoft.com/en-in/blog/windows-azure-web-sites-how-application-strings-and-connection-strings-work/")

Here is a sample code on how to read the app settings in PHP



<span style="font-size: medium"><strong>Summary</strong></span>

The sample code is a way to get started on how to retrieve the connection strings at runtime in PHP. I have used the above sample to read from a database and display it on a page. The project is hosted on GitHub. See here: [https://github.com/kaushalp/Problematique/edit/master/ProblematicMvc/client.php](https://github.com/kaushalp/Problematique/edit/master/ProblematicMvc/client.php "https://github.com/kaushalp/Problematique/edit/master/ProblematicMvc/client.php")