---
id: 1405
title: 'Azure App Service: How to connect to the Kudu site of a specific instance'
date: 2016-11-21T12:21:00+00:00
author: kaushal
layout: post
guid: https://blogs.msdn.microsoft.com/kaushal/?p=1405
permalink: /2016/11/21/azure-app-service-how-to-connect-to-the-kudu-site-of-a-specific-instance/
opengraph_tags:
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Azure App Service: How to connect to the Kudu site of a specific instance" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2016/11/21/azure-app-service-how-to-connect-to-the-kudu-site-of-a-specific-instance/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="Every Azure Web App has an associated &#8216;scm&#8217; service site, which runs Kudu and other Site Extensions. OVERVIEW: Kudu site can be accessed using either of these credentials Single Sign-on User-level credentials (aka Deployment Credentials) Site-level credentials&nbsp; (aka Publish Profile Credentials) Kudu site always connect to a single instance. E.g. If the site is hosted..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2016/11/image_thumb418.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Azure App Service: How to connect to the Kudu site of a specific instance" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2016/11/21/azure-app-service-how-to-connect-to-the-kudu-site-of-a-specific-instance/" />
    <meta name="twitter:description" content="Every Azure Web App has an associated &#8216;scm&#8217; service site, which runs Kudu and other Site Extensions. OVERVIEW: Kudu site can be accessed using either of these credentials Single Sign-on User-level credentials (aka Deployment Credentials) Site-level credentials&nbsp; (aka Publish Profile Credentials) Kudu site always connect to a single instance. E.g. If the site is hosted..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2016/11/image_thumb418.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Azure App Service: How to connect to the Kudu site of a specific instance" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2016/11/21/azure-app-service-how-to-connect-to-the-kudu-site-of-a-specific-instance/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="Every Azure Web App has an associated &#8216;scm&#8217; service site, which runs Kudu and other Site Extensions. OVERVIEW: Kudu site can be accessed using either of these credentials Single Sign-on User-level credentials (aka Deployment Credentials) Site-level credentials&nbsp; (aka Publish Profile Credentials) Kudu site always connect to a single instance. E.g. If the site is hosted..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2016/11/image_thumb418.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Azure App Service: How to connect to the Kudu site of a specific instance" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2016/11/21/azure-app-service-how-to-connect-to-the-kudu-site-of-a-specific-instance/" />
    <meta name="twitter:description" content="Every Azure Web App has an associated &#8216;scm&#8217; service site, which runs Kudu and other Site Extensions. OVERVIEW: Kudu site can be accessed using either of these credentials Single Sign-on User-level credentials (aka Deployment Credentials) Site-level credentials&nbsp; (aka Publish Profile Credentials) Kudu site always connect to a single instance. E.g. If the site is hosted..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2016/11/image_thumb418.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Azure App Service: How to connect to the Kudu site of a specific instance" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2016/11/21/azure-app-service-how-to-connect-to-the-kudu-site-of-a-specific-instance/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="Every Azure Web App has an associated &#8216;scm&#8217; service site, which runs Kudu and other Site Extensions. OVERVIEW: Kudu site can be accessed using either of these credentials Single Sign-on User-level credentials (aka Deployment Credentials) Site-level credentials&nbsp; (aka Publish Profile Credentials) Kudu site always connect to a single instance. E.g. If the site is hosted..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2016/11/image_thumb418.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Azure App Service: How to connect to the Kudu site of a specific instance" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2016/11/21/azure-app-service-how-to-connect-to-the-kudu-site-of-a-specific-instance/" />
    <meta name="twitter:description" content="Every Azure Web App has an associated &#8216;scm&#8217; service site, which runs Kudu and other Site Extensions. OVERVIEW: Kudu site can be accessed using either of these credentials Single Sign-on User-level credentials (aka Deployment Credentials) Site-level credentials&nbsp; (aka Publish Profile Credentials) Kudu site always connect to a single instance. E.g. If the site is hosted..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2016/11/image_thumb418.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Azure App Service: How to connect to the Kudu site of a specific instance" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2016/11/21/azure-app-service-how-to-connect-to-the-kudu-site-of-a-specific-instance/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="Every Azure Web App has an associated &#8216;scm&#8217; service site, which runs Kudu and other Site Extensions. OVERVIEW: Kudu site can be accessed using either of these credentials Single Sign-on User-level credentials (aka Deployment Credentials) Site-level credentials&nbsp; (aka Publish Profile Credentials) Kudu site always connect to a single instance. E.g. If the site is hosted..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2016/11/image_thumb418.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Azure App Service: How to connect to the Kudu site of a specific instance" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2016/11/21/azure-app-service-how-to-connect-to-the-kudu-site-of-a-specific-instance/" />
    <meta name="twitter:description" content="Every Azure Web App has an associated &#8216;scm&#8217; service site, which runs Kudu and other Site Extensions. OVERVIEW: Kudu site can be accessed using either of these credentials Single Sign-on User-level credentials (aka Deployment Credentials) Site-level credentials&nbsp; (aka Publish Profile Credentials) Kudu site always connect to a single instance. E.g. If the site is hosted..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2016/11/image_thumb418.png" />
    
categories:
  - ARRAffinity
  - Azure
  - Azure App Service
  - Azure Web App
  - Kudu
  - Web App
---
<font size="2">Every Azure Web App has an associated &#8216;scm&#8217; service site, which runs Kudu and other </font>[<font size="2">Site Extensions</font>](https://github.com/projectkudu/kudu/wiki/Azure-Site-Extensions)<font size="2">. </font> 

<div>
  <font size="2"><font size="4"><font face="Segoe UI Semibold"><u>OVERVIEW</u></font>:</font> </font>
</div>

  * <font size="2">Kudu site can be accessed using either of these credentials</font> 
      * <font size="2">Single Sign-on</font> 
          * <font size="2">User-level credentials (aka Deployment Credentials)</font> 
              * <font size="2">Site-level credentials&nbsp; (aka Publish Profile Credentials)</font></ul> 
              * <font size="2">Kudu site always connect to a single instance. E.g. If the site is hosted in an App Service plan which is scaled out to 3 instances, then at any time the KUDU will always connect to one instance only.</font></ul> 
            Here is a simple request flow of an Azure Web App 
            
            > [<img title="image" style="border-top: 0px;border-right: 0px;border-bottom: 0px;padding-top: 0px;padding-left: 0px;border-left: 0px;padding-right: 0px" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/2016/11/image_thumb418.png" width="616" height="340" />](https://msdnshared.blob.core.windows.net/media/2016/11/image503.png)
            
            <font size="2">The front-end uses <b>ARRAffinity</b> cookie to affinitize the request to specific instances. This cookie can be disabled if needed. Refer </font>[<font size="2">this</font>](https://azure.microsoft.com/en-in/blog/disabling-arrs-instance-affinity-in-windows-azure-web-sites/) <font size="2">on how disable ARR Affinity. </font> 
            
            <div>
              <font size="2">The <b>ARRAffinity</b> cookie is unique and corresponds to an instance. If there are multiple instances, then there will be <b>ARRAffinity</b> cookie corresponding to those many instances.</font> <font size="2">So we can modify the <b>ARRAffinity</b> cookie in the HTTP response and force KUDU to connect to a specific instance. </font>
            </div>
            
            <div>
              &nbsp;
            </div>
            
            <div>
              <font size="2"><font size="4"><font face="Segoe UI Semibold"><u>PRE-REQUISITES</u></font>:</font> </font>
            </div>
            
              * <font size="2"><strong>Browser</strong>: Chrome/Firefox/Opera or any other browser which has extensions that allows you to edit cookies.</font> 
                  * <font size="2"><strong>Extension</strong>: <a href="https://chrome.google.com/webstore/detail/editthiscookie/fngmhnnpilhplaeedifhccceomclgfbg?hl=en">EditThisCookie (Chrome)</a> | <a title="https://addons.opera.com/en/extensions/details/edit-this-cookie/" href="https://addons.opera.com/en/extensions/details/edit-this-cookie/">EditThisCookie (Opera)</a></font></ul> 
                <u><font size="4" face="Segoe UI Semibold">DETERMINE THE ARRAFFINITY COOKIE OF AN INSTANCE</font> </u> 
                
                  * <font size="2">Browse to </font>[<font size="2">https://resources.azure.com/</font>](https://resources.azure.com/) <font size="2">(Azure Resource Explorer) </font> 
                      * <font size="2">In the search window enter the name of the web app. See the following screenshot for reference:</font></ul> 
                    > [<img title="image" style="border-left-width: 0px;border-right-width: 0px;border-bottom-width: 0px;padding-top: 0px;padding-left: 0px;padding-right: 0px;border-top-width: 0px" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/2016/11/image_thumb419.png" width="1028" height="487" />](https://msdnshared.blob.core.windows.net/media/2016/11/image504.png)
                    
                      * <font size="2">If there are other Azure resources with similar names, select the resource of type “<b>Microsoft.Web/sites</b>” </font> 
                          * <font size="2">In the left side panel, expand “<b>instances</b>” and this would load all the instances on which the web app is hosted. The instance name displayed is also the value of the <strong>ARRAffinity</strong> cookie. </font></ul> 
                        > [<img title="image" style="border-left-width: 0px;border-right-width: 0px;border-bottom-width: 0px;padding-top: 0px;padding-left: 0px;padding-right: 0px;border-top-width: 0px" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/2016/11/image_thumb420.png" width="1026" height="498" />](https://msdnshared.blob.core.windows.net/media/2016/11/image505.png)
                        
                        <font size="2">In the above image the site kaushalp is scaled out to 2 instances. So we have 2 instance id’s which are beginning with:</font>
                        
                          1. <font size="2">bac64d </font> 
                              * <font size="2">c2a879</font></ol> 
                            <u><font size="4" face="Segoe WP Semibold">CONNECT TO THE KUDU CONSOLE OF A SPECIFIC INSTANCE</font></u> 
                            
                              * <font size="2">For this we need to have a tool which allows us to modify the cookies </font> 
                                  * <font size="2">There are multiple ways to do this. </font> 
                                      * <font size="2">I am using <b>EditThisCookie</b> extension in chrome browser. Here is the link to install this: </font>[<font size="2">Install EditThisCookie</font>](https://chrome.google.com/webstore/detail/editthiscookie/fngmhnnpilhplaeedifhccceomclgfbg?hl=en) <font size="2"></font> 
                                          * <font size="2">Now, browse to the KUDU site of your web app: </font>[<font size="2">https://<sitename>.scm.azurewebsites.net</font>](https://%3csitename%3e.scm.azurewebsites.net) <font size="2">(<i>replace <sitename> with name of the web app</i>) </font> 
                                              * <font size="2">Click on <strong>Environment</strong>. </font> 
                                                  * <font size="2">Under <b>System info</b>, the “<b>instance id</b>” value determines the instance to which the KUDU is connected. In the screenshot below, the kudu site is connected to the instance whose <strong>short instance id</strong> is <strong>bac64d</strong>.</font></ul> 
                                                > [<font size="2"><a href="https://msdnshared.blob.core.windows.net/media/2016/11/image507.png"><img title="image" style="border-left-width: 0px;border-right-width: 0px;border-bottom-width: 0px;padding-top: 0px;padding-left: 0px;padding-right: 0px;border-top-width: 0px" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/2016/11/image_thumb421.png" width="679" height="258" /></a></font>](https://msdnshared.blob.core.windows.net/media/2016/11/image506.png)
                                                
                                                  * <font size="2">We can use one of the instances value we obtained via <b>ARM explorer</b> to force KUDU to connect to a specific site. <br />(Here we are connecting to the instance with the id beginning with “<b>bac64d</b>” ) </font> 
                                                      * <font size="2">In the browser window click on <b>EditThisCookie </b><b><a href="https://msdnshared.blob.core.windows.net/media/2016/11/clip_image005.gif"><img title="clip_image005" style="border-left-width: 0px;border-right-width: 0px;border-bottom-width: 0px;padding-top: 0px;padding-left: 0px;margin: 0px;padding-right: 0px;border-top-width: 0px" border="0" alt="clip_image005" src="https://msdnshared.blob.core.windows.net/media/2016/11/clip_image005_thumb.gif" width="19" height="19" /></a></b>&nbsp; icon (next to the <b>Address bar)</b>. </font></ul> 
                                                    > [<font size="2"><a href="https://msdnshared.blob.core.windows.net/media/2016/11/clip_image00618.jpg"><img title="clip_image006" style="border-left-width: 0px;border-right-width: 0px;border-bottom-width: 0px;padding-top: 0px;padding-left: 0px;padding-right: 0px;border-top-width: 0px" border="0" alt="clip_image006" src="https://msdnshared.blob.core.windows.net/media/2016/11/clip_image006_thumb14.jpg" width="621" height="103" /></a></font>](https://msdnshared.blob.core.windows.net/media/2016/11/clip_image00617.jpg)
                                                    
                                                      * <font size="2">In the pop-up, click on <strong>ARRAffinity</strong> </font>
                                                    
                                                    > [<font size="2"><a href="https://msdnshared.blob.core.windows.net/media/2016/11/clip_image0072.jpg"><img title="clip_image007" style="border-left-width: 0px;border-right-width: 0px;border-bottom-width: 0px;padding-top: 0px;padding-left: 0px;padding-right: 0px;border-top-width: 0px" border="0" alt="clip_image007" src="https://msdnshared.blob.core.windows.net/media/2016/11/clip_image007_thumb1.jpg" width="620" height="226" /></a></font>](https://msdnshared.blob.core.windows.net/media/2016/11/clip_image0071.jpg)
                                                    
                                                      * <font size="2">Replace the value with the instance id that you need to connect to</font>
                                                    
                                                    > [<font size="2"><a href="https://msdnshared.blob.core.windows.net/media/2016/11/image509.png"><img title="image" style="border-left-width: 0px;border-right-width: 0px;border-bottom-width: 0px;padding-top: 0px;padding-left: 0px;padding-right: 0px;border-top-width: 0px" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/2016/11/image_thumb422.png" width="591" height="525" /></a></font>](https://msdnshared.blob.core.windows.net/media/2016/11/image508.png)
                                                    
                                                      * <font size="2">Click on the<strong> tick mark</strong> to save the cookie and then refresh the page. </font>
                                                    
                                                    <font size="2">It should have connected to other instance. To confirm, browse to <strong>Environment </strong>and under <strong>System Info </strong>the value of Instance id should match the value that was entered earlier.</font>