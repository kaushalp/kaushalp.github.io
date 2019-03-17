---
id: 284
title: 'Windows Azure Web Sites: SSL Support and configuration'
date: 2013-06-04T00:11:01+00:00
author: Kaushal Kumar Panday
layout: post
guid: https://blogs.msdn.microsoft.com/kaushal/2013/06/04/windows-azure-web-sites-ssl-support-and-configuration/
permalink: /2013/06/04/windows-azure-web-sites-ssl-support-and-configuration/
orig_url:
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2013/06/04/support-for-ssl-on-windows-azure-web-sites.aspx
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2013/06/04/support-for-ssl-on-windows-azure-web-sites.aspx
orig_site_id:
  - "13803"
  - "13803"
orig_post_id:
  - "10423401"
  - "10423401"
orig_parent_id:
  - "10423401"
  - "10423401"
orig_application_key:
  - kaushal
  - kaushal
orig_post_author_id:
  - "213737"
  - "213737"
orig_post_author_username:
  - djkaushal
  - djkaushal
orig_post_author_created:
  - 2009-07-24 14:00:49.000
  - 2009-07-24 14:00:49.000
orig_is_approved:
  - "1"
  - "1"
orig_url_title:
  - http://blogs.msdn.com/b/kaushal/archive/2013/06/04/windows-azure-web-sites-ssl-support-and-configuration.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2013/06/04/windows-azure-web-sites-ssl-support-and-configuration.aspx
orig_post_name:
  - support for ssl on windows azure web sites
  - support for ssl on windows azure web sites
orig_thread_id:
  - "845254"
  - "845254"
orig_post_author_email:
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
orig_attachment_count:
  - "0"
  - "0"
total_views:
  - "6117"
  - "6117"
opengraph_tags:
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Windows Azure Web Sites: SSL Support and configuration" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2013/06/04/windows-azure-web-sites-ssl-support-and-configuration/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="Finally in the first week of June 2013, it has been announced that Windows Azure Web Sites will provide native support for SSL, which includes both SNI SSL and IP based SSL for custom web site domain names. This feature was one which took some time to be implemented and finally has been introduced. Before..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3157.image_thumb_7A7F294E.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Windows Azure Web Sites: SSL Support and configuration" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2013/06/04/windows-azure-web-sites-ssl-support-and-configuration/" />
    <meta name="twitter:description" content="Finally in the first week of June 2013, it has been announced that Windows Azure Web Sites will provide native support for SSL, which includes both SNI SSL and IP based SSL for custom web site domain names. This feature was one which took some time to be implemented and finally has been introduced. Before..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3157.image_thumb_7A7F294E.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Windows Azure Web Sites: SSL Support and configuration" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2013/06/04/windows-azure-web-sites-ssl-support-and-configuration/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="Finally in the first week of June 2013, it has been announced that Windows Azure Web Sites will provide native support for SSL, which includes both SNI SSL and IP based SSL for custom web site domain names. This feature was one which took some time to be implemented and finally has been introduced. Before..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3157.image_thumb_7A7F294E.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Windows Azure Web Sites: SSL Support and configuration" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2013/06/04/windows-azure-web-sites-ssl-support-and-configuration/" />
    <meta name="twitter:description" content="Finally in the first week of June 2013, it has been announced that Windows Azure Web Sites will provide native support for SSL, which includes both SNI SSL and IP based SSL for custom web site domain names. This feature was one which took some time to be implemented and finally has been introduced. Before..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3157.image_thumb_7A7F294E.png" />
    
categories:
  - Uncategorized
tags:
  - HTTPS
  - IP Based SSL
  - SNI
  - SSL
  - WAWS
  - Windows Azure
  - Windows Azure Web Sites
---
<font size="2">Finally in the first week of June 2013, it has been announced that <strong>Windows Azure Web Sites </strong>will provide native support for <strong>SSL</strong>, which includes both <font color="#05aaf1"><strong>SNI SSL</strong> <font color="#000000">and</font> <strong>IP based SSL</strong></font> for custom web site domain names. This feature was one which took some time to be implemented and finally has been introduced. Before this the only way of doing <strong>SSL</strong> was via <strong><font color="#000000">Cloud Service & Rewriting the URL</font></strong>. Refer this article: </font>[<font size="2">http://www.bradygaster.com/running-ssl-with-windows-azure-web-sites</font>](http://www.bradygaster.com/running-ssl-with-windows-azure-web-sites "http://www.bradygaster.com/running-ssl-with-windows-azure-web-sites")<font size="2">&#160;</font>

<font size="2">The users can view and configure this feature on the <font color="#05aaf1"><strong>CONFIGURE management page</strong></font>. Below is a snapshot of what the users would view:</font>

<font size="2"></font> 

<a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/2541.image_08BB118E.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/2541.image_5F00_08BB118E.png"><font size="2"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3157.image_thumb_7A7F294E.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/3157.image_5F00_thumb_5F00_7A7F294E.png" width="840" height="520" /></font></a>

<font size="2"></font><font size="2"></font> 

<font size="2">The <strong><font color="#05aaf1">certificates </font></strong>and the <strong><font color="#05aaf1">ssl bindings</font></strong> section are the ones which were incorporated into the portal. Before we discuss further we need to understand there are certain pre-requisites which has to be acknowledged.</font>

<font size="2"></font> 

<font size="2"></font> </p> 

  * <font size="2">This feature is not available to sites which are running in either <strong><font color="#ff0000">Free</font></strong> or <strong><font color="#ff0000">Shared</font></strong> mode. (<em>SSL support for <strong>Shared mode</strong> maybe added later, but there is not time frame provided for this</em>.)</font>
<font size="2"></font></ul> 

<font size="2"></font> 

<a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6644.image_4C946747.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/6644.image_5F00_4C946747.png"><font size="2"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3060.image_thumb_67608D53.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/3060.image_5F00_thumb_5F00_67608D53.png" width="843" height="125" /></font></a>

<font size="2"></font> 

<font size="2"></font> </p> 

  * <font size="2"><strong><font color="#05aaf1">ssl bindings</font></strong> section is enabled when the user has a valid custom domain name added for that site. which also implies that in order for the <strong>Choose a certificate</strong> drop down to work the user should configure a custom domain name for the website. </font>

<font size="2"></font>

<font size="2"></font>

<font size="2"></font> 

## <u><font size="5">Adding a SSL Binding to the Windows Azure Web Site</font></u>

<font size="2"></font> 

<font size="2">Once the site has the provided pre-requisites, the user is ready to configure a SSL binding for the site. Lets ensure the web site is scaled to <strong><font color="#05aaf1">RESERVED</font></strong> before we proceed.</font>

<font size="2"></font> 

<a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6507.image_3975CB4C.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/6507.image_5F00_3975CB4C.png"><font size="2"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8512.image_thumb_26C0D195.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/8512.image_5F00_thumb_5F00_26C0D195.png" width="650" height="205" /></font></a>

<font size="2"></font> 

<h2 align="left">
  <u><font size="4"></font></u>
</h2>

<h2 align="left">
  <u><font size="4">Uploading the Certificate</font></u>
</h2>

<font size="2"></font> 

<font size="2"></font> </p> 

  * <font size="2">Go to the Windows azure Portal and select Web Sites.</font>
<font size="2"></font> 

  * <font size="2">Select the site (running in <strong><font color="#05aaf1">RESERVED</font> </strong>mode) for which we need to configure this binding.</font>
<font size="2"></font> 

  * <font size="2">Go to the <strong><font color="#05aaf1">CONFIGURE management page</font></strong>.</font>
<font size="2"></font> 

  * <font size="2">Scroll down to the <strong>certificates </strong>section.</font>
<font size="2"></font> 

  * <font size="2">click on <strong><font color="#008000">upload a certificate</font></strong>. This would pop-up a window as shown below:</font>
<font size="2"></font></ul> 

<font size="2"></font> 

<a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3757.image_2F4430DF.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/3757.image_5F00_2F4430DF.png"><font size="2"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/1641.image_thumb_2C9E05DF.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/1641.image_5F00_thumb_5F00_2C9E05DF.png" width="491" height="360" /></font></a>

<font size="2"></font> 

<font size="2"></font> </p> 

  * <font size="2">Browse to the location of the file and select the file.</font>
<font size="2"></font> 

  * <font size="2">Enter the private key password.</font>
<font size="2"></font> 

  * <font size="2">Click on </font><a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/7532.image_65B77392.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/7532.image_5F00_65B77392.png"><font size="2"><img title="image" style="border: 0px currentcolor; display: inline; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6371.image_thumb_375DEDE5.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/6371.image_5F00_thumb_5F00_375DEDE5.png" width="27" height="27" /></font></a> <font size="2">to upload the certificate. If the upload is successful the portal would reflect the change.</font>
<font size="2"></font></ul> 

<font size="2"></font> 

<a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8867.image_209EA65C.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/8867.image_5F00_209EA65C.png"><font size="2"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8308.image_thumb_3B6ACC68.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/8308.image_5F00_thumb_5F00_3B6ACC68.png" width="832" height="230" /></font></a>

<font size="2"></font> 

<h2 align="left">
  <u><font size="4"></font></u>
</h2>

<h2 align="left">
  <u><font size="4">Adding a custom domain name</font></u>
</h2>

<font size="2"></font> 

<font size="2">Follow the instructions in the following URL to configure a custom domain for your site: </font><a title="Configuring a custom domain name for a Windows Azure web site" href="https://www.windowsazure.com/en-us/develop/net/common-tasks/custom-dns-web-site/" target="_blank" rel="noopener noreferrer"><strong><font size="2">Configuring a custom domain name for a Windows Azure web site</font></strong></a><font size="2">.</font>

<font size="2"></font> 

<font size="2">I added a custom domain on one of my Web Sites for the demo. Here is the snapshot:</font>

<font size="2"></font> 

<a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/5518.image_5F92B7A8.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/5518.image_5F00_5F92B7A8.png"><font size="2"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/2500.image_thumb_3D3DB2E0.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/2500.image_5F00_thumb_5F00_3D3DB2E0.png" width="410" height="216" /></font></a>

<font size="2"></font> <font size="2"></font> 

<h2 align="left">
  <u><font size="4">Adding the SSL Binding</font></u>
</h2>

<font size="2"></font> 

<font size="2">On WAWS, the user can configure the following 2 types of bindings:</font>

<font size="2"></font> 

<font size="2"></font> </p> 

  1. <font size="2">IP based SL binding.</font>
  2. <font size="2">SNI SSL binding.</font>

<font size="2"></font>

### <font style="font-weight: bold;" size="3">SNI SSL Binding</font>

<font size="2"></font> 

<font size="2"></font> </p> 

  * <font size="2">Go to the <strong><font color="#05aaf1">ssl bindings</font></strong> section on the <strong><font color="#05aaf1">CONFIGURE management page</font></strong>. </font>
<font size="2"></font> 

  * <font size="2">Click on the <strong><font color="#05aaf1">Choose a domain name</font></strong> drop down to select one of the domain names configured for the site.</font>
<font size="2"></font></ul> 

<font size="2"></font> 

<a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3513.image_5809D8EC.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/3513.image_5F00_5809D8EC.png"><font size="2"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3060.image_thumb_757EBAA9.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/3060.image_5F00_thumb_5F00_757EBAA9.png" width="831" height="181" /></font></a>

<font size="2"></font> 

<font size="2"></font> </p> 

  * <font size="2">Click on the <strong><font color="#05aaf1">Choose a certificate </font></strong>drop down to select a certificate from the list of certificates uploaded for this site.</font>
<font size="2"></font></ul> 

<font size="2"></font> 

<a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3733.image_59DCBF64.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/3733.image_5F00_59DCBF64.png"><font size="2"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/7462.image_thumb_501757EC.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/7462.image_5F00_thumb_5F00_501757EC.png" width="842" height="173" /></font></a>

<font size="2"></font> 

<font size="2"></font> </p> 

  * <font size="2"><font color="#05aaf1"><strong>SNI SSL</strong></font> is the default option, so no changes has to be done.</font>
<font size="2"></font> 

  * <font size="2">Click <strong>Save</strong> to commit the changes. The user will get a warning notification regarding the impact this may have on billing for the site.</font>
<font size="2"></font></ul> 

<font size="2"></font> 

<a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/5751.image_589AB736.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/5751.image_5F00_589AB736.png"><font size="2"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3644.image_thumb_23FCEBAC.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/3644.image_5F00_thumb_5F00_23FCEBAC.png" width="787" height="214" /></font></a>

<font size="2"></font> 

<font size="2"></font> </p> 

  *  <font size="2">click on <strong><font color="#00ff00"><font style="background-color: rgb(51, 51, 51);">YES</font> </font></strong>to proceed. Upon success the below message will be seen.</font>
<font size="2"></font></ul> 

<font size="2"></font> 

<a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/0535.image_1A378434.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/0535.image_5F00_1A378434.png"><font size="2"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/2548.image_thumb_3503AA40.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/2548.image_5F00_thumb_5F00_3503AA40.png" width="727" height="81" /></font></a>

<font size="2"></font> 

### <font size="3"></font>

### <font size="3">IP based SSL Binding</font>

<font size="2"></font> 

<font size="2"></font> </p> 

  * <font size="2">As specified in the earlier steps, the user has to <strong>upload a certificate</strong> and <strong>configure a domain name</strong> for the website.</font>
<font size="2"></font> 

  * <font size="2">Once done, he could choose it for the corresponding drop downs as we showed earlier.</font>
<font size="2"></font> 

  * <font size="2">Now select <font color="#05aaf1"><strong>IP Based SSL</strong></font> from the third drop down to configure the <strong><font color="#05aaf1">IP based SSL bindings</font></strong> for the site.</font>
<font size="2"></font></ul> 

<font size="2"></font> 

<a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/1004.image_0065DEB6.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/1004.image_5F00_0065DEB6.png"><font size="2"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/5483.image_thumb_36D690B8.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/5483.image_5F00_thumb_5F00_36D690B8.png" width="846" height="188" /></font></a>

<font size="2"></font> 

<font size="2"></font> </p> 

  * <font size="2">Click Save to commit the changes. The user will get a warning that this may impact the billing for the site.</font>
<font size="2"></font></ul> 

<font size="2"></font> 

<a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6406.image_5AFE7BF8.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/6406.image_5F00_5AFE7BF8.png"><font size="2"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3806.image_thumb_6381DB42.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/3806.image_5F00_thumb_5F00_6381DB42.png" width="787" height="214" /></font></a>

<font size="2"></font> 

<font size="2"></font> </p> 

  *  <font size="2">Click on <strong><font color="#00ff00"><font style="background-color: rgb(51, 51, 51);">YES</font> </font></strong>to proceed. Upon success, the below message will be seen.</font>
<font size="2"></font></ul> 

<font size="2"></font> 

<p align="center">
  <a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/5383.image_4773AD08.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/5383.image_5F00_4773AD08.png"><font size="2"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6406.image_thumb_251EA840.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/6406.image_5F00_thumb_5F00_251EA840.png" width="727" height="81" /></font></a>
</p>

  * <h2 align="left">
      <font color="#000000" size="2" face="Segoe UI">Once IP Based SSL binding has been added, the site is assigned a new <font style="font-weight: bold;">IP Address </font>by <font style="font-weight: bold;">WAWS</font>. This IP Address is displayed as Virtual IP Address on the <font style="font-weight: bold;">DASHBOARD </font>page. We need to use this IP address and update the <font style="font-weight: bold;">DNS </font>records to point to the new <font style="font-weight: bold;">VIP</font>. </font><a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/5123.image_6CB88CDB.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/5123.image_5F00_6CB88CDB.png"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/0677.image_thumb_42D818A6.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/0677.image_5F00_thumb_5F00_42D818A6.png" width="825" height="391" /></a>
    </h2>

  * <h2 align="left">
      <font color="#000000" size="2" face="Segoe UI">The above VIP is different from the one seen in the <font style="font-weight: bold;">CONFIGURE </font>management page. The website will be pointing to both the IP addresses. The difference is that when domain name points to the default IP Address it is equivalent to <font style="font-weight: bold;">SNI binding <font style="font-weight: normal;">and when the domain name points to the newly assigned VIP it uses the <font style="font-weight: bold;">IP Based SSL</font>. To notice this difference, access the <font style="font-weight: bold;">URL </font>over <font style="font-weight: bold;">HTTPS </font>from a <font style="font-weight: bold;">XP </font>client running <font style="font-weight: bold;">IE 8</font>.</font></font></font>
    </h2>

  * <h2 align="left">
      <font color="#000000" size="2" face="Segoe UI">The <font style="font-weight: bold;">A </font>record for the domain name needs to be updated to point to the new IP Address. If there was a <font style="font-weight: bold;">CNAME </font>pointing to <sitename>.azurewebsites.net, then it has to be removed.</font>
    </h2>

<p align="center">
  <font color="#ca0207" size="5"><u>*******IMPORTANT*******</u></font>
</p>

<p align="center">
  <font size="2"></font>
</p>

<font size="2"></font><font size="2"></font><font size="2"></font><font size="2"></font><font size="2"></font> 

<table cellspacing="0" cellpadding="2" width="700" align="center" bgcolor="#cccccc" border="1">
  <tr>
    <td valign="top" width="700">
      <font size="2"><strong>NOTE:</strong> <font style="background-color: rgb(255, 255, 0);">If there are multiple bindings for the site then the domain names must be unique</font>. Irrespective of whether they are <strong>IP based SSL bindings</strong> or <strong>SNI SSL bindings</strong>. In simple words, the rules that are applicable while configuring a SSL binding on IIS are still applicable here.&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; <br />&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; <br />Also <strong><font style="background-color: rgb(255, 255, 0);" color="#ff0000">Non-SNI compliant browsers</font></strong> will not be able to browse to the website if it is configured to use <strong><font color="#09a5e8">SNI SSL bindings</font></strong>.</font>
    </td>
  </tr>
</table>

<font size="2"></font> 

## &#160;

## <u><font size="4">Pricing for the SSL Connections for Windows Azure Web Sites</font></u>

<font size="2">The users have to shell out more money when they configure the website to use <strong><font color="#09a5e8">IP Based SSL</font></strong>. This is very obvious, as this requires a <strong>dedicated IP</strong> (a resource) to be allocated for the website. This is also an expensive resource. </font>

<font size="2"><strong><font color="#09a5e8">SNI SSL </font></strong>is comparatively cheaper as it doesn’t need a dedicated IP Address. However, it has own limitations as the <strong><font style="background-color: rgb(255, 255, 0);" color="#ff0000">non-SNI compliant browsers </font></strong>will not be able to access the site.</font>

<font size="2"></font>

<font size="2"></font> 

<a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/1565.image_2DA2078A.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/1565.image_5F00_2DA2078A.png"><font size="2"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8867.image_thumb_51C9F2CA.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/8867.image_5F00_thumb_5F00_51C9F2CA.png" width="846" height="528" /></font></a>

<font size="2"></font>

<a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/2806.image_7C38B498.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/2806.image_5F00_7C38B498.png"><font size="2"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6507.image_thumb_1DBA74D9.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/6507.image_5F00_thumb_5F00_1DBA74D9.png" width="846" height="685" /></font></a>

<font size="4"><font size="3"><strong>Windows Azure Pricing Calculator for Web Sites</strong>:</font> </font>[<font size="2">http://www.windowsazure.com/en-us/pricing/details/web-sites/</font>](http://www.windowsazure.com/en-us/pricing/details/web-sites/ "http://www.windowsazure.com/en-us/pricing/details/web-sites/")<font size="2">&#160;</font>