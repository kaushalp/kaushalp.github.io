---
id: 1021
title: 'Azure Web Apps: How to retrieve user email in the claim when using Microsoft Account as a provider in Easy Auth'
date: 2016-04-01T16:03:13+00:00
author: kaushal
layout: post
guid: https://blogs.msdn.microsoft.com/kaushal/?p=1021
permalink: /2016/04/01/azure-web-apps-how-to-retrieve-user-email-in-the-claim-when-using-microsoft-account-as-a-provider-in-easy-auth/
opengraph_tags:
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Azure Web Apps: How to retrieve user email in the claim when using Microsoft Account as a provider in Easy Auth" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2016/04/01/azure-web-apps-how-to-retrieve-user-email-in-the-claim-when-using-microsoft-account-as-a-provider-in-easy-auth/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="App Service Authentication/Authorization also known as Easy Auth is one of the widely used feature in Azure App Service. It reduces the burden on the developers and provides a way for the application to sign in users without changing code. It is implemented as a module and is injected at runtime within the app. It..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2016/04/image_thumb36.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Azure Web Apps: How to retrieve user email in the claim when using Microsoft Account as a provider in Easy Auth" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2016/04/01/azure-web-apps-how-to-retrieve-user-email-in-the-claim-when-using-microsoft-account-as-a-provider-in-easy-auth/" />
    <meta name="twitter:description" content="App Service Authentication/Authorization also known as Easy Auth is one of the widely used feature in Azure App Service. It reduces the burden on the developers and provides a way for the application to sign in users without changing code. It is implemented as a module and is injected at runtime within the app. It..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2016/04/image_thumb36.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Azure Web Apps: How to retrieve user email in the claim when using Microsoft Account as a provider in Easy Auth" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2016/04/01/azure-web-apps-how-to-retrieve-user-email-in-the-claim-when-using-microsoft-account-as-a-provider-in-easy-auth/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="App Service Authentication/Authorization also known as Easy Auth is one of the widely used feature in Azure App Service. It reduces the burden on the developers and provides a way for the application to sign in users without changing code. It is implemented as a module and is injected at runtime within the app. It..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2016/04/image_thumb36.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Azure Web Apps: How to retrieve user email in the claim when using Microsoft Account as a provider in Easy Auth" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2016/04/01/azure-web-apps-how-to-retrieve-user-email-in-the-claim-when-using-microsoft-account-as-a-provider-in-easy-auth/" />
    <meta name="twitter:description" content="App Service Authentication/Authorization also known as Easy Auth is one of the widely used feature in Azure App Service. It reduces the burden on the developers and provides a way for the application to sign in users without changing code. It is implemented as a module and is injected at runtime within the app. It..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2016/04/image_thumb36.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Azure Web Apps: How to retrieve user email in the claim when using Microsoft Account as a provider in Easy Auth" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2016/04/01/azure-web-apps-how-to-retrieve-user-email-in-the-claim-when-using-microsoft-account-as-a-provider-in-easy-auth/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="App Service Authentication/Authorization also known as Easy Auth is one of the widely used feature in Azure App Service. It reduces the burden on the developers and provides a way for the application to sign in users without changing code. It is implemented as a module and is injected at runtime within the app. It..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2016/04/image_thumb36.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Azure Web Apps: How to retrieve user email in the claim when using Microsoft Account as a provider in Easy Auth" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2016/04/01/azure-web-apps-how-to-retrieve-user-email-in-the-claim-when-using-microsoft-account-as-a-provider-in-easy-auth/" />
    <meta name="twitter:description" content="App Service Authentication/Authorization also known as Easy Auth is one of the widely used feature in Azure App Service. It reduces the burden on the developers and provides a way for the application to sign in users without changing code. It is implemented as a module and is injected at runtime within the app. It..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2016/04/image_thumb36.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Azure Web Apps: How to retrieve user email in the claim when using Microsoft Account as a provider in Easy Auth" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2016/04/01/azure-web-apps-how-to-retrieve-user-email-in-the-claim-when-using-microsoft-account-as-a-provider-in-easy-auth/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="App Service Authentication/Authorization also known as Easy Auth is one of the widely used feature in Azure App Service. It reduces the burden on the developers and provides a way for the application to sign in users without changing code. It is implemented as a module and is injected at runtime within the app. It..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2016/04/image_thumb36.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Azure Web Apps: How to retrieve user email in the claim when using Microsoft Account as a provider in Easy Auth" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2016/04/01/azure-web-apps-how-to-retrieve-user-email-in-the-claim-when-using-microsoft-account-as-a-provider-in-easy-auth/" />
    <meta name="twitter:description" content="App Service Authentication/Authorization also known as Easy Auth is one of the widely used feature in Azure App Service. It reduces the burden on the developers and provides a way for the application to sign in users without changing code. It is implemented as a module and is injected at runtime within the app. It..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2016/04/image_thumb36.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Azure Web Apps: How to retrieve user email in the claim when using Microsoft Account as a provider in Easy Auth" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2016/04/01/azure-web-apps-how-to-retrieve-user-email-in-the-claim-when-using-microsoft-account-as-a-provider-in-easy-auth/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="App Service Authentication/Authorization also known as Easy Auth is one of the widely used feature in Azure App Service. It reduces the burden on the developers and provides a way for the application to sign in users without changing code. It is implemented as a module and is injected at runtime within the app. It..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2016/04/image_thumb36.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Azure Web Apps: How to retrieve user email in the claim when using Microsoft Account as a provider in Easy Auth" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2016/04/01/azure-web-apps-how-to-retrieve-user-email-in-the-claim-when-using-microsoft-account-as-a-provider-in-easy-auth/" />
    <meta name="twitter:description" content="App Service Authentication/Authorization also known as Easy Auth is one of the widely used feature in Azure App Service. It reduces the burden on the developers and provides a way for the application to sign in users without changing code. It is implemented as a module and is injected at runtime within the app. It..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2016/04/image_thumb36.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Azure Web Apps: How to retrieve user email in the claim when using Microsoft Account as a provider in Easy Auth" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2016/04/01/azure-web-apps-how-to-retrieve-user-email-in-the-claim-when-using-microsoft-account-as-a-provider-in-easy-auth/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="App Service Authentication/Authorization also known as Easy Auth is one of the widely used feature in Azure App Service. It reduces the burden on the developers and provides a way for the application to sign in users without changing code. It is implemented as a module and is injected at runtime within the app. It..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2016/04/image_thumb36.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Azure Web Apps: How to retrieve user email in the claim when using Microsoft Account as a provider in Easy Auth" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2016/04/01/azure-web-apps-how-to-retrieve-user-email-in-the-claim-when-using-microsoft-account-as-a-provider-in-easy-auth/" />
    <meta name="twitter:description" content="App Service Authentication/Authorization also known as Easy Auth is one of the widely used feature in Azure App Service. It reduces the burden on the developers and provides a way for the application to sign in users without changing code. It is implemented as a module and is injected at runtime within the app. It..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2016/04/image_thumb36.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Azure Web Apps: How to retrieve user email in the claim when using Microsoft Account as a provider in Easy Auth" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2016/04/01/azure-web-apps-how-to-retrieve-user-email-in-the-claim-when-using-microsoft-account-as-a-provider-in-easy-auth/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="App Service Authentication/Authorization also known as Easy Auth is one of the widely used feature in Azure App Service. It reduces the burden on the developers and provides a way for the application to sign in users without changing code. It is implemented as a module and is injected at runtime within the app. It..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2016/04/image_thumb36.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Azure Web Apps: How to retrieve user email in the claim when using Microsoft Account as a provider in Easy Auth" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2016/04/01/azure-web-apps-how-to-retrieve-user-email-in-the-claim-when-using-microsoft-account-as-a-provider-in-easy-auth/" />
    <meta name="twitter:description" content="App Service Authentication/Authorization also known as Easy Auth is one of the widely used feature in Azure App Service. It reduces the burden on the developers and provides a way for the application to sign in users without changing code. It is implemented as a module and is injected at runtime within the app. It..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2016/04/image_thumb36.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Azure Web Apps: How to retrieve user email in the claim when using Microsoft Account as a provider in Easy Auth" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2016/04/01/azure-web-apps-how-to-retrieve-user-email-in-the-claim-when-using-microsoft-account-as-a-provider-in-easy-auth/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="App Service Authentication/Authorization also known as Easy Auth is one of the widely used feature in Azure App Service. It reduces the burden on the developers and provides a way for the application to sign in users without changing code. It is implemented as a module and is injected at runtime within the app. It..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2016/04/image_thumb36.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Azure Web Apps: How to retrieve user email in the claim when using Microsoft Account as a provider in Easy Auth" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2016/04/01/azure-web-apps-how-to-retrieve-user-email-in-the-claim-when-using-microsoft-account-as-a-provider-in-easy-auth/" />
    <meta name="twitter:description" content="App Service Authentication/Authorization also known as Easy Auth is one of the widely used feature in Azure App Service. It reduces the burden on the developers and provides a way for the application to sign in users without changing code. It is implemented as a module and is injected at runtime within the app. It..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2016/04/image_thumb36.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Azure Web Apps: How to retrieve user email in the claim when using Microsoft Account as a provider in Easy Auth" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2016/04/01/azure-web-apps-how-to-retrieve-user-email-in-the-claim-when-using-microsoft-account-as-a-provider-in-easy-auth/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="App Service Authentication/Authorization also known as Easy Auth is one of the widely used feature in Azure App Service. It reduces the burden on the developers and provides a way for the application to sign in users without changing code. It is implemented as a module and is injected at runtime within the app. It..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2016/04/image_thumb36.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Azure Web Apps: How to retrieve user email in the claim when using Microsoft Account as a provider in Easy Auth" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2016/04/01/azure-web-apps-how-to-retrieve-user-email-in-the-claim-when-using-microsoft-account-as-a-provider-in-easy-auth/" />
    <meta name="twitter:description" content="App Service Authentication/Authorization also known as Easy Auth is one of the widely used feature in Azure App Service. It reduces the burden on the developers and provides a way for the application to sign in users without changing code. It is implemented as a module and is injected at runtime within the app. It..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2016/04/image_thumb36.png" />
    
categories:
  - Uncategorized
tags:
  - accesstoken
  - Authentication/Authorization
  - Azure App Service
  - Easy Auth
  - email
  - User claim
  - Web Apps
  - WebSites
---
<span style="font-family: segoe ui"><span style="font-size: small"><a href="https://docs.microsoft.com/en-in/azure/app-service/app-service-authentication-overview?toc=%2fazure%2fapp-service-web%2ftoc.json"><strong>App Service Authentication/Authorization </strong></a>also known as<strong> Easy Auth</strong> is one of the widely used feature in <strong>Azure App Service</strong>. It reduces the burden on the developers and provides a way for the application to sign in users without changing code. It is implemented as a module and is injected at runtime within the app. It automates a lot of configuration which usually is a tedious task. It is a one time process where the users have to configure the web app to use one or more of the identity providers. Following is a list of providers currently supported with this module:<br /> </span></span>

  * <span style="font-family: segoe ui"><span style="font-size: small"><strong>Azure Active Directory (AAD)</strong> </span></span>
  * <span style="font-family: segoe ui"><span style="font-size: small"><strong>Facebook</strong> </span></span>
  * <span style="font-family: segoe ui"><span style="font-size: small"><strong>Google</strong> </span></span>
  * <span style="font-family: segoe ui"><span style="font-size: small"><strong>Twitter</strong> </span></span>
  * <span style="font-family: segoe ui"><span style="font-size: small"><strong>Microsoft Account (microsoftaccount)</strong> </span></span>

<span style="font-size: small;font-family: segoe ui">Refer the following article to configure your web application to use Microsoft account as the auth provider.<br /> </span>

<p style="padding-left: 30px">
  <a href="https://docs.microsoft.com/en-in/azure/app-service-mobile/app-service-mobile-how-to-configure-microsoft-authentication?toc=%2fazure%2fapp-service-web%2ftoc.json" title="https://azure.microsoft.com/en-us/documentation/articles/app-service-mobile-how-to-configure-microsoft-authentication/"><span style="font-size: small;font-family: segoe ui">How to configure your App Service application to use Microsoft Account login</span></a><span style="font-size: small;font-family: segoe ui"> </span>
</p>

<span style="font-size: small;font-family: segoe ui">Multiple providers can be configured for a single web app. For this, in portal set the</span>

<span style="font-size: small;font-family: segoe ui">&#8220;<strong>Action to take when request is not authenticated</strong>&#8220;<strong> </strong>= “<strong>Allow request (no action)</strong>”. </span>

<span style="font-size: small;font-family: segoe ui">This is also known as <strong>deferred authentication</strong>. In this case the providers from the app have to be called explicitly and the application will consume it based on the obtained claim. The following table illustrates the api endpoint which is used to invoke certain calls.  </span>

<table style="height: 110px;margin-left: 50px;background-color: #00bdff;border-style: solid;border-color: #0775BD" width="597" cellspacing="0" cellpadding="0" border="3">
  <tr>
    <td width="128" valign="top">
      <span style="font-size: small;font-family: segoe ui"><strong><span style="color: #ffffff"> <span style="color: #000000">Login End Point</span></span></strong></span>
    </td>
    
    <td width="465">
        <span style="font-size: small;font-family: consolas;color: #0000ff;background-color: #ffffff"><span style="color: #000000">/.auth/login/</span><span style="color: #c0504d"><provider><span style="font-family: Consolas;font-size: small"> </span></span></span>
    </td>
  </tr>
  
  <tr>
    <td width="132" valign="top">
    </td>
    
    <td width="472" valign="top">
      <span style="font-size: small;font-family: segoe ui">  <span style="font-family: consolas;color: #0000ff;background-color: #ffffff"><span style="color: #000000">/.auth/login/</span><span style="color: #c0504d"><provider<span style="color: #000000">></span></span><span style="color: #000000">?post_login_redirect_uri=</span><span style="color: #c0504d"><url-path><span style="font-family: Consolas;font-size: small"> </span></span></span></span>
    </td>
  </tr>
  
  <tr>
    <td width="133" valign="top">
      <span style="font-size: small;font-family: segoe ui"><strong><span style="color: #ffffff"> <span style="color: #000000">Logout End point</span></span></strong></span>
    </td>
    
    <td width="473" valign="top">
        <span style="color: #000000;font-family: consolas;font-size: small;background-color: #ffffff">/.auth/logout<span style="font-family: Consolas;font-size: small"> </span></span>
    </td>
  </tr>
  
  <tr>
    <td width="134" valign="top">
    </td>
    
    <td width="473" valign="top">
      <span style="font-size: small;font-family: segoe ui">  <span style="font-family: consolas;color: #0000ff;background-color: #ffffff"><span style="color: #000000">/.auth/logout?post_logout_redirect_uri</span><span style="color: #c0504d"><span style="color: #000000">=</span><url-path><span style="font-family: Consolas;font-size: small"> </span></span></span></span>
    </td>
  </tr>
  
  <tr>
    <td width="134" valign="top">
      <strong><span style="color: #ffffff;font-family: Segoe UI;font-size: small"> <span style="color: #000000">Token Access</span></span></strong>
    </td>
    
    <td width="473" valign="top">
        <span style="color: #000000;font-family: consolas;font-size: small;background-color: #ffffff">/.auth/me<span style="font-family: Consolas;font-size: small"> </span></span>
    </td>
  </tr>
</table>

<p style="padding-left: 30px">
  <span style="font-size: small;font-family: segoe ui"><strong><span style="font-family: consolas;color: #0000ff;background-color: #cccccc"><providers></span></strong> can be set to <strong>aad</strong>, <strong>facebook</strong>, <strong>google</strong>, <strong>twitter </strong>& <strong>microsoftaccount</strong>. Here is an example:</span>
</p>

<p style="padding-left: 30px">
  <a href="https://easyauth.kaushalz.com/.auth/login/microsoftaccount?post_login_redirect_url=/" title="https://easyauth.kaushalz.com/.auth/login/microsoftaccount?post_login_redirect_url=/"><span style="font-family: segoe ui"><span style="font-size: small">https://easyauth.kaushalz.com/.auth/login/<span style="background-color: #ffff00">microsoftaccount</span>?<span style="background-color: #ffff00">post_login_redirect_url=/</span></span></span></a>
</p>

<table style="height: 55px;margin-left: 50px" width="610" cellspacing="0" cellpadding="0" border="3">
  <tr>
    <td width="529" valign="top">
      <span style="font-size: small;font-family: segoe ui"><span style="font-family: segoe ui"><span style="font-size: small"><strong>NOTE</strong></span></span>:<em> The query string parameter</em> <span style="font-size: small;font-family: segoe ui"><span style="font-family: consolas;color: #0000ff;background-color: #cccccc">post_login_redirect_uri</span></span> <em>redirects the user request to the value specified in url path. </em></span><span style="font-size: small;font-family: segoe ui"><em>In the above example url, post successful authentication, the users will be redirected to the root of the application</em>.<br /> </span>
    </td>
  </tr>
</table>

# Adding users email address to the Claim<span style="font-family: segoe ui"></span>

<span style="font-size: small;font-family: segoe ui">By default, the claim which is obtained from <strong>Microsoft Account</strong> provider doesn’t contain the users email address. Here is a how the default user claims obtained from MSA looks like</span>

<p style="padding-left: 60px">
  <a href="https://msdnshared.blob.core.windows.net/media/2016/04/image37.png"><img style="padding-top: 0px;padding-left: 0px;padding-right: 0px;border-width: 0px" title="image" src="https://msdnshared.blob.core.windows.net/media/2016/04/image_thumb36.png" alt="image" width="605" border="0" height="583" /></a>
</p>

<span style="font-size: small;font-family: segoe ui">To add the email address as part of the claim the following scopes have to be enabled:</span>

  * **<span style="font-size: small;font-family: segoe ui">wl.basic </span>**
  * <span style="font-family: segoe ui"><span style="font-size: small"><strong>wl.emails</strong> </span></span>

<table style="height: 29px;margin-left: 50px" width="610" cellspacing="0" cellpadding="0" border="3">
  <tr>
    <td width="494" valign="top">
      <span style="font-family: segoe ui"><span style="font-size: small"><strong>NOTE</strong>: The token can be obtain by calling the following endpoint <span style="font-family: consolas;color: #0000ff;background-color: #cccccc">/.auth/me</span></span></span>
    </td>
  </tr>
</table>

<span style="font-size: small;font-family: segoe ui">Refer the following steps on how to configure this via the Azure portal<br /> </span>

  * <span style="font-size: small;font-family: segoe ui">Log-in to Azure portal: </span>[<span style="font-size: small;font-family: segoe ui">https://portal.azure.com</span>](https://portal.azure.com)<span style="font-size: small;font-family: segoe ui"> </span>
  * <span style="font-size: small;font-family: segoe ui">Click on <strong>App Service</strong> & select the web app<br /> </span>
  * <span style="font-size: small;font-family: segoe ui">Under <strong>Settings</strong> blade, click on <strong>Authentication/Authorization</strong> (This will launch another blade for this feature</span>
  * <span style="font-size: small;font-family: segoe ui">In here, configure the following<br /> </span></p> 
      1. <span style="font-size: small;font-family: segoe ui">Set App Service Authentication to <strong>On</strong></span>
      2. <span style="font-size: small;font-family: segoe ui">Under Authentication providers, click on <strong>Microsoft Account</strong>.</span>
      3. <span style="font-size: small;font-family: segoe ui">Click on <strong> <span style="color: #0000ff"><span style="font-family: consolas;background-color: #cccccc">wl.basic</span></span> & <span style="color: #0000ff"><span style="font-family: consolas;background-color: #cccccc">wl.emails</span></span></strong> to enable them </span><span style="font-size: small;font-family: segoe ui">(Refer the following screenshot)</span>

<p style="padding-left: 60px">
  <a href="https://msdnshared.blob.core.windows.net/media/2016/04/image38.png"><span style="font-size: small;font-family: segoe ui"><img style="padding-top: 0px;padding-left: 0px;margin: 1px;padding-right: 0px;border-width: 0px" title="image" src="https://msdnshared.blob.core.windows.net/media/2016/04/image_thumb37.png" alt="image" width="1020" border="0" height="847" /></span></a>
</p>

  * <span style="font-size: small;font-family: segoe ui">Click on <strong>OK</strong> and then click on <strong>Save</strong>. </span>

<span style="font-size: small;font-family: segoe ui">When the users try to login again, the application will notify the user that it needs permissions so that the application can retrieve users email address. This happens for the first time.<br /> </span>

<p style="padding-left: 60px">
  <a href="https://msdnshared.blob.core.windows.net/media/2016/04/image40.png"><img style="padding-top: 0px;padding-left: 0px;padding-right: 0px;border-width: 0px" title="image" src="https://msdnshared.blob.core.windows.net/media/2016/04/image_thumb39.png" alt="image" width="415" border="0" height="446" /></a>
</p>

<span style="font-size: small;font-family: segoe ui">Upon giving permissions to the application, the <strong>users email address</strong> becomes part of the <strong>user_claims</strong>. Below is a screenshot for reference:</span>

<p style="padding-left: 60px">
  <a href="https://msdnshared.blob.core.windows.net/media/2016/04/image39.png"><span style="font-size: small;font-family: segoe ui"><img style="padding-top: 0px;padding-left: 0px;padding-right: 0px;border-width: 0px" title="image" src="https://msdnshared.blob.core.windows.net/media/2016/04/image_thumb38.png" alt="image" width="681" border="0" height="796" /></span></a>
</p>

<table style="height: 24px;margin-left: 50px" width="610" cellspacing="0" cellpadding="0" border="3">
  <tr>
    <td width="494" valign="top">
      <span style="font-family: segoe ui"><span style="font-size: small"><strong>NOTE</strong>: I used Chrome browser with the <strong>JSON Formatter </strong>extension installed to see the claim </span></span>
    </td>
  </tr>
</table>

&nbsp;

<span style="text-decoration: underline"><strong><span style="font-size: small;font-family: segoe ui">MORE INFORMATION:</span></strong></span>

<span style="font-size: small;font-family: segoe ui">In case the application is not hosted on Azure App Service, please refer the following thread on Stackoverflow on how to do this for your application.</span>

<span style="font-size: small;font-family: segoe ui"><a href="http://stackoverflow.com/questions/17168353/getting-email-from-oauth-authentication-microsoft?lq=1">http://stackoverflow.com/questions/17168353/getting-email-from-oauth-authentication-microsoft?lq=1</a><strong><br /> </strong></span>

<span style="font-size: small;font-family: segoe ui"> </span>