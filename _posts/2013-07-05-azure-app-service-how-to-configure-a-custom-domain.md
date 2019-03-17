---
id: 316
title: 'Azure App Service: How to configure a custom domain'
date: 2013-07-05T19:48:00+00:00
author: kaushal
layout: post
guid: https://blogs.msdn.microsoft.com/kaushal/2013/07/05/microsoft-azure-web-sites-how-to-configure-a-custom-domain/
permalink: /2013/07/05/azure-app-service-how-to-configure-a-custom-domain/
orig_url:
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2013/07/06/windows-azure-web-sites-how-to-configure-a-custom-domain.aspx
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2013/07/06/windows-azure-web-sites-how-to-configure-a-custom-domain.aspx
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2013/07/06/windows-azure-web-sites-how-to-configure-a-custom-domain.aspx
orig_site_id:
  - "13803"
  - "13803"
  - "13803"
orig_post_id:
  - "10432099"
  - "10432099"
  - "10432099"
orig_parent_id:
  - "10432099"
  - "10432099"
  - "10432099"
orig_application_key:
  - kaushal
  - kaushal
  - kaushal
orig_post_author_id:
  - "213737"
  - "213737"
  - "213737"
orig_post_author_username:
  - djkaushal
  - djkaushal
  - djkaushal
orig_post_author_created:
  - 2009-07-24 14:00:49.000
  - 2009-07-24 14:00:49.000
  - 2009-07-24 14:00:49.000
orig_is_approved:
  - "1"
  - "1"
  - "1"
orig_url_title:
  - http://blogs.msdn.com/b/kaushal/archive/2013/07/05/microsoft-azure-web-sites-how-to-configure-a-custom-domain.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2013/07/05/microsoft-azure-web-sites-how-to-configure-a-custom-domain.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2013/07/05/microsoft-azure-web-sites-how-to-configure-a-custom-domain.aspx
orig_post_name:
  - windows azure web sites how to configure a custom domain
  - windows azure web sites how to configure a custom domain
  - windows azure web sites how to configure a custom domain
orig_thread_id:
  - "847760"
  - "847760"
  - "847760"
orig_post_author_email:
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
orig_attachment_count:
  - "0"
  - "0"
  - "0"
total_views:
  - "28293"
  - "28293"
  - "28293"
opengraph_tags:
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="" />
    <meta property="og:url" content="" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="" />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="" />
    <meta name="twitter:url" content="" />
    <meta name="twitter:description" content="" />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="" />
    <meta property="og:url" content="" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="" />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="" />
    <meta name="twitter:url" content="" />
    <meta name="twitter:description" content="" />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="" />
    <meta property="og:url" content="" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="" />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="" />
    <meta name="twitter:url" content="" />
    <meta name="twitter:description" content="" />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="" />
    <meta property="og:url" content="" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="" />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="" />
    <meta name="twitter:url" content="" />
    <meta name="twitter:description" content="" />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="" />
    <meta property="og:url" content="" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="" />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="" />
    <meta name="twitter:url" content="" />
    <meta name="twitter:description" content="" />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="" />
    <meta property="og:url" content="" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="" />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="" />
    <meta name="twitter:url" content="" />
    <meta name="twitter:description" content="" />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="" />
    <meta property="og:url" content="" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="" />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="" />
    <meta name="twitter:url" content="" />
    <meta name="twitter:description" content="" />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="" />
    <meta property="og:url" content="" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="" />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="" />
    <meta name="twitter:url" content="" />
    <meta name="twitter:description" content="" />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="" />
    <meta property="og:url" content="" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="" />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="" />
    <meta name="twitter:url" content="" />
    <meta name="twitter:description" content="" />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="" />
    <meta property="og:url" content="" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="" />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="" />
    <meta name="twitter:url" content="" />
    <meta name="twitter:description" content="" />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="" />
    <meta property="og:url" content="" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="" />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="" />
    <meta name="twitter:url" content="" />
    <meta name="twitter:description" content="" />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="" />
    <meta property="og:url" content="" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="" />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="" />
    <meta name="twitter:url" content="" />
    <meta name="twitter:description" content="" />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="" />
    <meta property="og:url" content="" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="" />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="" />
    <meta name="twitter:url" content="" />
    <meta name="twitter:description" content="" />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="" />
    <meta property="og:url" content="" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="" />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="" />
    <meta name="twitter:url" content="" />
    <meta name="twitter:description" content="" />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="" />
    <meta property="og:url" content="" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="" />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="" />
    <meta name="twitter:url" content="" />
    <meta name="twitter:description" content="" />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="" />
    <meta property="og:url" content="" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="" />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="" />
    <meta name="twitter:url" content="" />
    <meta name="twitter:description" content="" />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="" />
    <meta property="og:url" content="" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="" />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="" />
    <meta name="twitter:url" content="" />
    <meta name="twitter:description" content="" />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="" />
    <meta property="og:url" content="" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="" />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="" />
    <meta name="twitter:url" content="" />
    <meta name="twitter:description" content="" />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" />
    
categories:
  - Uncategorized
tags:
  - A record
  - ANTARES
  - awverify
  - Azure
  - azurewebsites.net
  - CNAME
  - DNS Verification
  - domain name
  - GoDaddy
  - kaushal
  - kaushalp
  - Petr Podhorsky
  - shared
  - standard
  - TXT record
  - WAWS
  - Windows Azure
  - Windows Azure Web Sites
---
**<span style="font-size: 10pt;font-family: segoe ui">[Updated on 2nd May 2016]</span>**

<span style="font-size: 10pt;font-family: segoe ui"><strong>Azure App Service</strong> provides a default hostname on site creation. It is of the format <strong><SITENAME>.azurewebsites.net</strong>. So when I create a website called <strong>Kaushalz</strong> then the hostname would be <strong>Kaushalz.azurewebsites.net</strong>. </span>

<span style="font-size: 10pt;font-family: segoe ui">Now the users can buy a custom domain via Azure portal. See this article: https://azure.microsoft.com/en-in/documentation/articles/custom-dns-web-site-buydomains-web-app/ </span>

<span style="font-size: 10pt;font-family: segoe ui">If you decide to buy a custom domain externally then you would have to configure it. There is one requirement though, the pricing tier of the Web App needs to be in either <strong>SHARED </strong>or higher tiers<strong>.</strong>&nbsp;</span>

<span style="font-size: 10pt;font-family: segoe ui">There is an article on <a href="http://www.windowsazure.com">www.windowsazure.com</a> on how to configure custom domain. Below is the URL: </span>

<a title="Configure a custom domain name in Azure App Service" href="https://azure.microsoft.com/en-in/documentation/articles/web-sites-custom-domain-name/" target="_blank" rel="noopener noreferrer"><span style="font-size: 10pt;font-family: segoe ui">http://azure.microsoft.com/en-us/documentation/articles/web-sites-custom-domain-name</span></a>

<span style="font-size: 10pt;font-family: segoe ui">However, I have still seen few customers running into issues in spite of this. In this post we will discuss adding custom domains to a MAWS site in detail. </span>

<span style="font-size: 10pt;font-family: segoe ui">There are 2 ways to configure domain names: </span>

  1. <span style="font-size: 10pt;font-family: segoe ui">Add an <strong>A Record</strong>. </span> 
      * <span style="font-size: 10pt;font-family: segoe ui">Add a <strong>CNAME</strong>. </span></ol> 
    <div style="margin-left: 98pt">
      <table style="background: #deeaf6;border-collapse: collapse" border="0">
        <colgroup> <col style="width: 623px"></colgroup> <tr>
          <td style="border-top: #0070c0 2.25pt solid;border-right: #0070c0 2.25pt solid;border-bottom: #0070c0 2.25pt solid;padding-left: 7px;border-left: #0070c0 2.25pt solid;padding-right: 7px">
            <p style="text-align: justify">
              <span style="font-size: 10pt;font-family: segoe ui"><strong>NOTE</strong>: A records map a domain name to one or more IP addresses. They are used when the IP is not bound to change. </span>
            </p>
            
            <p style="text-align: justify">
              <span style="font-size: 10pt;font-family: segoe ui"><strong>Example</strong>: kaushalz.com points to <strong>65.52.168.214</strong>. </span>
            </p>
            
            <p style="text-align: justify">
              <span style="font-size: 10pt;font-family: segoe ui">On the other hand <strong>CNAME</strong> (<strong>CANONICAL NAME</strong>) records map one domain name to another domain name. It is typically used when there are multiple hosted services. </span>
            </p>
            
            <p style="text-align: justify">
              <span style="font-size: 10pt;font-family: segoe ui"><strong>Example</strong>: <a href="ftp://ftp.kaushalz.com">ftp.kaushalz.com</a> or <a href="http://www.kaushalz.com">www.kaushalz.com</a> points to <a href="http://kaushalz.com">kaushalz.com</a></span>
            </p>
          </td>
        </tr>
      </table>
    </div>
    
    <span style="font-size: 10pt;font-family: segoe ui">I have purchased the domain <strong>kaushal.co.in</strong> from GoDaddy. Here <strong>kaushal.co.in</strong> is also referred to as <strong>ROOT</strong>/<strong>NAKED</strong> domain. By design, <strong>ROOT</strong> domains have to be an <strong>A record</strong>, so they will point to an IP always. </span>
    
    <span style="font-size: 10pt;font-family: segoe ui">Anything that is prefixed before this is referred to as <strong>sub-domain</strong>. Examples are <strong>www.<span style="font-size: small;font-family: segoe ui">kaushal.co.in</span></strong>, <strong>ftp.<span style="font-size: small;font-family: segoe ui">kaushal.co.in</span>, </strong><strong>*.<span style="font-size: small;font-family: segoe ui">kaushal.co.in</span>.</strong></span>
    
    <span style="font-size: 10pt;font-family: segoe ui">As per DNS best practices, it is always recommended to point your sub-domains to CNAME records. This is because IP address can change dynamically for certain sites and this is not apt in case of an internet facing website.</span>
    
    <table style="border-collapse: collapse" border="0">
      <colgroup> <col style="width: 888px"> <col style="width: 85px"></colgroup> <tr>
        <td style="border-top: #0070c0 4.5pt solid;padding-left: 7px;padding-right: 7px" colspan="2">
          &nbsp;
        </td>
      </tr>
      
      <tr style="background: #3b3838">
        <td style="padding-left: 7px;padding-right: 7px" valign="middle">
          <span style="font-size: 18pt;font-family: segoe ui;color: #00b0f0"><strong>STEP 1: Create a Website and scale it to SHARED/BASIC/STANDARD</strong></span>
        </td>
      </tr>
    </table>
    
      * <span style="font-size: 10pt;font-family: segoe ui">In the Azure portal create a web app and scale this to a minimum of SHARED tier in order to be able to configure a <strong>Custom Domain</strong>.</span> 
          * <span style="font-size: 10pt;font-family: segoe ui">Refer this link for scaling <strong>Microsoft Azure Web Sites</strong>: <a href="http://azure.microsoft.com/en-us/documentation/articles/web-sites-scale/">Configure your web sites for basic, shared or standard mode</a> </span></ul> 
        <span style="font-family: segoe ui"><span style="font-size: 10pt">Once the web app has been scaled to <strong>SHARED</strong> or higher tier, we can proceed further.</span></span>
        
        <table style="border-collapse: collapse" border="0">
          <colgroup> <col style="width: 888px"> <col style="width: 85px"></colgroup> <tr>
            <td style="border-top: #0070c0 4.5pt solid;padding-left: 7px;padding-right: 7px" colspan="2">
              &nbsp;
            </td>
          </tr>
          
          <tr style="background: #3b3838">
            <td style="padding-left: 7px;padding-right: 7px" valign="middle">
              <span style="font-size: 18pt;font-family: segoe ui;color: #00b0f0"><strong>STEP 2: Configuration on the DNS Service Provider /DNS Server</strong></span>
            </td>
          </tr>
        </table>
        
        <p style="padding-left: 30px">
          <span style="font-size: 10pt;font-family: segoe ui">In the Azure portal, select the web app and under settings browse to <strong>Custom Domains and SSL</strong>. In the&nbsp; <strong><span style="font-size: small;font-family: segoe ui">Custom Domains and SSL</span></strong> blade, click on <strong>Bring External Domains</strong>. This will launch a new blade as shown below.</span>
        </p>
        
        <p style="padding-left: 30px">
          <a href="https://msdnshared.blob.core.windows.net/media/2016/05/image50.png"><img title="image" style="border-top: 0px;border-right: 0px;border-bottom: 0px;float: none;padding-top: 0px;padding-left: 0px;margin-left: auto;border-left: 0px;padding-right: 0px;margin-right: auto" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb48.png" width="309" height="562" /></a>
        </p>
        
        <p style="margin-left: 18pt">
          <span style="font-size: 10pt;font-family: segoe ui">It specifies an IP (<strong>Front-end VIP</strong>) which is to be used while configuring <strong>A Records</strong> on the <strong>DNS server</strong>. Additionally it also suggests that before we add custom domains for the site, <strong>Azure</strong> needs to verify that the user is authorized to use the domain name or not. </span>
        </p>
        
          * <div>
              <span style="font-size: 10pt;font-family: segoe ui">Add an <strong>A record</strong> pointing to the <strong>IP</strong> as seen above. </span>
            </div>
            
            <p style="text-align: center;margin-left: 18pt">
              <img alt="" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/0081.050614_1141_MicrosoftAz4.png" />
            </p>
        
        <div style="margin-left: 98pt">
          <table style="background: #deeaf6;border-collapse: collapse" border="0">
            <colgroup> <col style="width: 623px"></colgroup> <tr>
              <td style="border-top: #0070c0 2.25pt solid;border-right: #0070c0 2.25pt solid;border-bottom: #0070c0 2.25pt solid;padding-left: 7px;border-left: #0070c0 2.25pt solid;padding-right: 7px">
                <p style="text-align: justify">
                  <span style="font-size: 10pt;font-family: segoe ui"><strong>NOTE: </strong>Entering &#8220;<strong>@</strong>&#8221; for the host name is the same as entering your domain name, minus the &#8220;<strong>www</strong>&#8220;. Entering &#8220;<strong>www</strong>&#8221; for the host name is the same as entering your domain name, including the &#8220;<strong>www</strong>&#8220;. </span>
                </p>
                
                <p style="text-align: justify">
                  <span style="font-size: 10pt;font-family: segoe ui">To create a <strong>wildcard A record</strong>, enter an asterisk (&#8220;<strong>*</strong>&#8220;) for the host name. The wildcard makes the server respond with the <strong>IP address</strong> specified instead of an error, if the subdomain queried does not exist within your zone file.</span>
                </p>
              </td>
            </tr>
          </table>
        </div>
        
          * <div style="text-align: left">
              <span style="font-size: 10pt;font-family: segoe ui">Additionally for the <strong>ROOT DOMAIN</strong> (<strong>kaushalz.org</strong>) you will have to add another <strong>CNAME</strong> entry. Here you will point <strong>awverify.kaushal.com</strong> to <strong>awverify.kaushal.azurewebsites.net</strong>. </span>
            </div>
            
            <p style="text-align: center;margin-left: 18pt">
              <img alt="" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8322.050614_1141_MicrosoftAz6.png" />
            </p>
            
              * <p style="text-align: left;margin-left: 18pt">
                  <span style="font-size: 10pt;font-family: segoe ui">My DNS service provider is <strong>GoDaddy,</strong> so I need to point <strong>www</strong> to <strong>kaushal.azurewebsites.net</strong>. Below is a snapshot of my <strong>DNS Manager</strong>. I have a <strong>CNAME</strong> entry pointing to the <strong><sitename>.azurewebsites.net</strong>. </span>
                </p></ul> 
            
            <p style="text-align: center;margin-left: 18pt">
              <p style="text-align: center;margin-left: 18pt">
                <img alt="" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/5102.050614_1141_MicrosoftAz5.png" />
              </p>
              
              <p style="text-align: center;margin-left: 18pt">
                <div style="margin-left: 98pt">
                  <table style="background: #deeaf6;border-collapse: collapse" border="0">
                    <colgroup> <col style="width: 623px"></colgroup> <tr>
                      <td style="border-top: #0070c0 2.25pt solid;border-right: #0070c0 2.25pt solid;border-bottom: #0070c0 2.25pt solid;padding-left: 7px;border-left: #0070c0 2.25pt solid;padding-right: 7px">
                        <p style="text-align: justify">
                          <span style="font-size: 10pt;font-family: segoe ui"><strong>NOTE: </strong>Above step is only for verification purpose. Once the <strong>ROOT DOMAIN</strong> (<strong>kaushalz.com</strong>) has been mapped to the site in Azure Portal, the <strong>awverify</strong> entry can be removed.</span>
                        </p>
                      </td>
                    </tr>
                  </table>
                </div>
                
                <table style="border-collapse: collapse" border="0">
                  <colgroup> <col style="width: 879px"> <col style="width: 95px"></colgroup> <tr>
                    <td style="border-top: #0070c0 4.5pt solid;padding-left: 7px;padding-right: 7px" colspan="2">
                      &nbsp;
                    </td>
                  </tr>
                  
                  <tr style="background: #3b3838">
                    <td style="padding-left: 7px;padding-right: 7px" valign="middle">
                      <span style="font-size: 18pt;font-family: segoe ui;color: #00b0f0"><strong>STEP 3: Map the domain name in the Azure Portal</strong></span>
                    </td>
                  </tr>
                </table>
                
                <p>
                  <span style="font-size: 10pt;font-family: segoe ui">Once the DNS entries have been made the DNS record propagation can take time. This depends on the DNS Provider. Once the records have been propagated, you could proceed with mapping this domain name to the specific website in <strong>Azure</strong>. </span>
                </p>
                
                <ul>
                  <li>
                    <span style="font-size: 10pt;font-family: segoe ui">In the Azure portal, select the web app and under settings browse to <strong>Custom Domains and SSL</strong>. In the&nbsp; <strong><span style="font-size: small;font-family: segoe ui">Custom Domains and SSL</span></strong> blade, click on <strong>Bring External Domains</strong>. This will launch a new blade as shown below.</span> <li>
                      <div>
                        <span style="font-size: 10pt;font-family: segoe ui">Enter the domain name and give it some time to verify. If it succeeds, then you would see something as shown below: </span>
                      </div>
                      
                      <p style="text-align: left">
                        <a href="https://msdnshared.blob.core.windows.net/media/2016/05/image51.png"><img title="image" style="border-top: 0px;border-right: 0px;border-bottom: 0px;float: none;padding-top: 0px;padding-left: 0px;margin-left: auto;border-left: 0px;padding-right: 0px;margin-right: auto" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb49.png" width="308" height="588" /></a>
                      </p>
                      
                      <li>
                        <p style="text-align: left">
                          <span style="font-size: 10pt;font-family: segoe ui">If the verification fails then you would get a corresponding warning message: </span>
                        </p>
                      </li></ul> 
                      
                      <p style="text-align: center">
                        <a href="https://msdnshared.blob.core.windows.net/media/2016/05/image52.png"><img title="image" style="border-top: 0px;border-right: 0px;border-bottom: 0px;padding-top: 0px;padding-left: 0px;border-left: 0px;padding-right: 0px" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/2016/05/image_thumb50.png" width="534" height="321" /></a>
                      </p>
                      
                      <div>
                        <table style="border-collapse: collapse" border="0">
                          <colgroup> <col style="width: 973px"></colgroup> <tr>
                            <td style="border-top: #0070c0 4.5pt solid;padding-left: 7px;padding-right: 7px">
                              &nbsp;
                            </td>
                          </tr>
                        </table>
                      </div>
                      
                      <p style="text-align: center">
                        <span style="font-size: 18pt;text-decoration: underline;color: #0070c0"><strong>Verifying DNS Propagation </strong></span>
                      </p>
                      
                      <p>
                        <span style="font-size: 10pt">You can verify the DNS propagation by going to this URL <a href="http://digwebinterface.com/">http://digwebinterface.com/</a> </span>
                      </p>
                      
                      <p>
                        <span style="font-size: 10pt">Specify the hostnames in the textbox and click on <strong>Dig</strong>. Verify the results to confirm if the recent changes have taken effect. </span>
                      </p>
                      
                      <p style="text-align: center">
                        <img alt="" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/7120.050614_1141_MicrosoftAz10.png" />
                      </p>
                      
                      <div style="margin-left: 98pt">
                        <table style="background: #deeaf6;border-collapse: collapse" border="0">
                          <colgroup> <col style="width: 623px"></colgroup> <tr>
                            <td style="border-top: #0070c0 2.25pt solid;border-right: #0070c0 2.25pt solid;border-bottom: #0070c0 2.25pt solid;padding-left: 7px;border-left: #0070c0 2.25pt solid;padding-right: 7px">
                              <p style="text-align: justify">
                                <span style="font-size: 10pt;font-family: segoe ui"><strong>NOTE: </strong><span style="color: #c00000;background-color: yellow">The propagation of the DNS entries takes up to 48 hours or sometimes even more than that</span>. In these cases you may have to wait for the propagation to succeed. The user needs to ensure that the awverify entry resolves to the corresponding entry which has been added in the DNS server while performing the look up. </span>
                              </p>
                            </td>
                          </tr>
                        </table>
                      </div>
                      
                      <p>
                        <span style="color: black"><span style="font-size: 10pt">I have observed that the DNS propagation is quicker with GoDaddy. This is my personal experience.</span></span>
                      </p>
                      
                      <table style="border-collapse: collapse" border="0">
                        <colgroup> <col style="width: 973px"></colgroup> <tr>
                          <td style="border-top: #0070c0 4.5pt solid;padding-left: 7px;padding-right: 7px">
                            &nbsp;
                          </td>
                        </tr>
                      </table>
                      
                      <p style="text-align: center">
                        <span style="font-size: 18pt;text-decoration: underline;color: #0070c0"><strong>MIGRATION FROM ON-PREMISE PRODUCTION TO MAWS </strong></span>
                      </p>
                      
                      <p>
                        <span style="font-size: 10pt">Now consider a scenario where the user wants to migrate his production website, which is on premise, to <strong>MICROSOFT AZURE WEB SITE</strong>, without affecting any of his existing sites. He would want to map the hostname (verification) to MAWS and then would modify his DNS records. What should he do? </span>
                      </p>
                      
                      <p>
                        <span style="font-size: 10pt">For this he would have to create <strong>CNAME</strong> records on the DNS service provider as shown below: </span>
                      </p>
                      
                      <div style="margin-left: 98pt">
                        <table style="border-collapse: collapse" border="0">
                          <colgroup> <col style="width: 187px"> <col style="width: 161px"> <col style="width: 246px"></colgroup> <tr style="height: 28px;background: #0070c0">
                            <td style="border-top: #0070c0 2.25pt solid;border-right: #0070c0 1pt solid;border-bottom: #0070c0 1pt solid;padding-left: 7px;border-left: #0070c0 2.25pt solid;padding-right: 7px" valign="middle">
                              <p style="text-align: center">
                                <span style="font-size: 12pt;font-family: segoe ui;color: white"><strong>HOST</strong></span>
                              </p>
                            </td>
                            
                            <td style="border-left-style: none;border-top: #0070c0 2.25pt solid;border-right: #0070c0 1pt solid;border-bottom: #0070c0 1pt solid;padding-left: 7px;padding-right: 7px" valign="middle">
                              <p style="text-align: center">
                                <span style="font-size: 12pt;font-family: segoe ui;color: white"><strong>RECORD TYPE</strong></span>
                              </p>
                            </td>
                            
                            <td style="border-left-style: none;border-top: #0070c0 2.25pt solid;border-right: #0070c0 2.25pt solid;border-bottom: #0070c0 1pt solid;padding-left: 7px;padding-right: 7px" valign="middle">
                              <p style="text-align: center">
                                <span style="font-size: 12pt;font-family: segoe ui;color: white"><strong>POINTS TO</strong></span>
                              </p>
                            </td>
                          </tr>
                          
                          <tr style="height: 22px">
                            <td style="border-top-style: none;border-right: #0070c0 1pt solid;background: white;border-bottom: #0070c0 1pt solid;padding-left: 7px;border-left: #0070c0 2.25pt solid;padding-right: 7px" valign="middle">
                              <p style="text-align: center">
                                <span style="font-size: 10pt;font-family: segoe ui;color: black">awverify.kaushalz.org</span>
                              </p>
                            </td>
                            
                            <td style="border-top-style: none;border-left-style: none;border-right: #0070c0 1pt solid;border-bottom: #0070c0 1pt solid;padding-left: 7px;padding-right: 7px" valign="middle">
                              <p style="text-align: center">
                                <span style="font-size: 10pt;font-family: segoe ui;color: black">CNAME</span>
                              </p>
                            </td>
                            
                            <td style="border-top-style: none;border-left-style: none;border-right: #0070c0 2.25pt solid;border-bottom: #0070c0 1pt solid;padding-left: 7px;padding-right: 7px" valign="middle">
                              <p style="text-align: center">
                                <span style="font-size: 10pt;font-family: segoe ui;color: black">awverify.kaushalz.azurewebsites.net</span>
                              </p>
                            </td>
                          </tr>
                          
                          <tr style="height: 22px">
                            <td style="border-top-style: none;border-right: #0070c0 1pt solid;background: white;border-bottom: #0070c0 2.25pt solid;padding-left: 7px;border-left: #0070c0 2.25pt solid;padding-right: 7px" valign="middle">
                              <p style="text-align: center">
                                <span style="font-size: 10pt;font-family: segoe ui;color: black">awverify.www.kaushalz.org</span>
                              </p>
                            </td>
                            
                            <td style="border-top-style: none;border-left-style: none;border-right: #0070c0 1pt solid;border-bottom: #0070c0 2.25pt solid;padding-left: 7px;padding-right: 7px" valign="middle">
                              <p style="text-align: center">
                                <span style="font-size: 10pt;font-family: segoe ui;color: black">CNAME</span>
                              </p>
                            </td>
                            
                            <td style="border-top-style: none;border-left-style: none;border-right: #0070c0 2.25pt solid;border-bottom: #0070c0 2.25pt solid;padding-left: 7px;padding-right: 7px" valign="middle">
                              <p style="text-align: center">
                                <span style="font-size: 10pt;font-family: segoe ui;color: black">awverify.kaushalz.azurewebsites.net</span>
                              </p>
                            </td>
                          </tr>
                        </table>
                      </div>
                      
                      <p>
                        <span style="font-size: 10pt">We add 2 entries: </span>
                      </p>
                      
                      <ul>
                        <li>
                          <span style="font-size: 10pt">One for the <strong>ROOT DOMAIN</strong> (<strong>kaushalz.com</strong>) </span>
                        </li>
                      </ul>
                      
                      <ul>
                        <li>
                          <span style="font-size: 10pt">One for the domain containing <strong>WWW</strong> (<strong>www.kaushalz.com</strong>) </span>
                        </li>
                      </ul>
                      
                      <p>
                        <span style="font-size: 10pt;font-family: segoe ui">Below is a snapshot on the DNS Provider (<strong>GoDaddy</strong>): </span>
                      </p>
                      
                      <p style="text-align: center">
                        <img alt="" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/7635.050614_1141_MicrosoftAz11.png" />
                      </p>
                      
                      <p>
                        <span style="font-family: segoe ui"><span style="font-size: 10pt">After adding the above 2 entries you could map the domain name to a site hosted on <strong>AZURE</strong>.</span></span>
                      </p>
                      
                      <table style="border-collapse: collapse" border="0">
                        <colgroup> <col style="width: 973px"></colgroup> <tr>
                          <td style="border-top: #0070c0 4.5pt solid;padding-left: 7px;padding-right: 7px">
                            &nbsp;
                          </td>
                        </tr>
                      </table>
                      
                      <p style="text-align: center">
                        <span style="font-size: 18pt;text-decoration: underline;color: #0070c0"><strong>DNS VERIFICATION LOGIC </strong></span>
                      </p>
                      
                      <p>
                        <span style="font-size: 10pt">The <strong>Microsoft Azure Web Sites</strong> DNS verification logic has 2 steps: </span>
                      </p>
                      
                      <ul>
                        <li>
                          <span style="font-size: 10pt">First we try to validate using <strong>CNAME</strong>. That means we look whether the custom domain provided is a <strong>CNAME</strong> record. If it is, then it is expanded. If the next record in the chain is also a <strong>CNAME</strong>, it is further expanded. The expansion goes on until we get an <strong>A record</strong> or something ending with &#8220;<strong>azurewebsites.net</strong>&#8220;. If it is found that the custom domain is eventually pointing to <strong><SITENAME>.azurewebsites.net</strong>, it is verified that the <strong><SITENAME></strong> is really the site for which the custom domain is being added and verification is done. </span>
                        </li>
                      </ul>
                      
                      <ul>
                        <li>
                          <span style="font-size: 10pt;font-family: segoe ui">If for some reason the validation of the <strong>CNAME</strong> fails, it proceeds with the alternative validation. That is useful for users when they want to just test their sites, but not really point the record to <strong>AZURE</strong>, or if it is a naked domain (some <strong>DNS registrars</strong> don&#8217;t support a <strong>CNAME</strong> for such hostname). The alternative validation puts &#8220;<strong>awverify</strong>&#8221; in front of the provided hostname and follows up the similar logic as above. The only difference is that this time the target has to be the <strong>awverify.<SITENAME>.azurewebsites.net</strong>. </span>
                        </li>
                      </ul>
                      
                      <p>
                        <span style="font-size: 10pt;font-family: segoe ui"><strong>TXT records</strong> are also supported. It is another alternative, because some DNS registrars don&#8217;t support <strong>CNAME&#8217;s</strong> pointing to invalid hostnames (the &#8220;<strong>awverify</strong>&#8221; version doesn&#8217;t truly exist). So one can also create just a <strong>TXT record</strong> instead of a <strong>CNAME</strong> (otherwise it is completely same setup as in validations above). </span>
                      </p>
                      
                      <p>
                        <span style="font-size: 10pt;font-family: segoe ui">Thanks to <strong>Petr Podhorsky</strong> (<strong>DEV</strong> on <strong>MICROSOFT AZURE WEB SITES</strong>) for sharing the <strong>DNS verification logic</strong>with us.</span>
                      </p>
                      
                      <table style="border-collapse: collapse" border="0">
                        <colgroup> <col style="width: 973px"></colgroup> <tr>
                          <td style="border-top: #0070c0 4.5pt solid;padding-left: 7px;padding-right: 7px">
                            &nbsp;
                          </td>
                        </tr>
                      </table>