---
id: 153
title: Central Certificate Store (CCS) with IIS 8 (Windows Server 2012)
date: 2012-10-11T03:23:32+00:00
author: kaushal
layout: post
guid: https://blogs.msdn.microsoft.com/kaushal/2012/10/11/central-certificate-store-ccs-with-iis-8-windows-server-2012/
permalink: /2012/10/11/central-certificate-store-ccs-with-iis-8-windows-server-2012/
orig_url:
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2012/10/11/central-certificate-store-ccs-with-iis-8-windows-server-2012.aspx
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2012/10/11/central-certificate-store-ccs-with-iis-8-windows-server-2012.aspx
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2012/10/11/central-certificate-store-ccs-with-iis-8-windows-server-2012.aspx
orig_site_id:
  - "13803"
  - "13803"
  - "13803"
orig_post_id:
  - "10358706"
  - "10358706"
  - "10358706"
orig_parent_id:
  - "10358706"
  - "10358706"
  - "10358706"
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
  - http://blogs.msdn.com/b/kaushal/archive/2012/10/11/central-certificate-store-ccs-with-iis-8-windows-server-2012.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2012/10/11/central-certificate-store-ccs-with-iis-8-windows-server-2012.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2012/10/11/central-certificate-store-ccs-with-iis-8-windows-server-2012.aspx
orig_post_name:
  - central certificate store ccs with iis 8 windows server 2012
  - central certificate store ccs with iis 8 windows server 2012
  - central certificate store ccs with iis 8 windows server 2012
orig_thread_id:
  - "823517"
  - "823517"
  - "823517"
orig_post_author_email:
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
orig_attachment_count:
  - "0"
  - "0"
  - "0"
total_views:
  - "28970"
  - "28970"
  - "28970"
opengraph_tags:
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Central Certificate Store (CCS) with IIS 8 (Windows Server 2012)" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/10/11/central-certificate-store-ccs-with-iis-8-windows-server-2012/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="In my previous posts on IIS 8, I discussed how scalability was&#160; achieved in IIS 8 via SNI. Below are the links to previous posts: &#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; ·&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; SSL Scalability with IIS 8 &#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; ·&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; SNI with IIS 8 In the first post I mentioned that scalability was achieved in IIS via Server Name Indication (SNI)..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4784.image_thumb_41B1B362.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Central Certificate Store (CCS) with IIS 8 (Windows Server 2012)" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/10/11/central-certificate-store-ccs-with-iis-8-windows-server-2012/" />
    <meta name="twitter:description" content="In my previous posts on IIS 8, I discussed how scalability was&#160; achieved in IIS 8 via SNI. Below are the links to previous posts: &#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; ·&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; SSL Scalability with IIS 8 &#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; ·&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; SNI with IIS 8 In the first post I mentioned that scalability was achieved in IIS via Server Name Indication (SNI)..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4784.image_thumb_41B1B362.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Central Certificate Store (CCS) with IIS 8 (Windows Server 2012)" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/10/11/central-certificate-store-ccs-with-iis-8-windows-server-2012/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="In my previous posts on IIS 8, I discussed how scalability was&#160; achieved in IIS 8 via SNI. Below are the links to previous posts: &#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; ·&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; SSL Scalability with IIS 8 &#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; ·&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; SNI with IIS 8 In the first post I mentioned that scalability was achieved in IIS via Server Name Indication (SNI)..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4784.image_thumb_41B1B362.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Central Certificate Store (CCS) with IIS 8 (Windows Server 2012)" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/10/11/central-certificate-store-ccs-with-iis-8-windows-server-2012/" />
    <meta name="twitter:description" content="In my previous posts on IIS 8, I discussed how scalability was&#160; achieved in IIS 8 via SNI. Below are the links to previous posts: &#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; ·&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; SSL Scalability with IIS 8 &#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; ·&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; SNI with IIS 8 In the first post I mentioned that scalability was achieved in IIS via Server Name Indication (SNI)..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4784.image_thumb_41B1B362.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Central Certificate Store (CCS) with IIS 8 (Windows Server 2012)" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/10/11/central-certificate-store-ccs-with-iis-8-windows-server-2012/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="In my previous posts on IIS 8, I discussed how scalability was&#160; achieved in IIS 8 via SNI. Below are the links to previous posts: &#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; ·&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; SSL Scalability with IIS 8 &#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; ·&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; SNI with IIS 8 In the first post I mentioned that scalability was achieved in IIS via Server Name Indication (SNI)..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4784.image_thumb_41B1B362.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Central Certificate Store (CCS) with IIS 8 (Windows Server 2012)" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/10/11/central-certificate-store-ccs-with-iis-8-windows-server-2012/" />
    <meta name="twitter:description" content="In my previous posts on IIS 8, I discussed how scalability was&#160; achieved in IIS 8 via SNI. Below are the links to previous posts: &#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; ·&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; SSL Scalability with IIS 8 &#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; ·&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; SNI with IIS 8 In the first post I mentioned that scalability was achieved in IIS via Server Name Indication (SNI)..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4784.image_thumb_41B1B362.png" />
    
categories:
  - Uncategorized
tags:
  - CCS
  - Central Certificate Store
  - IIS 8
  - Scalability
  - SSL
---
<font size="2" face="Segoe UI">In my previous posts on IIS 8, I discussed how scalability was&#160; achieved in IIS 8 via SNI.</font>

<font size="2" face="Segoe UI">Below are the links to previous posts:</font>

> <p class="MsoListParagraphCxSpFirst" style="line-height: 115%; text-indent: -18pt; margin-bottom: 6pt; mso-list: l1 level1 lfo5; mso-add-space: auto;">
>   <!--[if !supportLists]-->
>   
>   <span lang="EN" style="line-height: 115%; font-family: symbol; font-size: 10pt; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol; mso-ansi-language: en;"><span style="mso-list: ignore;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; ·<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
>   
>   <span lang="EN" style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-ansi-language: en;"><a href="http://blogs.msdn.com/b/kaushal/archive/2012/08/08/ssl-scalability-with-iis-8-windows-8-server.aspx" target="_blank" rel="noopener noreferrer">SSL Scalability with IIS 8</a><o:p></o:p></span>
> </p>
> 
> <p class="MsoListParagraphCxSpLast" style="line-height: 115%; text-indent: -18pt; margin-bottom: 6pt; mso-list: l1 level1 lfo5; mso-add-space: auto;">
>   <!--[if !supportLists]-->
>   
>   <span lang="EN" style="line-height: 115%; font-family: symbol; font-size: 10pt; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol; mso-ansi-language: en;"><span style="mso-list: ignore;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span><span lang="EN" style="line-height: 115%; font-family: symbol; font-size: 10pt; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol; mso-ansi-language: en;"><span style="mso-list: ignore;">·<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
>   
>   <span lang="EN" style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-ansi-language: en;"><a href="http://blogs.msdn.com/b/kaushal/archive/2012/09/04/server-name-indication-sni-in-iis-8-windows-server-2012.aspx" target="_blank" rel="noopener noreferrer">SNI with IIS 8</a></span>
> </p>

<font size="2" face="Segoe UI">In the first post I mentioned that scalability was achieved in IIS via <strong>Server Name Indication</strong> (<strong>SNI</strong>) and <strong>Central Certificate Store</strong> (<strong>CCS</strong>). In my second post linked above I discussed how scalability was achieved via SNI.</font>

<font size="2" face="Segoe UI">In this article I’ll discuss <strong>CCS</strong> in detail and also its functionality.</font>

* * *

<font size="4" face="Segoe UI"><u><strong>What is CCS</strong>?</u></font>

<font size="2" face="Segoe UI"><strong>Central Certificate Store</strong> or <strong>Centralized SSL Certificate Support</strong> is a feature which allows certificates to be stored on a central location like a <strong>file share</strong>. This feature is very similar to Shared Configuration, where the certificates are stored on a file share and the servers in farm load them on demand.</font>

<font size="2" face="Segoe UI">In <strong>CCS</strong> the files are exported along with the private key (in <strong>.pfx</strong> format) and stored centrally on a file share. Files are named specifically using a naming convention and stored in the file share which are loaded on demand basis for an incoming SSL request. <font style="background-color: rgb(143, 176, 140);"><strong>CCS </strong>uses the <strong>Server Name Indication</strong> information from the <strong>Client Hello</strong> for functionality</font>.</font>

<font size="4" face="Segoe UI"><u><strong>Why do we need CCS when we already have SNI</strong>?</u></font>

<font size="2" face="Segoe UI">While <strong>SNI</strong> addressed only the <strong>SSL scalability</strong> problem with <strong>IIS</strong>, <strong>CCS </strong>addresses both <strong>SSL scalability</strong> and <strong>manageability </strong>of the certificates.</font>

<font size="2" face="Segoe UI">Also consider a hosting scenario where typically there are close to 1000 sites. If all of these were SSL enabled, then there would be close to 1000 SSL bindings. These explicit bindings are specific to a site and are loaded in memory during start-up of IIS Services. In case of CCS there exists only binding and the certs are loaded on demand and cached for future use, this way the memory consumption is lesser and there is a slight performance gain.</font>

<font size="4" face="Segoe UI"><strong><u>How does CCS improve manageability of Certificates?</u></strong></font>

<font size="2" face="Segoe UI">Prior to IIS 8, IIS always picked up the certificates store (<strong>Personal </strong>store of <strong>MY Computer </strong>account) which is local to every machine. In case of a stand-alone server this is not a problem. However, consider a web-farm scenario with 2 or more servers in the farm. If one has to configure a site to use SSL, the certificate has to be installed on all the servers along with the private key. If the certificate expires, again the same step has to be repeated on all the servers. So there was lot of manual work involved. If there were more servers in the farm or if you were to introduce another SSL site, it would be a bigger headache for the server admins.</font>

<font size="2" face="Segoe UI">In the server farm, we configure all the servers to use the <strong>CCS </strong>binding which reads from this <strong>Central Certificate Store</strong>. Now IIS picks the certificate from the file share and not the local certificate store. The server admins have the task simplified and they need to install/renew the certificate on a single location i.e., the file share.</font>

* * *

<font face="Segoe UI"></font> </p> 

<p align="center">
  <font color="#4bacc6" size="5" face="Segoe UI"><strong><u>Installing CCS</u></strong></font>
</p>

<font size="2" face="Segoe UI">Unlike <strong>SNI</strong>, <strong>CCS </strong>is not pre-installed it has to be installed separately. It is shipped as a <strong>native module</strong> and has to be installed via the <strong>Server Manager</strong> console on Windows Server 2012 & via <strong>Programs & Features </strong>on Windows 8. Below are instructions to </font>

<font face="Segoe UI"><font style="background-color: rgb(255, 255, 255);" size="4"><u><strong>Installing CCS on Windows Server 2012:</strong></u></font></font>

> <p class="MsoListParagraphCxSpFirst" style="text-indent: -18pt; mso-list: l0 level1 lfo1;">
>   <!--[if !supportLists]-->
>   
>   <span style="line-height: 105%; font-family: symbol; font-size: 10pt; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol;"><span style="mso-list: ignore;">·<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
>   
>   <span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">Launch Server Manager.<o:p></o:p></span>
> </p>
> 
> <p class="MsoListParagraphCxSpMiddle" style="text-indent: -18pt; mso-list: l0 level1 lfo1;">
>   <!--[if !supportLists]-->
>   
>   <span style="line-height: 105%; font-family: symbol; font-size: 10pt; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol;"><span style="mso-list: ignore;">·<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
>   
>   <span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">Under Manage menu, select Add Roles and Features:</span>
> </p>
> 
> <p class="MsoListParagraphCxSpMiddle" style="text-indent: -18pt; mso-list: l0 level1 lfo1;">
>   &#160;&#160;&#160;&#160;&#160;&#160;&#160; <a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3704.image_36689F25.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/3704.image_5F00_36689F25.png"><img title="image" style="display: inline; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4784.image_thumb_41B1B362.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/4784.image_5F00_thumb_5F00_41B1B362.png" width="550" height="340" /></a>
> </p>
> 
> <p class="MsoListParagraphCxSpMiddle" style="text-indent: -18pt; mso-list: l0 level1 lfo1;">
>   <!--[if !supportLists]-->
>   
>   <span style="line-height: 105%; font-family: symbol; font-size: 10pt; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol;"><span style="mso-list: ignore;">·<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
>   
>   <span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">In "<strong>Add Roles and Features Wizard</strong>" click "<strong>Next</strong>".<o:p></o:p></span>
> </p>
> 
> <p class="MsoListParagraphCxSpMiddle" style="text-indent: -18pt; mso-list: l0 level1 lfo1;">
>   <!--[if !supportLists]-->
>   
>   <span style="line-height: 105%; font-family: symbol; font-size: 10pt; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol;"><span style="mso-list: ignore;">·<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
>   
>   <span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">Select "<strong>Role-based or Feature-based Installation</strong>" and click on Next.<o:p></o:p></span>
> </p>
> 
> <p class="MsoListParagraphCxSpMiddle" style="text-indent: -18pt; mso-list: l0 level1 lfo1;">
>   <!--[if !supportLists]-->
>   
>   <span style="line-height: 105%; font-family: symbol; font-size: 10pt; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol;"><span style="mso-list: ignore;">·<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
>   
>   <span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">Select the appropriate server (local is selected by default) and click on Next.<o:p></o:p></span>
> </p>
> 
> <p class="MsoListParagraphCxSpMiddle" style="text-indent: -18pt; mso-list: l0 level1 lfo1;">
>   <!--[if !supportLists]-->
>   
>   <span style="line-height: 105%; font-family: symbol; font-size: 10pt; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol;"><span style="mso-list: ignore;">·<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
>   
>   <span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">Select Web Server (IIS):</span>
> </p>
> 
> <p class="MsoListParagraphCxSpMiddle" style="text-indent: -18pt; mso-list: l0 level1 lfo1;">
>   &#160;&#160;&#160;&#160;&#160;&#160;&#160; <a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/1134.image_067DD797.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/1134.image_5F00_067DD797.png"><img title="image" style="display: inline; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8475.image_thumb_76225FDD.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/8475.image_5F00_thumb_5F00_76225FDD.png" width="543" height="404" /></a>
> </p>
> 
> <p class="MsoListParagraphCxSpMiddle" style="text-indent: -18pt; mso-list: l0 level1 lfo1;">
>   <!--[if !supportLists]-->
>   
>   <span style="line-height: 105%; font-family: symbol; font-size: 10pt; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol;"><span style="mso-list: ignore;">·<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
>   
>   <span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">No additional features are needed for IIS, so click "<strong>Next</strong>".<o:p></o:p></span>
> </p>
> 
> <p class="MsoListParagraphCxSpMiddle" style="text-indent: -18pt; mso-list: l0 level1 lfo1;">
>   <!--[if !supportLists]-->
>   
>   <span style="line-height: 105%; font-family: symbol; font-size: 10pt; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol;"><span style="mso-list: ignore;">·<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
>   
>   <span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">Click on Next again.<o:p></o:p></span>
> </p>
> 
> <p class="MsoListParagraphCxSpMiddle" style="text-indent: -18pt; mso-list: l0 level1 lfo1;">
>   <!--[if !supportLists]-->
>   
>   <span style="line-height: 105%; font-family: symbol; font-size: 10pt; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol;"><span style="mso-list: ignore;">·<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
>   
>   <span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">By default, Centralized Certificates is not selected. Expand Security and then select "<strong>Centralized SSL Certificates Support</strong>" and click on Next.</span>
> </p>
> 
> <p class="MsoListParagraphCxSpMiddle" style="text-indent: -18pt; mso-list: l0 level1 lfo1;">
>   &#160;&#160;&#160;&#160;&#160;&#160;&#160; <a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4375.image_7AB86A97.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/4375.image_5F00_7AB86A97.png"><img title="image" style="display: inline; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/2625.image_thumb_2A26D964.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/2625.image_5F00_thumb_5F00_2A26D964.png" width="546" height="407" /></a>
> </p>
> 
> <p class="MsoListParagraphCxSpMiddle" style="text-indent: -18pt; mso-list: l0 level1 lfo1;">
>   <!--[if !supportLists]-->
>   
>   <span style="line-height: 105%; font-family: symbol; font-size: 10pt; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol;"><span style="mso-list: ignore;">·<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
>   
>   <span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">Click on Install and wait until the installation completes.<o:p></o:p></span>
> </p>
> 
> <p class="MsoListParagraphCxSpLast" style="text-indent: -18pt; mso-list: l0 level1 lfo1;">
>   <!--[if !supportLists]-->
>   
>   <font face="Segoe UI"><span style="line-height: 105%; font-family: symbol; font-size: 10pt; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol;"><span style="mso-list: ignore;">·<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
>   
>   <span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">Upon successful installation the wizard would reflect the status:</span></font>
> </p>
> 
> <p class="MsoListParagraphCxSpLast" style="text-indent: -18pt; mso-list: l0 level1 lfo1;">
>   <a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/1184.image_0FBF671D.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/1184.image_5F00_0FBF671D.png"><font face="Segoe UI"></font></a>&#160;&#160;&#160;&#160;&#160;&#160;&#160; <font face="Segoe UI"><a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/2577.image_263205A4.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/2577.image_5F00_263205A4.png"><img title="image" style="display: inline; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6428.image_thumb_50E4C9D7.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/6428.image_5F00_thumb_5F00_50E4C9D7.png" width="544" height="405" /></a></font>
> </p>

<p class="MsoListParagraphCxSpLast" style="text-indent: -18pt; mso-list: l0 level1 lfo1;">
  <font face="Segoe UI"><font style="background-color: rgb(255, 255, 255);"><font size="3"><u><strong></strong></u></font></font></font>
</p>

<p class="MsoListParagraphCxSpLast" style="text-indent: -18pt; mso-list: l0 level1 lfo1;">
  <font face="Segoe UI"><font style="background-color: rgb(255, 255, 255);"><font size="3"><u><strong></strong></u></font></font></font>
</p>

> <p class="MsoListParagraphCxSpLast" style="text-indent: -18pt; mso-list: l0 level1 lfo1;">
>   <font size="4" face="Segoe UI"><strong><u>Installing CCS on Windows 8:</u></strong></font>
> </p>
> 
> <p class="MsoListParagraphCxSpFirst" style="line-height: 115%; text-indent: -18pt; margin-bottom: 6pt; mso-list: l0 level1 lfo3; mso-add-space: auto;">
>   <!--[if !supportLists]-->
>   
>   <span style="line-height: 115%; font-family: symbol; font-size: 10pt; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol;"><span style="mso-list: ignore;">·<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
>   
>   <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">Go to run prompt, type "<span class="SpellE"><b style="mso-bidi-font-weight: normal;">appwiz.cpl</b></span>", and hit <b style="mso-bidi-font-weight: normal;">Enter</b> key.<o:p></o:p></span>
> </p>
> 
> <p class="MsoListParagraphCxSpMiddle" style="line-height: 115%; text-indent: -18pt; margin-bottom: 6pt; mso-list: l0 level1 lfo3; mso-add-space: auto;">
>   <!--[if !supportLists]-->
>   
>   <span style="line-height: 115%; font-family: symbol; font-size: 10pt; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol;"><span style="mso-list: ignore;">·<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
>   
>   <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">This would launch the Programs and Features Console.<o:p></o:p></span>
> </p>
> 
> <p class="MsoListParagraphCxSpMiddle" style="line-height: 115%; text-indent: -18pt; margin-bottom: 6pt; mso-list: l0 level1 lfo3; mso-add-space: auto;">
>   <!--[if !supportLists]-->
>   
>   <span style="line-height: 115%; font-family: symbol; font-size: 10pt; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol;"><span style="mso-list: ignore;">·<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
>   
>   <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">Click on "<b style="mso-bidi-font-weight: normal;">Turn Windows features on or off</b>".<o:p></o:p></span>
> </p>
> 
> <p class="MsoListParagraphCxSpMiddle" style="line-height: 115%; text-indent: -18pt; margin-bottom: 6pt; mso-list: l0 level1 lfo3; mso-add-space: auto;">
>   <!--[if !supportLists]-->
>   
>   <span style="line-height: 115%; font-family: symbol; font-size: 10pt; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol;"><span style="mso-list: ignore;">·<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
>   
>   <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">Select "<b style="mso-bidi-font-weight: normal;">Internet Information Services</b>" and expand the tree.</span>
> </p>
> 
> <p class="MsoListParagraphCxSpMiddle" style="line-height: 115%; text-indent: -18pt; margin-bottom: 6pt; mso-list: l0 level1 lfo3; mso-add-space: auto;">
>   &#160;&#160;&#160;&#160;&#160;&#160;&#160; <a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/1541.image_2EACBE51.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/1541.image_5F00_2EACBE51.png"><img title="image" style="display: inline; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4452.image_thumb_64CE36A0.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/4452.image_5F00_thumb_5F00_64CE36A0.png" width="501" height="317" /></a>
> </p>
> 
> <p class="MsoListParagraphCxSpMiddle" style="line-height: 115%; text-indent: -18pt; margin-bottom: 6pt; mso-list: l0 level1 lfo3; mso-add-space: auto;">
>   <!--[if !supportLists]-->
>   
>   <span style="line-height: 115%; font-family: symbol; font-size: 10pt; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol;"><span style="mso-list: ignore;">·<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
>   
>   <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">Go to World Web Wide Services->Security<o:p></o:p></span>
> </p>
> 
> <p class="MsoListParagraphCxSpMiddle" style="line-height: 115%; text-indent: -18pt; margin-bottom: 6pt; mso-list: l0 level1 lfo3; mso-add-space: auto;">
>   <!--[if !supportLists]-->
>   
>   <span style="line-height: 115%; font-family: symbol; font-size: 10pt; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol;"><span style="mso-list: ignore;">·<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
>   
>   <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">Select "<b style="mso-bidi-font-weight: normal;">Centralized SSL Certificate Support</b>" and click on ok.</span>
> </p>
> 
> <p class="MsoListParagraphCxSpMiddle" style="line-height: 115%; text-indent: -18pt; margin-bottom: 6pt; mso-list: l0 level1 lfo3; mso-add-space: auto;">
>   &#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; <a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6835.image_026011A0.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/6835.image_5F00_026011A0.png"><img title="image" style="display: inline; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/7180.image_thumb_2C7F99BB.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/7180.image_5F00_thumb_5F00_2C7F99BB.png" width="433" height="516" /></a>
> </p>
> 
> <p class="MsoListParagraphCxSpLast" style="line-height: 115%; text-indent: -18pt; margin-bottom: 6pt; mso-list: l0 level1 lfo3; mso-add-space: auto;">
>   <!--[if !supportLists]-->
>   
>   <span style="line-height: 115%; font-family: symbol; font-size: 10pt; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol;"><span style="mso-list: ignore;">·<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
>   
>   <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">Centralized Certificates is installed successfully.</span>
> </p>

* * *

> <p class="MsoListParagraphCxSpLast" style="line-height: 115%; text-indent: -18pt; margin-bottom: 6pt; mso-list: l0 level1 lfo3; mso-add-space: auto;" align="center">
>   <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;"><strong><font color="#4f81bd" size="5"><u>Configuring Central Certificate Store</u></font></strong></span>
> </p>

<p class="MsoListParagraphCxSpLast" style="line-height: 115%; text-indent: -18pt; margin-bottom: 6pt; mso-list: l0 level1 lfo3; mso-add-space: auto;">
  <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;"><strong><u><font size="2"></font></u></strong></span>
</p>

<p class="MsoListParagraphCxSpFirst" style="margin: 0cm 0cm 6pt 54pt; line-height: 115%; text-indent: -36pt; mso-list: l0 level1 lfo7; mso-add-space: auto;">
  <!--[if !supportLists]-->
  
  <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Segoe UI&quot;;"><span style="mso-list: ignore;">1.<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
  
  <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">Launch IIS Manager.<o:p></o:p></span>
</p>

<p class="MsoListParagraphCxSpMiddle" style="margin: 0cm 0cm 6pt 54pt; line-height: 115%; text-indent: -36pt; mso-list: l0 level1 lfo7; mso-add-space: auto;">
  <!--[if !supportLists]-->
  
  <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Segoe UI&quot;;"><span style="mso-list: ignore;">2.<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
  
  <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">Under "<strong>Connections</strong>" select <<span class="SpellE">MachineName</span>>.</span>
</p>

<p class="MsoListParagraphCxSpMiddle" style="margin: 0cm 0cm 6pt 54pt; line-height: 115%; text-indent: -36pt; mso-list: l0 level1 lfo7; mso-add-space: auto;">
  &#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; <a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3660.image_50584B48.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/3660.image_5F00_50584B48.png"><img title="image" style="display: inline; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4846.image_thumb_71884124.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/4846.image_5F00_thumb_5F00_71884124.png" width="246" height="243" /></a>
</p>

<p class="MsoListParagraphCxSpMiddle" style="margin: 0cm 0cm 6pt 54pt; line-height: 115%; text-indent: -36pt; mso-list: l0 level1 lfo7; mso-add-space: auto;">
  <!--[if !supportLists]-->
  
  <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Segoe UI&quot;;"><span style="mso-list: ignore;">3.<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
  
  <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">In the middle-pane, under "<strong>Management</strong>", double-click on "<strong>Centralized Certificates</strong>"</span>
</p>

> <p class="MsoListParagraphCxSpMiddle" style="margin: 0cm 0cm 6pt 54pt; line-height: 115%; text-indent: -36pt; mso-list: l0 level1 lfo7; mso-add-space: auto;">
>   &#160;&#160;&#160; <a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/0647.image_2FA15BD6.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/0647.image_5F00_2FA15BD6.png"><img title="image" style="display: inline; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/1526.image_thumb_1BA7C940.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/1526.image_5F00_thumb_5F00_1BA7C940.png" width="290" height="115" /></a>
> </p>

<p class="MsoListParagraphCxSpMiddle" style="margin: 0cm 0cm 6pt 54pt; line-height: 115%; text-indent: -36pt; mso-list: l0 level1 lfo7; mso-add-space: auto;">
  <!--[if !supportLists]-->
  
  <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Segoe UI&quot;;"><span style="mso-list: ignore;">4.<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
  
  <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">Under "<strong>Actions</strong>" pane select <strong>Edit Feature Settings</strong>:</span>
</p>

> <p class="MsoListParagraphCxSpMiddle" style="margin: 0cm 0cm 6pt 54pt; line-height: 115%; text-indent: -36pt; mso-list: l0 level1 lfo7; mso-add-space: auto;">
>   &#160;&#160;&#160; <a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/1220.image_6C09AAB3.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/1220.image_5F00_6C09AAB3.png"><img title="image" style="display: inline; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/2100.image_thumb_30D5CEE8.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/2100.image_5F00_thumb_5F00_30D5CEE8.png" width="244" height="246" /></a>
> </p>

<p class="MsoListParagraphCxSpMiddle" style="margin: 0cm 0cm 6pt 54pt; line-height: 115%; text-indent: -36pt; mso-list: l0 level1 lfo7; mso-add-space: auto;">
  <!--[if !supportLists]-->
  
  <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Segoe UI&quot;;"><span style="mso-list: ignore;">5.<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
  
  <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">Select the check box "<strong>Enable Centralized Certificates</strong>" and provide the following details:</span>
</p>

> <p class="MsoListParagraphCxSpMiddle" style="margin: 0cm 0cm 6pt 54pt; line-height: 115%; text-indent: -36pt; mso-list: l0 level1 lfo7; mso-add-space: auto;">
>   &#160;&#160;&#160; <a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/5417.image_44168587.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/5417.image_5F00_44168587.png"><img title="image" style="display: inline; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6813.image_thumb_4603D490.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/6813.image_5F00_thumb_5F00_4603D490.png" width="473" height="467" /></a>
> </p>

<table class="MsoTableColorfulListAccent5" style="border: currentcolor; width: 364.35pt; margin-left: 24pt; border-collapse: collapse; mso-border-alt: solid #31849b 3.0pt; mso-border-themecolor: accent5; mso-border-themeshade: 191; mso-yfti-tbllook: 1184; mso-padding-alt: 0cm 5.4pt 0cm 5.4pt; mso-border-insideh: 3.0pt solid #31849b; mso-border-insideh-themecolor: accent5; mso-border-insideh-themeshade: 191; mso-border-insidev: 3.0pt solid #31849b; mso-border-insidev-themecolor: accent5; mso-border-insidev-themeshade: 191;" cellspacing="0" cellpadding="0" width="486" align="center" border="1">
  <tr style="height: 37.7pt; mso-yfti-irow: -1; mso-yfti-firstrow: yes;">
    <td style="background: rgb(242, 115, 10); padding: 0cm 5.4pt; border: 3pt solid rgb(49, 132, 155); width: 109.2pt; height: 37.7pt; mso-border-themecolor: accent5; mso-border-themeshade: 191; mso-background-themecolor: accent6; mso-background-themeshade: 204;" width="146">
      <p align="center">
        <b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-themecolor: background1;">Element Name</span></b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-themecolor: background1;"><o:p></o:p></span>
      </p>
    </td>
    
    <td style="background: rgb(242, 115, 10); border-width: 3pt 3pt 3pt medium; border-style: solid solid solid none; border-color: rgb(49, 132, 155) rgb(49, 132, 155) rgb(49, 132, 155) currentcolor; padding: 0cm 5.4pt; width: 9cm; height: 37.7pt; mso-border-themecolor: accent5; mso-border-themeshade: 191; mso-background-themecolor: accent6; mso-background-themeshade: 204; mso-border-left-alt: solid #31849b 3.0pt; mso-border-left-themecolor: accent5; mso-border-left-themeshade: 191;" width="340">
      <p align="center">
        <b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-themecolor: background1;">Description</span></b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-themecolor: background1;"><o:p></o:p></span>
      </p>
    </td>
  </tr>
  
  <tr style="height: 35.1pt; mso-yfti-irow: 0;">
    <td style="background: rgb(218, 238, 243); border-width: medium 3pt 3pt; border-style: none solid solid; border-color: currentcolor rgb(49, 132, 155) rgb(49, 132, 155); padding: 0cm 5.4pt; width: 109.2pt; height: 35.1pt; mso-border-themecolor: accent5; mso-border-themeshade: 191; mso-background-themecolor: accent5; mso-border-top-alt: solid #31849b 3.0pt; mso-border-top-themecolor: accent5; mso-border-top-themeshade: 191; mso-background-themetint: 51;" width="146">
      <p class="MsoNormal" style="text-align: center; mso-yfti-cnfc: 68; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto;" align="center">
        <b><span style="color: black; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 9pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-themecolor: text1; mso-bidi-font-size: 12.0pt;">Enable Centralized Certificates<o:p></o:p></span></b>
      </p>
    </td>
    
    <td style="background: rgb(218, 238, 243); border-width: medium 3pt 3pt medium; border-style: none solid solid none; border-color: currentcolor rgb(49, 132, 155) rgb(49, 132, 155) currentcolor; padding: 0cm 5.4pt; width: 9cm; height: 35.1pt; mso-background-themecolor: accent5; mso-border-left-alt: solid #31849b 3.0pt; mso-border-left-themecolor: accent5; mso-border-left-themeshade: 191; mso-border-top-alt: solid #31849b 3.0pt; mso-border-top-themecolor: accent5; mso-border-top-themeshade: 191; mso-background-themetint: 51; mso-border-bottom-themecolor: accent5; mso-border-bottom-themeshade: 191; mso-border-right-themecolor: accent5; mso-border-right-themeshade: 191;" width="340">
      <p class="MsoNormal" style="mso-yfti-cnfc: 64; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto;">
        <span style="color: black; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 9pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-themecolor: text1; mso-bidi-font-size: 12.0pt;">Select the <b>Enable Centralized Certificates</b> check box if you want to create a central certificate store for your web farm. Otherwise, clear the check box.<o:p></o:p></span>
      </p>
    </td>
  </tr>
  
  <tr style="height: 24.05pt; mso-yfti-irow: 1;">
    <td style="background: rgb(237, 246, 249); border-width: medium 3pt 3pt; border-style: none solid solid; border-color: currentcolor rgb(49, 132, 155) rgb(49, 132, 155); padding: 0cm 5.4pt; width: 109.2pt; height: 24.05pt; mso-border-themecolor: accent5; mso-border-themeshade: 191; mso-background-themecolor: accent5; mso-border-top-alt: solid #31849b 3.0pt; mso-border-top-themecolor: accent5; mso-border-top-themeshade: 191; mso-background-themetint: 25;" width="146">
      <p class="MsoNormal" style="text-align: center; mso-yfti-cnfc: 4; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto;" align="center">
        <b><span style="color: black; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 9pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-themecolor: text1; mso-bidi-font-size: 12.0pt;">Physical path<o:p></o:p></span></b>
      </p>
    </td>
    
    <td style="background: rgb(237, 246, 249); border-width: medium 3pt 3pt medium; border-style: none solid solid none; border-color: currentcolor rgb(49, 132, 155) rgb(49, 132, 155) currentcolor; padding: 0cm 5.4pt; width: 9cm; height: 24.05pt; mso-background-themecolor: accent5; mso-border-left-alt: solid #31849b 3.0pt; mso-border-left-themecolor: accent5; mso-border-left-themeshade: 191; mso-border-top-alt: solid #31849b 3.0pt; mso-border-top-themecolor: accent5; mso-border-top-themeshade: 191; mso-background-themetint: 25; mso-border-bottom-themecolor: accent5; mso-border-bottom-themeshade: 191; mso-border-right-themecolor: accent5; mso-border-right-themeshade: 191;" width="340">
      <p class="MsoNormal" style="mso-margin-top-alt: auto; mso-margin-bottom-alt: auto;">
        <span style="color: black; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 9pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-themecolor: text1; mso-bidi-font-size: 12.0pt;">Type the physical path to the directory on the central certificate store server where you want the certificates stored.<o:p></o:p></span>
      </p>
    </td>
  </tr>
  
  <tr style="height: 23.35pt; mso-yfti-irow: 2;">
    <td style="background: rgb(218, 238, 243); border-width: medium 3pt 3pt; border-style: none solid solid; border-color: currentcolor rgb(49, 132, 155) rgb(49, 132, 155); padding: 0cm 5.4pt; width: 109.2pt; height: 23.35pt; mso-border-themecolor: accent5; mso-border-themeshade: 191; mso-background-themecolor: accent5; mso-border-top-alt: solid #31849b 3.0pt; mso-border-top-themecolor: accent5; mso-border-top-themeshade: 191; mso-background-themetint: 51;" width="146">
      <p class="MsoNormal" style="text-align: center; mso-yfti-cnfc: 68; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto;" align="center">
        <b><span style="color: black; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 9pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-themecolor: text1; mso-bidi-font-size: 12.0pt;">User name<o:p></o:p></span></b>
      </p>
    </td>
    
    <td style="background: rgb(218, 238, 243); border-width: medium 3pt 3pt medium; border-style: none solid solid none; border-color: currentcolor rgb(49, 132, 155) rgb(49, 132, 155) currentcolor; padding: 0cm 5.4pt; width: 9cm; height: 23.35pt; mso-background-themecolor: accent5; mso-border-left-alt: solid #31849b 3.0pt; mso-border-left-themecolor: accent5; mso-border-left-themeshade: 191; mso-border-top-alt: solid #31849b 3.0pt; mso-border-top-themecolor: accent5; mso-border-top-themeshade: 191; mso-background-themetint: 51; mso-border-bottom-themecolor: accent5; mso-border-bottom-themeshade: 191; mso-border-right-themecolor: accent5; mso-border-right-themeshade: 191;" width="340">
      <p class="MsoNormal" style="mso-yfti-cnfc: 64; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto;">
        <span style="color: black; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 9pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-themecolor: text1; mso-bidi-font-size: 12.0pt;">Type the name of the user account to use when accessing the central certificate store.<o:p></o:p></span>
      </p>
    </td>
  </tr>
  
  <tr style="height: 19.75pt; mso-yfti-irow: 3;">
    <td style="background: rgb(237, 246, 249); border-width: medium 3pt 3pt; border-style: none solid solid; border-color: currentcolor rgb(49, 132, 155) rgb(49, 132, 155); padding: 0cm 5.4pt; width: 109.2pt; height: 19.75pt; mso-border-themecolor: accent5; mso-border-themeshade: 191; mso-background-themecolor: accent5; mso-border-top-alt: solid #31849b 3.0pt; mso-border-top-themecolor: accent5; mso-border-top-themeshade: 191; mso-background-themetint: 25;" width="146">
      <p class="MsoNormal" style="text-align: center; mso-yfti-cnfc: 4; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto;" align="center">
        <b><span style="color: black; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 9pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-themecolor: text1; mso-bidi-font-size: 12.0pt;">Password<o:p></o:p></span></b>
      </p>
    </td>
    
    <td style="background: rgb(237, 246, 249); border-width: medium 3pt 3pt medium; border-style: none solid solid none; border-color: currentcolor rgb(49, 132, 155) rgb(49, 132, 155) currentcolor; padding: 0cm 5.4pt; width: 9cm; height: 19.75pt; mso-background-themecolor: accent5; mso-border-left-alt: solid #31849b 3.0pt; mso-border-left-themecolor: accent5; mso-border-left-themeshade: 191; mso-border-top-alt: solid #31849b 3.0pt; mso-border-top-themecolor: accent5; mso-border-top-themeshade: 191; mso-background-themetint: 25; mso-border-bottom-themecolor: accent5; mso-border-bottom-themeshade: 191; mso-border-right-themecolor: accent5; mso-border-right-themeshade: 191;" width="340">
      <p class="MsoNormal" style="mso-margin-top-alt: auto; mso-margin-bottom-alt: auto;">
        <span style="color: black; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 9pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-themecolor: text1; mso-bidi-font-size: 12.0pt;">Enter the password for the User Account<o:p></o:p></span>
      </p>
    </td>
  </tr>
  
  <tr style="height: 24.05pt; mso-yfti-irow: 4;">
    <td style="background: rgb(218, 238, 243); border-width: medium 3pt 3pt; border-style: none solid solid; border-color: currentcolor rgb(49, 132, 155) rgb(49, 132, 155); padding: 0cm 5.4pt; width: 109.2pt; height: 24.05pt; mso-border-themecolor: accent5; mso-border-themeshade: 191; mso-background-themecolor: accent5; mso-border-top-alt: solid #31849b 3.0pt; mso-border-top-themecolor: accent5; mso-border-top-themeshade: 191; mso-background-themetint: 51;" width="146">
      <p class="MsoNormal" style="text-align: center; mso-yfti-cnfc: 68; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto;" align="center">
        <b><span style="color: black; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 9pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-themecolor: text1; mso-bidi-font-size: 12.0pt;">Confirm password<o:p></o:p></span></b>
      </p>
    </td>
    
    <td style="background: rgb(218, 238, 243); border-width: medium 3pt 3pt medium; border-style: none solid solid none; border-color: currentcolor rgb(49, 132, 155) rgb(49, 132, 155) currentcolor; padding: 0cm 5.4pt; width: 9cm; height: 24.05pt; mso-background-themecolor: accent5; mso-border-left-alt: solid #31849b 3.0pt; mso-border-left-themecolor: accent5; mso-border-left-themeshade: 191; mso-border-top-alt: solid #31849b 3.0pt; mso-border-top-themecolor: accent5; mso-border-top-themeshade: 191; mso-background-themetint: 51; mso-border-bottom-themecolor: accent5; mso-border-bottom-themeshade: 191; mso-border-right-themecolor: accent5; mso-border-right-themeshade: 191;" width="340">
      <p class="MsoNormal" style="mso-yfti-cnfc: 64; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto;">
        <span style="color: black; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 9pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-themecolor: text1; mso-bidi-font-size: 12.0pt;">Enter the password for User Account again to confirm.<o:p></o:p></span>
      </p>
    </td>
  </tr>
  
  <tr style="height: 47.4pt; mso-yfti-irow: 5; mso-yfti-lastrow: yes;">
    <td style="background: rgb(237, 246, 249); border-width: medium 3pt 3pt; border-style: none solid solid; border-color: currentcolor rgb(49, 132, 155) rgb(49, 132, 155); padding: 0cm 5.4pt; width: 109.2pt; height: 47.4pt; mso-border-themecolor: accent5; mso-border-themeshade: 191; mso-background-themecolor: accent5; mso-border-top-alt: solid #31849b 3.0pt; mso-border-top-themecolor: accent5; mso-border-top-themeshade: 191; mso-background-themetint: 25;" width="146">
      <p class="MsoNormal" style="text-align: center; mso-yfti-cnfc: 4; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto;" align="center">
        <b><span style="color: black; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 9pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-themecolor: text1; mso-bidi-font-size: 12.0pt;">Private Key Password (Optional)<o:p></o:p></span></b>
      </p>
    </td>
    
    <td style="background: rgb(237, 246, 249); border-width: medium 3pt 3pt medium; border-style: none solid solid none; border-color: currentcolor rgb(49, 132, 155) rgb(49, 132, 155) currentcolor; padding: 0cm 5.4pt; width: 9cm; height: 47.4pt; mso-background-themecolor: accent5; mso-border-left-alt: solid #31849b 3.0pt; mso-border-left-themecolor: accent5; mso-border-left-themeshade: 191; mso-border-top-alt: solid #31849b 3.0pt; mso-border-top-themecolor: accent5; mso-border-top-themeshade: 191; mso-background-themetint: 25; mso-border-bottom-themecolor: accent5; mso-border-bottom-themeshade: 191; mso-border-right-themecolor: accent5; mso-border-right-themeshade: 191;" width="340">
      <blockquote>
        <p class="MsoListParagraphCxSpFirst" style="line-height: normal; text-indent: -18pt; margin-bottom: 0pt; mso-list: l0 level1 lfo9; mso-add-space: auto;">
          <!--[if !supportLists]-->
          
          <font face="Segoe UI"><font size="2"><span style="color: black; font-family: symbol; font-size: 9pt; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol; mso-themecolor: text1; mso-bidi-font-size: 12.0pt;"><span style="mso-list: ignore;">·<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
          
          <b style="mso-bidi-font-weight: normal;"><i style="mso-bidi-font-style: normal;"><span style="color: black; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 9pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-themecolor: text1; mso-bidi-font-size: 12.0pt;">This is optional</span></i></b><span style="color: black; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 9pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-themecolor: text1; mso-bidi-font-size: 12.0pt;">. If the certificates do not have password, leave this empty.<o:p></o:p></span></font></font>
        </p>
        
        <p>
          <font size="2" face="Segoe UI"></font>
        </p>
      </blockquote>
      
      <p>
        <font size="2" face="Segoe UI"></font>
      </p>
      
      <blockquote>
        <p>
          <font size="2" face="Segoe UI"></font>
        </p>
        
        <p class="MsoListParagraphCxSpLast" style="line-height: normal; text-indent: -18pt; margin-bottom: 0pt; mso-list: l0 level1 lfo9; mso-add-space: auto;">
          <!--[if !supportLists]-->
          
          <font face="Segoe UI"><font size="2"><span style="color: black; font-family: symbol; font-size: 9pt; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol; mso-themecolor: text1; mso-bidi-font-size: 12.0pt;"><span style="mso-list: ignore;">·<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
          
          <span style="color: black; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 9pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-themecolor: text1; mso-bidi-font-size: 12.0pt;">If the certificates have one global password, enter that password here.</span></font></font>
        </p>
      </blockquote>
    </td>
  </tr>
</table>

<p class="MsoListParagraphCxSpMiddle" style="margin: 0cm 0cm 6pt 54pt; line-height: 115%; text-indent: -36pt; mso-list: l0 level1 lfo7; mso-add-space: auto;">
  <!--[if !supportLists]-->
  
  <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Segoe UI&quot;;"><span style="mso-list: ignore;"></span></span>
</p>

<p class="MsoListParagraphCxSpMiddle" style="margin: 0cm 0cm 6pt 54pt; line-height: 115%; text-indent: -36pt; mso-list: l0 level1 lfo7; mso-add-space: auto;">
  <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Segoe UI&quot;;"><span style="mso-list: ignore;">6.<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;<font face="Segoe UI">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </font></span></span></span><!--[endif]-->
  
  <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">Centralized SSL Certificate Support feature is now ready to be used. </span>
</p>

<p class="MsoListParagraphCxSpMiddle" style="margin: 0cm 0cm 6pt 54pt; line-height: 115%; text-indent: -36pt; mso-list: l0 level1 lfo7; mso-add-space: auto;">
  <!--[if !supportLists]-->
  
  <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Segoe UI&quot;;"><span style="mso-list: ignore;">7.<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
  
  <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">One manageability feature that is noteworthy is the ability to group the certificates by their expiration dates:</span>
</p>

> <p class="MsoListParagraphCxSpMiddle" style="margin: 0cm 0cm 6pt 54pt; line-height: 115%; text-indent: -36pt; mso-list: l0 level1 lfo7; mso-add-space: auto;">
>   &#160; <a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/7802.image_320A41FA.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/7802.image_5F00_320A41FA.png"><img title="image" style="display: inline; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4341.image_thumb_682BBA49.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/4341.image_5F00_thumb_5F00_682BBA49.png" width="502" height="144" /></a>
> </p>

<p class="MsoListParagraphCxSpLast" style="margin: 0cm 0cm 6pt 54pt; line-height: 115%; text-indent: -36pt; mso-list: l0 level1 lfo7; mso-add-space: auto;">
  <!--[if !supportLists]-->
  
  <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Segoe UI&quot;;"><span style="mso-list: ignore;">8.<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
  
  <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">The webserver is setup to use Centralized Certificate Store.<o:p></o:p></span>
</p>

* * *

   <font size="2"></p> 

<p align="center">
  <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;"><strong><font color="#4f81bd" size="5"><u>How CCS works?</u></font></strong></span>
</p>

<p align="left">
  <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;"><strong><u><font color="#4f81bd" size="5"><font size="2"></font></font><font size="2"></font></u><font size="2"></font></strong><font size="2"></font></span><font size="2" face="Segoe UI">Below steps outline, how the SSL handshake works with a CCS binding on the IIS 8 web server:</font>
</p>

<ol>
  <li>
    <font face="Segoe UI">The client and the server establish a <strong>TCP</strong> connection via <strong>TCP </strong>handshake.</font>
  </li>
  <li>
    <font face="Segoe UI">The client sends a <strong>Client Hello</strong> to the server. This packet contains the specific protocol version, list of supported cipher suites along with the hostname (let’s say <a href="http://www.outlook.com">www.outlook.com</a> provided its a SNI compliant browser). The TCP/IP headers in the packet contain the <strong>IPAddress</strong> and the <strong>Port</strong> number.</font>
  </li>
  <li>
    <font face="Segoe UI">The server checks the registry (legacy bindings) to find a <strong>certificate hash</strong>/<strong>thumbprint</strong> corresponding to the above combination of <strong>IP:Port</strong>.</font>
  </li>
  <li>
    <font face="Segoe UI">If there is no legacy binding for that <strong>IP:Port</strong>, then server uses the port number from the Client Hello to check the registry for a <strong>CCS</strong> binding for this port. The server checks the below key to find the binding information: <strong><font style="background-color: rgb(255, 255, 0);">HKLM\SYSTEM\CurrentControlSet\Services\HTTP\Parameters\SslCcsBindingInfo</font></strong></font>
  </li>
  <li>
    <font face="Segoe UI">If the above step fails i.e., if the server couldn’t find a corresponding CCS binding for that port, then it would fallback to the <strong>legacy binding</strong>. (If this is absent then the SSL handshake would fail).</font>
  </li>
  <li>
    <font face="Segoe UI">If <strong>Step 4</strong> succeeds. The hostname (from Client Hello) is used to generate a filename like <strong><font style="background-color: rgb(255, 255, 0);">hostname.pfx</font></strong>. The filename is passed as a parameter along with the other details (<strong>CCS Configuration</strong>) to the <strong>crypto API’s</strong> which in turn call the <strong>File System API&#8217;s</strong> to retrieve the corresponding certificate from the <strong>Central Certificate Store (File Share)</strong>. The retrieved certificate is cached and the corresponding certificate without private key is added to the <strong>Server Hello</strong> and sent to the client.</font>
  </li>
  <li>
    <font face="Segoe UI">If it cannot find a filename, then it falls back to <strong>Step 5</strong>. </font>
  </li>
</ol>

<p>
  <font size="2"> </p> 
  
  <li>
    <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;"><strong><font color="#4f81bd" size="2"></font></strong></span>
  </li>
  <p>
    </font>
  </p>
  
  <p align="center">
    <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;"><strong><u><font color="#4f81bd" size="5"></font></u></strong></span>
  </p>
  
  <hr />
  
  <p align="center">
    <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;"><strong><font color="#4f81bd" size="5"><u>File Naming Convention</u></font></strong></span>
  </p>
  
  <p>
    <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">Centralized Certificate Store follows a specific naming convention for the certificates. When the client sends a <strong>Client Hello</strong>, IIS uses the <strong>hostname</strong> available from <strong>SNI</strong> to construct a filename (<em><u><font color="#0000ff">hostname.pfx</font></u></em>), and searches the File share to find this file. Once it finds the file it loads it in memory and responds to the client with a Server Hello.</span>
  </p>
  
  <p>
    <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">For IIS to find the exact file match, a naming convention has to be used while storing certificates on the <strong>CCS file share</strong>. As per naming convention the name of the certificate should be: </span>
  </p>
  
  <p align="center">
    <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;"><font style="background-color: rgb(204, 204, 204);" size="3"><strong>Filename Syntax:&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; <subject-name-of-cert.pfx>&#160;&#160; </strong></font></span>
  </p>
  
  <p>
    <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">But how does IIS handle <strong>Wild-Card </strong>& <strong>SAN </strong>Certificates. What is the naming convention for such certificates? Below is the solution:</span>
  </p>
  
  <table class="MsoTableMediumShading2Accent1" style="border: currentcolor; border-collapse: collapse; mso-border-alt: solid windowtext 2.25pt; mso-yfti-tbllook: 1184; mso-padding-alt: 0cm 5.4pt 0cm 5.4pt; mso-border-insideh: 2.25pt solid windowtext; mso-border-insidev: 2.25pt solid windowtext;" cellspacing="0" cellpadding="0" border="1">
    <tr style="height: 36.85pt; mso-yfti-irow: -1; mso-yfti-firstrow: yes;">
      <td style="background: rgb(79, 129, 189); padding: 0cm 5.4pt; border: 2.25pt solid windowtext; width: 32.55pt; height: 36.85pt; mso-background-themecolor: accent1;" width="43">
        <p align="center">
          <b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 14pt; mso-themecolor: background1;">SL <br />NO<o:p></o:p></span></b>
        </p>
      </td>
      
      <td style="background: rgb(79, 129, 189); border-width: 2.25pt 2.25pt 2.25pt medium; border-style: solid solid solid none; border-color: windowtext windowtext windowtext currentcolor; padding: 0cm 5.4pt; width: 427pt; height: 36.85pt; mso-background-themecolor: accent1; mso-border-left-alt: solid windowtext 2.25pt;" width="569">
        <p align="center">
          <b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 16pt; mso-themecolor: background1; mso-bidi-font-size: 12.0pt;">Description</span></b><b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-themecolor: background1;"><o:p></o:p></span></b>
        </p>
      </td>
    </tr>
    
    <tr style="height: 36.85pt; mso-yfti-irow: 0;">
      <td style="background: rgb(79, 129, 189); border-width: medium 2.25pt 2.25pt; border-style: none solid solid; border-color: currentcolor windowtext windowtext; padding: 0cm 5.4pt; width: 32.55pt; height: 36.85pt; mso-background-themecolor: accent1; mso-border-top-alt: solid windowtext 2.25pt;" valign="top" width="43">
        <p align="center">
          <b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 14pt; mso-themecolor: background1;">1<o:p></o:p></span></b>
        </p>
      </td>
      
      <td style="background: rgb(216, 216, 216); border-width: medium 2.25pt 2.25pt medium; border-style: none solid solid none; border-color: currentcolor windowtext windowtext currentcolor; padding: 0cm 5.4pt; width: 427pt; height: 36.85pt; mso-background-themecolor: background1; mso-background-themeshade: 216; mso-border-left-alt: solid windowtext 2.25pt; mso-border-top-alt: solid windowtext 2.25pt;" valign="top" width="569">
        <p class="MsoNormal" style="margin-bottom: 0pt; mso-yfti-cnfc: 64;" align="left">
          <b style="mso-bidi-font-weight: normal;"><span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt;"><u>Certificate with single Subject Name<o:p></o:p></u></span></b>
        </p>
        
        <p class="MsoNormal" style="margin-bottom: 0pt; mso-yfti-cnfc: 64;">
          <span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;"><span style="mso-spacerun: yes;">&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span>If the subject name is "<font color="#0000ff"><u>www.contoso.com</u></font>" then the IIS provider will look for <strong><font style="background-color: rgb(0, 255, 0);">www.contoso.com.pfx</font></strong>).</span>
        </p>
        
        <p class="MsoNormal" style="margin-bottom: 0pt; mso-yfti-cnfc: 64;">
          <span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;"></span>
        </p>
      </td>
    </tr>
    
    <tr style="height: 36.85pt; mso-yfti-irow: 1;">
      <td style="background: rgb(79, 129, 189); border-width: medium 2.25pt 2.25pt; border-style: none solid solid; border-color: currentcolor windowtext windowtext; padding: 0cm 5.4pt; width: 32.55pt; height: 36.85pt; mso-background-themecolor: accent1; mso-border-top-alt: solid windowtext 2.25pt;" valign="top" width="43">
        <p align="center">
          <b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 14pt; mso-themecolor: background1;">2<o:p></o:p></span></b>
        </p>
      </td>
      
      <td style="border-width: medium 2.25pt 2.25pt medium; border-style: none solid solid none; border-color: currentcolor windowtext windowtext currentcolor; padding: 0cm 5.4pt; width: 427pt; height: 36.85pt; mso-border-left-alt: solid windowtext 2.25pt; mso-border-top-alt: solid windowtext 2.25pt;" valign="top" width="569">
        <p class="MsoNormal" style="margin-bottom: 0pt;" align="left">
          <b style="mso-bidi-font-weight: normal;"><span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt;"><u>Wildcard certificate<o:p></o:p></u></span></b>
        </p>
        
        <p class="MsoNormal">
          <span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;"><span style="mso-spacerun: yes;">&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span>The IIS provider uses the underscore character (“_”) as a special character to indicate that it is a wildcard certificate. If the subject name in the SSL certificate is <font color="#0000ff"><u>*.contoso.com</u></font>, then the file name should be "<strong><font style="background-color: rgb(0, 255, 0);">_.contoso.com.pfx</font></strong>".<o:p></o:p></span>
        </p>
        
        <table class="MsoTableColorfulList" style="border-collapse: collapse; mso-yfti-tbllook: 1184; mso-padding-alt: 0cm 5.4pt 0cm 5.4pt;" cellspacing="0" cellpadding="0" border="0">
          <tr style="mso-yfti-irow: -1; mso-yfti-firstrow: yes; mso-yfti-lastrow: yes;">
            <td style="background: rgb(158, 58, 56); border-width: medium medium 1.5pt; border-style: none none solid; border-color: currentcolor currentcolor white; padding: 0cm 5.4pt; width: 385.4pt; mso-background-themecolor: accent2; mso-background-themeshade: 204; mso-border-bottom-themecolor: background1;" valign="top" width="514">
              <p class="MsoNormal" style="margin-bottom: 0pt; mso-yfti-cnfc: 5;">
                <b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-themecolor: background1;">NOTE</span></b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-bidi-font-weight: bold; mso-themecolor: background1;">: IIS provider would first try to search for a SSL certificate with the filename that exactly matches the domain name of the destination site. For example, if the destination site is www.contoso.com, the IIS provider first tries to locate www.consoto.com.pfx.<span style="mso-spacerun: yes;">&#160; </span>If that is unsuccessful, then it tries to locate _.contoso.com <br /></span>
              </p>
            </td>
          </tr>
        </table>
        
        <p class="MsoNormal" style="margin-bottom: 0pt;">
          <span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;"><span style="mso-spacerun: yes;">&#160;</span><o:p></o:p></span>
        </p>
      </td>
    </tr>
    
    <tr style="height: 36.85pt; mso-yfti-irow: 2; mso-yfti-lastrow: yes;">
      <td style="background: rgb(79, 129, 189); border-width: medium 2.25pt 2.25pt; border-style: none solid solid; border-color: currentcolor windowtext windowtext; padding: 0cm 5.4pt; width: 32.55pt; height: 36.85pt; mso-background-themecolor: accent1; mso-border-top-alt: solid windowtext 2.25pt;" valign="top" width="43" align="center">
        <p align="center">
          <b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 14pt; mso-themecolor: background1;">3<o:p></o:p></span></b>
        </p>
      </td>
      
      <td style="background: rgb(216, 216, 216); border-width: medium 2.25pt 2.25pt medium; border-style: none solid solid none; border-color: currentcolor windowtext windowtext currentcolor; padding: 0cm 5.4pt; width: 427pt; height: 36.85pt; mso-background-themecolor: background1; mso-background-themeshade: 216; mso-border-left-alt: solid windowtext 2.25pt; mso-border-top-alt: solid windowtext 2.25pt;" valign="top" width="569">
        <p class="MsoNormal" style="margin-bottom: 0pt; mso-yfti-cnfc: 64;" align="left">
          <b style="mso-bidi-font-weight: normal;"><span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt;"><u>SAN Certificates<o:p></o:p></u></span></b>
        </p>
        
        <p class="MsoNormal" style="margin-bottom: 0pt; mso-yfti-cnfc: 64;">
          <p>
            <span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;"> </p> 
            
            <p class="MsoNormal" style="margin-bottom: 0pt; mso-yfti-cnfc: 64;">
              <span style="mso-spacerun: yes;">&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span>In this case, the certificate must be duplicated with the file names matching Subject names in the certificate. For example, if the certificate is issued for "<font color="#0000ff"><u>www.contoso1.com</u></font>" & <span class="GramE">"<font color="#0000ff"><u>www.contoso2.com</u></font></span>", then the file names should be <strong><font style="background-color: rgb(0, 255, 0);">www.contoso1.com.pfx</font></strong> & <strong><font style="background-color: rgb(0, 255, 0);">www.contoso2.com.pfx</font></strong>, respectively.
            </p>
            
            <p class="MsoNormal" style="margin-bottom: 0pt; mso-yfti-cnfc: 64;">
              So if the SAN Certificate is issued for 3 hostnames then there would be 3 files for those 3 hostnames respectively.
            </p>
            
            <table cellspacing="0" cellpadding="0" width="533" border="0">
              <tr>
                <td valign="top" width="531">
                  <p class="MsoNormal">
                    &#160;
                  </p>
                  
                  <table class="MsoTableColorfulList" style="border-collapse: collapse; mso-yfti-tbllook: 1184; mso-padding-alt: 0cm 5.4pt 0cm 5.4pt;" cellspacing="0" cellpadding="0" border="0">
                    <tr style="mso-yfti-irow: -1; mso-yfti-firstrow: yes; mso-yfti-lastrow: yes;">
                      <td style="background: rgb(158, 58, 56); border-width: medium medium 1.5pt; border-style: none none solid; border-color: currentcolor; padding: 0cm 5.4pt; width: 385.4pt; mso-background-themecolor: accent2; mso-background-themeshade: 204; mso-border-bottom-themecolor: background1;" valign="top" width="531">
                        <p class="MsoNormal" style="margin-bottom: 0pt; mso-yfti-cnfc: 5;">
                          <b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-themecolor: background1;">NOTE</span></b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-bidi-font-weight: bold; mso-themecolor: background1;">: A SAN Certificate is like a global set. It can also be a wild card certificate&#160; <br /></span>
                        </p>
                      </td>
                    </tr>
                  </table>
                </td>
              </tr>
            </table>
            
            <p>
              </span>
            </p>
            
            <p class="MsoNormal" style="margin-bottom: 0pt; mso-yfti-cnfc: 64;">
              &#160;
            </p></td> </tr> </tbody> </table> 
            
            <p class="MsoListParagraphCxSpFirst" style="margin: 0cm 0cm 0pt 42.55pt; line-height: 150%; text-indent: -1cm; mso-list: l3 level1 lfo11; mso-add-space: auto;">
              <!--[if !supportLists]-->
              
              <span style="line-height: 150%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;"><o:p></o:p></span>
            </p>
            
            <p class="MsoListParagraphCxSpFirst" style="margin: 0cm 0cm 0pt 42.55pt; line-height: 150%; text-indent: -1cm; mso-list: l3 level1 lfo11; mso-add-space: auto;">
              <span style="line-height: 150%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;"><o:p>&#160;&#160;&#160;&#160; </o:p></span>
            </p>
            
            <p class="MsoListParagraphCxSpFirst" style="margin: 0cm 0cm 0pt 42.55pt; line-height: 150%; text-indent: -1cm; mso-list: l3 level1 lfo11; mso-add-space: auto;">
              <span style="line-height: 150%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;"><o:p></o:p></span>
            </p>
            
            <hr />
            </font> </p> 
            
            <p align="center">
              <font color="#4f81bd" size="5" face="Segoe UI"><strong><u>Configuring a website to use CCS Bindings</u></strong></font>
            </p>
            
            <p class="MsoListParagraphCxSpFirst" style="margin: 0cm 0cm 0pt 54pt; line-height: normal; text-indent: -36pt; mso-list: l9 level1 lfo13; mso-add-space: auto;">
              <!--[if !supportLists]-->
              
              <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Segoe UI&quot;;"><span style="mso-list: ignore;">1.<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
              
              <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">Open IIS Manager.<o:p></o:p></span>
            </p>
            
            <p class="MsoListParagraphCxSpMiddle" style="margin: 0cm 0cm 0pt 54pt; line-height: normal; text-indent: -36pt; mso-list: l9 level1 lfo13; mso-add-space: auto;">
              <!--[if !supportLists]-->
              
              <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Segoe UI&quot;;"><span style="mso-list: ignore;">2.<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
              
              <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">Under Connections pane, right click "<b style="mso-bidi-font-weight: normal;">Sites</b>" and select "<b style="mso-bidi-font-weight: normal;">Add Website…</b>"<o:p></o:p></span>
            </p>
            
            <p class="MsoListParagraphCxSpMiddle" style="margin: 0cm 0cm 0pt 54pt; line-height: normal; text-indent: -36pt; mso-list: l9 level1 lfo13; mso-add-space: auto;">
              <!--[if !supportLists]-->
              
              <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Segoe UI&quot;;"><span style="mso-list: ignore;">3.<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
              
              <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">Fill the details as shown below<o:p></o:p></span>
            </p>
            
            <p class="MsoListParagraphCxSpMiddle" style="margin: 0cm 0cm 0pt 63.8pt; line-height: normal; text-indent: -1cm; mso-list: l2 level1 lfo18; mso-add-space: auto;">
              <!--[if !supportLists]-->
              
              <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Segoe UI&quot;;"><span style="mso-list: ignore;">a.<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
              
              <b style="mso-bidi-font-weight: normal;"><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">Site name</span></b><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">: CentralSSL0<o:p></o:p></span>
            </p>
            
            <p class="MsoListParagraphCxSpMiddle" style="margin: 0cm 0cm 0pt 63.8pt; line-height: normal; text-indent: -1cm; mso-list: l2 level1 lfo18; mso-add-space: auto;">
              <!--[if !supportLists]-->
              
              <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Segoe UI&quot;;"><span style="mso-list: ignore;">b.<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
              
              <b style="mso-bidi-font-weight: normal;"><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">Physical path</span></b><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">: <u>C:\inetpub\wwwroot\CentralSSL0\</u><o:p></o:p></span>
            </p>
            
            <p class="MsoListParagraphCxSpMiddle" style="margin: 0cm 0cm 0pt 63.8pt; line-height: normal; text-indent: -1cm; mso-list: l2 level1 lfo18; mso-add-space: auto;">
              <!--[if !supportLists]-->
              
              <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Segoe UI&quot;;"><span style="mso-list: ignore;">c.<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
              
              <b style="mso-bidi-font-weight: normal;"><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">Type</span></b><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">: https<o:p></o:p></span>
            </p>
            
            <p class="MsoListParagraphCxSpMiddle" style="margin: 0cm 0cm 0pt 63.8pt; line-height: normal; text-indent: -1cm; mso-list: l2 level1 lfo18; mso-add-space: auto;">
              <!--[if !supportLists]-->
              
              <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Segoe UI&quot;;"><span style="mso-list: ignore;">d.<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
              
              <span class="SpellE"><b style="mso-bidi-font-weight: normal;"><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">Hostname</span></b></span><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">: CentralSSL0</span>
            </p>
            
            <blockquote>
              <p class="MsoListParagraphCxSpMiddle" style="margin: 0cm 0cm 0pt 63.8pt; line-height: normal; text-indent: -1cm; mso-list: l2 level1 lfo18; mso-add-space: auto;">
                <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;"></span><span lang="EN" style="line-height: 115%; font-family: symbol; font-size: 10pt; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol; mso-ansi-language: en;"><span style="mso-list: ignore;">·<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><span lang="EN" style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-ansi-language: en;"><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">In Windows Server 8, host name must be specified when using CCS. (New ) </span></span><span lang="EN" style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-ansi-language: en;"></span><span lang="EN" style="line-height: 115%; font-family: symbol; font-size: 10pt; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol; mso-ansi-language: en;"><span style="mso-list: ignore;"></span></span>
              </p>
              
              <p class="MsoListParagraphCxSpMiddle" style="margin: 0cm 0cm 0pt 63.8pt; line-height: normal; text-indent: -1cm; mso-list: l2 level1 lfo18; mso-add-space: auto;">
                <span lang="EN" style="line-height: 115%; font-family: symbol; font-size: 10pt; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol; mso-ansi-language: en;"><span style="mso-list: ignore;">·<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
                
                <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">The value depends on the certificate being used.<o:p></o:p></span>
              </p>
            </blockquote>
            
            <p class="MsoListParagraphCxSpMiddle" style="margin: 0cm 0cm 0pt 63.8pt; line-height: normal; text-indent: -1cm; mso-list: l2 level1 lfo18; mso-add-space: auto;">
              <!--[if !supportLists]-->
              
              <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Segoe UI&quot;;"><span style="mso-list: ignore;">e.<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
              
              <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">Require Server Name Indication: Selected<o:p></o:p></span>
            </p>
            
            <p class="MsoListParagraphCxSpMiddle" style="margin: 0cm 0cm 0pt 63.8pt; line-height: 115%; text-indent: -1cm; mso-list: l2 level1 lfo18; mso-add-space: auto;">
              <!--[if !supportLists]-->
              
              <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Segoe UI&quot;;"><span style="mso-list: ignore;">f.<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
              
              <span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">Use Centralized Certificate Store: Selected<o:p></o:p></span>
            </p>
            
            <blockquote>
              <p class="MsoListParagraphCxSpMiddle" style="margin: 0cm 0cm 0pt 63.8pt; line-height: 115%; mso-add-space: auto;">
                <b style="mso-bidi-font-weight: normal;"><span style="background: yellow; line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-highlight: yellow;">NOTE</span></b><span style="background: yellow; line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-highlight: yellow;">: There is no need to select a specific certificate.</span><span style="line-height: 115%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;"><o:p></o:p></span>
              </p>
            </blockquote>
            
            <p class="MsoListParagraphCxSpMiddle" style="margin: 0cm 0cm 0pt 63.8pt; line-height: normal; text-indent: -1cm; mso-list: l2 level1 lfo18; mso-add-space: auto;">
              <!--[if !supportLists]-->
              
              <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Segoe UI&quot;;"><span style="mso-list: ignore;">g.<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
              
              <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">With the use of SNI and the naming contract, the corresponding certificate is selected automatically. In this example, IIS tries to read CentralSSL0.pfx from the Centralized SSL Certificates file share.</span>
            </p>
            
            <blockquote>
              <p class="MsoListParagraphCxSpMiddle" style="margin: 0cm 0cm 0pt 63.8pt; line-height: normal; text-indent: -1cm; mso-list: l2 level1 lfo18; mso-add-space: auto;">
                <a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8561.image_543227B3.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/8561.image_5F00_543227B3.png"><img title="image" style="display: inline; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8551.image_thumb_318DE938.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/8551.image_5F00_thumb_5F00_318DE938.png" width="524" height="505" /></a>
              </p>
            </blockquote>
            
            <p class="MsoListParagraphCxSpLast" style="margin: 0cm 0cm 0pt 63.8pt; line-height: normal; text-indent: -1cm; mso-list: l2 level1 lfo18; mso-add-space: auto;">
              <!--[if !supportLists]-->
              
              <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Segoe UI&quot;;"><span style="mso-list: ignore;">h.<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
              
              <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">Click on "<b style="mso-bidi-font-weight: normal;">OK</b>".<o:p></o:p></span>
            </p>
            
            <p class="MsoNormal" style="line-height: normal; margin-bottom: 0pt;">
              <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">You have successfully created a website using Centralized Certificate Store. The management experience is similar to that of Shared Configuration and traditional SSL. There are some differences though:<o:p></o:p></span>
            </p>
            
            <p class="MsoListParagraphCxSpFirst" style="margin: 0cm 0cm 0pt 90pt; line-height: normal; text-indent: -18pt; mso-list: l0 level1 lfo14; mso-add-space: auto;">
              <!--[if !supportLists]-->
              
              <span style="font-family: symbol; font-size: 10pt; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol;"><span style="mso-list: ignore;">·<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
              
              <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">The certificates are stored centrally on a file share.<o:p></o:p></span>
            </p>
            
            <p class="MsoListParagraphCxSpMiddle" style="margin: 0cm 0cm 0pt 90pt; line-height: normal; text-indent: -18pt; mso-list: l0 level1 lfo14; mso-add-space: auto;">
              <!--[if !supportLists]-->
              
              <span style="font-family: symbol; font-size: 10pt; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol;"><span style="mso-list: ignore;">·<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
              
              <span style="background: yellow; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-highlight: yellow;">Host name has to be specified for SSL</span><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;"> site when using CCS.<o:p></o:p></span>
            </p>
            
            <p class="MsoListParagraphCxSpLast" style="margin: 0cm 0cm 0pt 90pt; line-height: normal; text-indent: -18pt; mso-list: l0 level1 lfo14; mso-add-space: auto;">
              <!--[if !supportLists]-->
              
              <span style="font-family: symbol; font-size: 10pt; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol;"><span style="mso-list: ignore;">·<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
              
              <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">SSL binding is not managed explicitly 1-to-1. They are loaded on-demand.<o:p></o:p></span>
            </p>
            
            <p>
              <font size="2" face="Segoe UI"></font>
            </p>
            
            <hr />
            
            <p align="center">
              <font color="#4f81bd" size="5" face="Segoe UI"><strong><u>CCS Bindings</u></strong></font>
            </p>
            
            <p class="MsoNormal">
              <span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">To view the <b style="mso-bidi-font-weight: normal;">CCS bindings</b> we execute the same <span class="SpellE"><strong>netsh</strong></span> command as earlier. Execute the following from an elevated command prompt: <o:p></o:p></span>
            </p>
            
            <p class="MsoNormal" align="center">
              <span class="SpellE"><span class="GramE"><b style="mso-bidi-font-weight: normal;"><span style="background: silver; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-bidi-font-size: 10.0pt; mso-highlight: silver;">netsh</span></b></span></span><b style="mso-bidi-font-weight: normal;"><span style="background: silver; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-bidi-font-size: 10.0pt; mso-highlight: silver;"> http show <span class="SpellE">sslcert</span></span></b>
            </p>
            
            <p class="MsoNormal" align="center">
              <b style="mso-bidi-font-weight: normal;"><span style="background: silver; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-bidi-font-size: 10.0pt; mso-highlight: silver;"><span class="SpellE"></span></span></b><b style="mso-bidi-font-weight: normal;"><span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-bidi-font-size: 10.0pt;"><o:p></o:p></span></b>
            </p>
            
            <table class="MsoTableLightListAccent1" style="border: currentcolor; border-collapse: collapse; mso-border-alt: solid #4f81bd 1.0pt; mso-border-themecolor: accent1; mso-yfti-tbllook: 1184; mso-padding-alt: 0cm 5.4pt 0cm 5.4pt;" cellspacing="0" cellpadding="0" width="462" align="center" border="2">
              <tr style="mso-yfti-irow: -1; mso-yfti-firstrow: yes; mso-yfti-lastrow: yes;">
                <td style="background: rgb(79, 129, 189); padding: 0cm 5.4pt; border: 1pt solid rgb(79, 129, 189); width: 462.1pt; mso-border-themecolor: accent1; mso-background-themecolor: accent1;" width="458">
                  <p class="MsoNormal" style="margin-bottom: 0pt; mso-yfti-cnfc: 5;">
                    <b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-themecolor: background1;"><font color="#ffffff">NOTE</font></span></b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-bidi-font-weight: bold; mso-themecolor: background1;"><font color="#ffffff">:</font> the first line in the output reads "<b>Central Certificate store</b>" and not "<span class="SpellE"><b>IP<span class="GramE">:Port</span></b></span>", as in earlier versions of <b>IIS</b>. The "<b>Certificate Hash</b>" is "</span><b><span style="background: yellow; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-highlight: yellow;">null</span></b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-bidi-font-weight: bold; mso-themecolor: background1;">" too. <o:p></o:p></span>
                  </p>
                  
                  <p class="MsoNormal" style="margin-bottom: 0pt; mso-yfti-cnfc: 5;">
                    <span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-bidi-font-weight: bold; mso-themecolor: background1;">The <b>null</b> indicates that the certificates are loaded on runtime.</span>
                  </p>
                  
                  <p class="MsoNormal" style="margin-bottom: 0pt; mso-yfti-cnfc: 5;">
                    <span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-bidi-font-weight: bold; mso-themecolor: background1;"></span>
                  </p>
                </td>
              </tr>
            </table>
            
            <p class="MsoNormal">
              <span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;"><o:p>&#160;</o:p></span>
            </p>
            
            <p class="MsoNormal">
              <span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">The above command reads the following registry key and enumerates the values. Below is the location:</span>
            </p>
            
            <p class="MsoNormal">
              <span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;"><b style="mso-bidi-font-weight: normal;"><span style="background: yellow; mso-highlight: yellow;">HKLM\SYSTEM\CurrentControlSet\Services\HTTP\Parameters\SslCcsBindingInfo</span></b><o:p></o:p></span>
            </p>
            
            <p>
              <a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3660.image_765A0D6C.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/3660.image_5F00_765A0D6C.png"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8561.image_thumb_3EC44C7E.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/8561.image_5F00_thumb_5F00_3EC44C7E.png" width="609" height="210" /></a>
            </p>
            
            <p>
              <font size="2" face="Segoe UI"></font>
            </p>
            
            <hr />
            
            <p align="center">
              <font color="#4f81bd" size="5" face="Segoe UI"><strong><u>CCS Configuration</u></strong></font>
            </p>
            
            <p>
              <font size="2" face="Segoe UI">In my previous post I had mentioned a new attribute called <strong><font style="background-color: rgb(255, 255, 0);">sslFlags</font></strong>. This attribute specifies whether the SSL binding is using <strong>SNI</strong> or <strong>CCS </strong>or both. CCS Configuration</font>
            </p>
            
            <p>
              &#160;
            </p>
            
            <table class="MsoTableMediumShading2Accent2" style="border: currentcolor; width: 395.75pt; border-collapse: collapse; mso-yfti-tbllook: 1184; mso-padding-alt: 0cm 5.4pt 0cm 5.4pt; mso-border-top-alt: solid windowtext 2.25pt; mso-border-bottom-alt: solid windowtext 2.25pt;" cellspacing="0" cellpadding="0" width="528" align="center" border="1">
              <tr style="height: 31.65pt; mso-yfti-irow: -1; mso-yfti-firstrow: yes;">
                <td style="background: rgb(192, 80, 77); border-width: 2.25pt medium 2.25pt 2.25pt; border-style: solid none solid solid; border-color: windowtext currentcolor windowtext windowtext; padding: 0cm 5.4pt; width: 44.15pt; height: 31.65pt; mso-background-themecolor: accent2;" width="59">
                  <p align="center">
                    <b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-themecolor: background1;">Using <br /></span></b><b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-themecolor: background1;">CCS<o:p></o:p></span></b>
                  </p>
                </td>
                
                <td style="background: rgb(192, 80, 77); border-width: 2.25pt 2.25pt 2.25pt medium; border-style: solid solid solid none; border-color: windowtext windowtext windowtext currentcolor; padding: 0cm 5.4pt; width: 46.5pt; height: 31.65pt; mso-background-themecolor: accent2;" width="62">
                  <p align="center">
                    <b style="mso-bidi-font-weight: normal;"><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-themecolor: background1;">Using <br />S</span></b><b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-themecolor: background1;">NI<o:p></o:p></span></b>
                  </p>
                </td>
                
                <td style="background: rgb(192, 80, 77); border-width: 2.25pt 2.25pt 2.25pt medium; border-style: solid solid solid none; border-color: windowtext windowtext windowtext currentcolor; padding: 0cm 5.4pt; width: 59.9pt; height: 31.65pt; mso-background-themecolor: accent2; mso-border-left-alt: solid windowtext 2.25pt;" width="80">
                  <p align="center">
                    <b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-themecolor: background1;">sslFlags<o:p></o:p></span></b>
                  </p>
                </td>
                
                <td style="background: rgb(192, 80, 77); border-width: 2.25pt 2.25pt 2.25pt medium; border-style: solid solid solid none; border-color: windowtext windowtext windowtext currentcolor; padding: 0cm 5.4pt; width: 245.2pt; height: 31.65pt; mso-background-themecolor: accent2; mso-border-left-alt: solid windowtext 2.25pt;" width="327">
                  <p align="center">
                    <b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-themecolor: background1;">Description<o:p></o:p></span></b>
                  </p>
                </td>
              </tr>
              
              <tr style="height: 25.5pt; mso-yfti-irow: 0;">
                <td style="background: rgb(192, 80, 77); border-width: medium medium medium 2.25pt; border-style: none none none solid; border-color: currentcolor currentcolor currentcolor windowtext; padding: 0cm 5.4pt; width: 44.15pt; height: 25.5pt; mso-background-themecolor: accent2;" width="59">
                  <p class="MsoNormal" style="text-align: center; mso-yfti-cnfc: 68;" align="center">
                    <b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-themecolor: background1;"><o:p></o:p></span></b>
                  </p>
                </td>
                
                <td style="background: rgb(192, 80, 77); border-width: medium 2.25pt medium medium; border-style: none solid none none; border-color: currentcolor windowtext currentcolor currentcolor; padding: 0cm 5.4pt; width: 46.5pt; height: 25.5pt; mso-background-themecolor: accent2;" width="62">
                  <p class="MsoNormal" style="text-align: center; mso-yfti-cnfc: 64;" align="center">
                    <b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-themecolor: background1;"></span></b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-themecolor: background1;"><o:p></o:p></span>
                  </p>
                </td>
                
                <td style="background: rgb(216, 216, 216); border-width: medium 2.25pt medium medium; border-style: none solid none none; border-color: currentcolor windowtext currentcolor currentcolor; padding: 0cm 5.4pt; width: 59.9pt; height: 25.5pt; mso-background-themecolor: background1; mso-background-themeshade: 216; mso-border-left-alt: solid windowtext 2.25pt;" width="80">
                  <p class="MsoNormal" style="text-align: center; mso-yfti-cnfc: 64;" align="center">
                    <b><span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;"></span></b><span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;"><o:p></o:p></span>
                  </p>
                </td>
                
                <td style="background: rgb(216, 216, 216); border-width: medium 2.25pt medium medium; border-style: none solid none none; border-color: currentcolor windowtext currentcolor currentcolor; padding: 0cm 5.4pt; width: 245.2pt; height: 25.5pt; mso-background-themecolor: background1; mso-background-themeshade: 216; mso-border-left-alt: solid windowtext 2.25pt;" width="327">
                  <p class="MsoNormal" style="text-align: center; mso-yfti-cnfc: 64;" align="center">
                    <span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;"></span><span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">Legacy SSL binding. Neither uses SNI nor CCS</span><span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;"><o:p></o:p></span>
                  </p>
                </td>
              </tr>
              
              <tr style="height: 25.5pt; mso-yfti-irow: 1;">
                <td style="background: rgb(192, 80, 77); border-width: medium medium medium 2.25pt; border-style: none none none solid; border-color: currentcolor currentcolor currentcolor windowtext; padding: 0cm 5.4pt; width: 44.15pt; height: 25.5pt; mso-background-themecolor: accent2;" width="59">
                  <p class="MsoNormal" style="text-align: center; mso-yfti-cnfc: 4;" align="center">
                    <b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-themecolor: background1;"><o:p></o:p></span></b>
                  </p>
                </td>
                
                <td style="background: rgb(192, 80, 77); border-width: medium 2.25pt medium medium; border-style: none solid none none; border-color: currentcolor windowtext currentcolor currentcolor; padding: 0cm 5.4pt; width: 46.5pt; height: 25.5pt; mso-background-themecolor: accent2;" width="62">
                  <p class="MsoNormal" style="text-align: center;" align="center">
                    <b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-themecolor: background1;">1</span></b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-themecolor: background1;"><o:p></o:p></span>
                  </p>
                </td>
                
                <td style="border-width: medium 2.25pt medium medium; border-style: none solid none none; border-color: currentcolor windowtext currentcolor currentcolor; padding: 0cm 5.4pt; width: 59.9pt; height: 25.5pt; mso-border-left-alt: solid windowtext 2.25pt;" width="80">
                  <p class="MsoNormal" style="text-align: center;" align="center">
                    <b><span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">1</span></b><span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;"><o:p></o:p></span>
                  </p>
                </td>
                
                <td style="border-width: medium 2.25pt medium medium; border-style: none solid none none; border-color: currentcolor windowtext currentcolor currentcolor; padding: 0cm 5.4pt; width: 245.2pt; height: 25.5pt; mso-border-left-alt: solid windowtext 2.25pt;" width="327">
                  <p class="MsoNormal" style="text-align: center;" align="center">
                    <span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">SSL binding using <strong>SNI</strong>.<o:p></o:p></span>
                  </p>
                </td>
              </tr>
              
              <tr style="height: 25.5pt; mso-yfti-irow: 2;">
                <td style="background: rgb(192, 80, 77); border-width: medium medium medium 2.25pt; border-style: none none none solid; border-color: currentcolor currentcolor currentcolor windowtext; padding: 0cm 5.4pt; width: 44.15pt; height: 25.5pt; mso-background-themecolor: accent2;" width="59">
                  <p class="MsoNormal" style="text-align: center; mso-yfti-cnfc: 68;" align="center">
                    <b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-themecolor: background1;">1<o:p></o:p></span></b>
                  </p>
                </td>
                
                <td style="background: rgb(192, 80, 77); border-width: medium 2.25pt medium medium; border-style: none solid none none; border-color: currentcolor windowtext currentcolor currentcolor; padding: 0cm 5.4pt; width: 46.5pt; height: 25.5pt; mso-background-themecolor: accent2;" width="62">
                  <p class="MsoNormal" style="text-align: center; mso-yfti-cnfc: 64;" align="center">
                    <b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-themecolor: background1;"></span></b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-themecolor: background1;"><o:p></o:p></span>
                  </p>
                </td>
                
                <td style="background: rgb(216, 216, 216); border-width: medium 2.25pt medium medium; border-style: none solid none none; border-color: currentcolor windowtext currentcolor currentcolor; padding: 0cm 5.4pt; width: 59.9pt; height: 25.5pt; mso-background-themecolor: background1; mso-background-themeshade: 216; mso-border-left-alt: solid windowtext 2.25pt;" width="80">
                  <p class="MsoNormal" style="text-align: center; mso-yfti-cnfc: 64;" align="center">
                    <b><span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">2</span></b><span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;"><o:p></o:p></span>
                  </p>
                </td>
                
                <td style="background: rgb(216, 216, 216); border-width: medium 2.25pt medium medium; border-style: none solid none none; border-color: currentcolor windowtext currentcolor currentcolor; padding: 0cm 5.4pt; width: 245.2pt; height: 25.5pt; mso-background-themecolor: background1; mso-background-themeshade: 216; mso-border-left-alt: solid windowtext 2.25pt;" width="327">
                  <p class="MsoNormal" style="text-align: center; mso-yfti-cnfc: 64;" align="center">
                    <span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">SSL binding uses <b style="mso-bidi-font-weight: normal;">CCS</b>, but <b style="mso-bidi-font-weight: normal;">SNI</b> is not enforced.<o:p></o:p></span>
                  </p>
                </td>
              </tr>
              
              <tr style="height: 25.5pt; mso-yfti-irow: 3; mso-yfti-lastrow: yes;">
                <td style="background: rgb(192, 80, 77); border-width: medium medium 2.25pt 2.25pt; border-style: none none solid solid; border-color: currentcolor currentcolor windowtext windowtext; padding: 0cm 5.4pt; width: 44.15pt; height: 25.5pt; mso-background-themecolor: accent2;" width="59">
                  <p class="MsoNormal" style="text-align: center; mso-yfti-cnfc: 4;" align="center">
                    <b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-themecolor: background1;">1<o:p></o:p></span></b>
                  </p>
                </td>
                
                <td style="background: rgb(192, 80, 77); border-width: medium 2.25pt 2.25pt medium; border-style: none solid solid none; border-color: currentcolor windowtext windowtext currentcolor; padding: 0cm 5.4pt; width: 46.5pt; height: 25.5pt; mso-background-themecolor: accent2;" width="62">
                  <p class="MsoNormal" style="text-align: center;" align="center">
                    <b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-themecolor: background1;">1</span></b><span style="color: white; line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-themecolor: background1;"><o:p></o:p></span>
                  </p>
                </td>
                
                <td style="border-width: medium 2.25pt 2.25pt medium; border-style: none solid solid none; border-color: currentcolor windowtext windowtext currentcolor; padding: 0cm 5.4pt; width: 59.9pt; height: 25.5pt; mso-border-left-alt: solid windowtext 2.25pt;" width="80">
                  <p class="MsoNormal" style="text-align: center;" align="center">
                    <b><span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">3</span></b><span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;"><o:p></o:p></span>
                  </p>
                </td>
                
                <td style="border-width: medium 2.25pt 2.25pt medium; border-style: none solid solid none; border-color: currentcolor windowtext windowtext currentcolor; padding: 0cm 5.4pt; width: 245.2pt; height: 25.5pt; mso-border-left-alt: solid windowtext 2.25pt;" width="327">
                  <p class="MsoNormal" style="text-align: center;" align="center">
                    <span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt;">SSL binding uses <b style="mso-bidi-font-weight: normal;">CCS</b>, but <b style="mso-bidi-font-weight: normal;">SNI</b> is enforced.<o:p></o:p></span>
                  </p>
                </td>
              </tr>
            </table>
            
            <p>
              <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Times New Roman&quot;;">If the sslFlags attribute is set to either <strong>2 </strong>or <strong>3</strong>, then it is using the <strong>CCS bindings</strong>. If you check the a</span><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Times New Roman&quot;;"><span class="SpellE">pplicationhost.config</span> this is what the binding section would contain:</span><span style="font-family: &quot;Times New Roman&quot;,&quot;serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;;"><o:p></o:p></span>
            </p>
            
            <p>
              <font size="2" face="Courier New"></font><font size="2" face="Courier New"></font><font size="2" face="Courier New"></font>
            </p>
            
            <table cellspacing="0" cellpadding="2" width="531" align="CENTER" bgcolor="#c0c0c0" border="1">
              <tr>
                <td valign="top" width="529">
                  <p>
                    <font size="2" face="Courier New"><bindings> <br /> < binding protocol="https" bindingInformation="*:443:centralssl0" <font style="background-color: rgb(255, 255, 0);">sslFlags="2"</font> /> <br />< /bindings></font>
                  </p>
                </td>
              </tr>
              
              <tr>
                <td valign="top" width="529">
                  <font size="2" face="Segoe UI"><strong>NOTE</strong>: The IIS manager exposes the above settings via configuration API’s in the IIS UI. It is not recommended to change the registry values directly. You will have to start </font>
                </td>
              </tr>
            </table>
            
            <p>
              <font size="2" face="Segoe UI">However, you wont find the configuration for the CCS Module in applicationhost.config. Well, this information is not stored in any of the config files. It is stored in registry under the following node:</font>
            </p>
            
            <p align="center">
              <b><i><font style="background-color: rgb(255, 255, 0);" size="2" face="Segoe UI">HKLM\SOFTWARE\Microsoft\IIS\CentralCertProvider</font></i></b>
            </p>
            
            <p>
              <a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/5543.image_19C260E0.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/5543.image_5F00_19C260E0.png"><img title="image" style="display: inline; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/1643.image_thumb_3D9B126D.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/1643.image_5F00_thumb_5F00_3D9B126D.png" width="591" height="208" />&#160;</a>
            </p>
            
            <p>
              <font size="2" face="Segoe UI">However, you wont find the configuration for the CCS Module in applicationhost.config. Well, this information is not stored in any of the config files</font>
            </p>
            
            <hr />
            
            <p align="center">
              <font size="5" face="Segoe UI"><strong><u>More Information:</u></strong></font>
            </p>
            
            <blockquote>
              <p class="MsoListParagraphCxSpFirst" style="text-indent: -18pt; mso-list: l0 level1 lfo1;">
                <!--[if !supportLists]-->
                
                <span style="line-height: 105%; font-family: symbol; font-size: 12pt; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol;"><span style="mso-list: ignore;">·<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span><!--[endif]-->
                
                <span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;;"><a href="http://technet.microsoft.com/en-us/video/microsoft-virtual-academy-iis8-centralized-certificate-store.aspx"><font size="2">Microsoft Virtual Academy: IIS8 Centralized Certificate Store</font></a><o:p></o:p></span>
              </p>
            </blockquote>
            
            <blockquote>
              <p class="MsoListParagraphCxSpMiddle" style="text-indent: -18pt; mso-list: l0 level1 lfo1;">
                <!--[if !supportLists]-->
                
                <span class="MsoHyperlink"><span style="color: windowtext; line-height: 105%; font-family: symbol; font-size: 12pt; text-decoration: none; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol; text-underline: none;"><span style="mso-list: ignore;">·<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span></span><!--[endif]-->
                
                <span class="MsoHyperlink"><span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;;"><a href="http://www.iis.net/learn/get-started/whats-new-in-iis-8/iis-80-centralized-ssl-certificate-support-ssl-scalability-and-manageability"><font size="2">IIS 8.0 Centralized SSL Certificate Support: SSL Scalability and Manageability</font></a><o:p></o:p></span></span>
              </p>
            </blockquote>
            
            <blockquote>
              <p class="MsoListParagraphCxSpLast" style="text-indent: -18pt; mso-list: l0 level1 lfo1;">
                <!--[if !supportLists]-->
                
                <span class="MsoHyperlink"><span style="color: windowtext; line-height: 105%; font-family: symbol; font-size: 12pt; text-decoration: none; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol; text-underline: none;"><span style="mso-list: ignore;">·</span></span></span><span class="MsoHyperlink"><span style="color: windowtext; font-family: symbol; text-decoration: none; mso-fareast-font-family: symbol; mso-bidi-font-family: symbol; text-underline: none;"><span style="mso-list: ignore;"><span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></span></span><!--[endif]-->
                
                <span class="MsoHyperlink"><span style="line-height: 105%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;;"><a href="http://technet.microsoft.com/en-us/library/jj129395.aspx"><font size="2">Plan SSL Central Certificate Store</font></a></span></span><span class="MsoHyperlink"><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; mso-fareast-font-family: &quot;Times New Roman&quot;;"> <o:p></o:p></span></span>
              </p>
              
              <p>
                &#160;
              </p>
            </blockquote>
            
            <hr />
            
            <p>
              <font size="2" face="Segoe UI">I’m not done yet. There are few things that I need to address like, if someone has all the 3 types of bindings then which cert would be served? I’m not going to answer it now.</font>
            </p>
            
            <p>
              <font size="2" face="Segoe UI">I will do it in my next blog post. Until then Ciao! <img class="wlEmoticon wlEmoticon-smile" alt="Smile" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8270.wlEmoticon-smile_268C9131.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/8270.wlEmoticon_2D00_smile_5F00_268C9131.png" /></font>
            </p>