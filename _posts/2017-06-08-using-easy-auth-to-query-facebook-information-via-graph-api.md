---
id: 1845
title: 'Azure App Service: Using Easy Auth to query Facebook information via Graph API'
date: 2017-06-08T03:12:32+00:00
author: kaushal
layout: post
guid: https://blogs.msdn.microsoft.com/kaushal/?p=1845
permalink: /2017/06/08/using-easy-auth-to-query-facebook-information-via-graph-api/
opengraph_tags:
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Azure App Service: Using Easy Auth to query Facebook information via Graph API" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2017/06/08/using-easy-auth-to-access-facebook-information-using-graph-api/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="On 8th August 2016, Facebook ended support FQL (Facebook Query Language). Here is a screenshot of the messaging from their site Facebook Query Language (FQL) Reference So they are encouraging the developers to use the GraphAPI to query the information. In this post we will cover on how to do this. Pre-Requisites Create an Azure..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2017/06/image_thumb192.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Azure App Service: Using Easy Auth to query Facebook information via Graph API" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2017/06/08/using-easy-auth-to-access-facebook-information-using-graph-api/" />
    <meta name="twitter:description" content="On 8th August 2016, Facebook ended support FQL (Facebook Query Language). Here is a screenshot of the messaging from their site Facebook Query Language (FQL) Reference So they are encouraging the developers to use the GraphAPI to query the information. In this post we will cover on how to do this. Pre-Requisites Create an Azure..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2017/06/image_thumb192.png" />
    
categories:
  - accesstoken
  - Authentication
  - Authentication/Authorization
  - Authorization
  - Azure
  - Azure App Service
  - Azure Web App
  - Azure Websites
  - Easy Auth
  - facebook
  - FQL
  - Graph Api
  - Web App
  - X-MS-TOKEN-FACEBOOK-ACCESS-TOKEN
---
<span style="font-size: small">On 8th August 2016, Facebook ended support <strong>FQL</strong> (<em>Facebook Query Language</em>). Here is a screenshot of the messaging from their site </span>[<span style="font-size: small">Facebook Query Language (FQL) Reference</span>](https://developers.facebook.com/docs/reference/fql/ "https://developers.facebook.com/docs/reference/fql/")

> [<span style="font-size: small"><img title="image" style="padding-top: 0px;padding-left: 0px;padding-right: 0px;border-width: 0px" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/2017/06/image_thumb192.png" width="721" height="108" /></span>](https://msdnshared.blob.core.windows.net/media/2017/06/image192.png)

#### <span style="font-size: small">So they are encouraging the developers to use the GraphAPI to query the information. In this post we will cover on how to do this.</span>

#### <span style="font-family: 'Segoe UI Semibold'">Pre-Requisites</span>

  * <span style="font-size: small">Create an Azure Web App and configure <strong>Facebook </strong>Authentication. This will require creating a “<strong>App ID</strong>” & “<strong>App Secret</strong>”. Refer this </span>[<span style="font-size: small">link</span>](https://docs.microsoft.com/en-us/azure/app-service-mobile/app-service-mobile-how-to-configure-facebook-authentication) <span style="font-size: small">on on how to do this.</span>
  * <span style="font-size: small">In the Azure Portal, under <strong>Facebook Authentication Settings </strong>select the <em>scopes </em>(or <em>permissions</em>) to access the required data.</span>
  * <span style="font-size: small">I created a ASP.NET MVC 5 application with default authentication set to <strong>Individual User Accounts</strong>.</span>

### Determining the scopes required to query the facebook data

### <span style="font-size: small">Facebook provides <a target="_blank" href="https://developers.facebook.com/tools/explorer/" rel="noopener noreferrer">Graph API Explorer</a>, which allows the users to test, create and debug their graph API calls. Using this the users can generate a <span style="font-weight: bold">accesstoken </span>with specific scope. Using this token, the users can call the Facebook GraphApi and review the results right there.</span>

### <span style="font-size: small">Here is a screenshot of the UI:</span>

> ### [<img title="image" style="padding-top: 0px;padding-left: 0px;padding-right: 0px;border: 0px" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/2017/06/image_thumb194.png" width="909" height="527" />](https://msdnshared.blob.core.windows.net/media/2017/06/image194.png)<span style="font-size: small"></span>
> 
> ### <span style="font-size: small">Once you have understood, the scopes and parameters you need to pass when calling the Facebook graph Api, we can start working on building the web application.</span>

### Create a Function to call an external Endpoint

The below **<span style="background-color: #cccccc;font-family: 'Courier New'">RequestResponse()</span> <span></span>**<span style="background-color: #cccccc;font-family: 'Courier New'"></span>method takes an URL as input. Using the **HttpWebRequest** method, we call the URL and return the response. 

<span style="font-size: small"></span>

### Calling the Facebook Graph Api

The below <span style="background-color: #cccccc;font-family: 'Courier New'"><strong>CallFacebookGraphApi()</strong></span> method code takes 3 inputs, all of which are of type string.

  1. **id** – This is the path that will be called. For example “me/feed”
  2. **fields** – this is the query string parameters that needs to be provided with the **id** above.
  3. **accesstoken** – this is the value of the “**X-MS-TOKEN-FACEBOOK-ACCESS-TOKEN**” header, that gets generated upon successful user login. This is used to authorize the GraphAPI call.

using the above 3 parameters we create a URL and call the **<span style="background-color: #cccccc;font-family: 'Courier New'">RequestResponse()</span>** method we created earlier.



### Fetching results from Facebook

Here we have a **ActionResult** Facebook, where we pass the parameters to the <span style="background-color: #cccccc;font-family: 'Courier New'"><strong>CallFacebookGraphApi()</strong></span> method we created above.

  
I have deployed a working version of the code on one of my web apps (**Azure App Service**). You can see the it working here: [https://easyauthkaushal-staging.azurewebsites.net](https://easyauthkaushal-staging.azurewebsites.net "https://easyauthkaushal-staging.azurewebsites.net")

This code is published on Github. You may fork it here: [https://github.com/kaushalp/Facebook-GraphApi-with-EasyAuth](https://github.com/kaushalp/Facebook-GraphApi-with-EasyAuth "https://github.com/kaushalp/Facebook-GraphApi-with-EasyAuth")

HTH,  
Kaushal