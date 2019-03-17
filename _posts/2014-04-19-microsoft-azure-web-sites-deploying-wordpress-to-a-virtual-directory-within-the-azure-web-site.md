---
id: 373
title: 'Microsoft Azure Web Sites: Deploying wordpress to a virtual directory within the azure web site'
date: 2014-04-19T03:34:46+00:00
author: Kaushal Kumar Panday
layout: post
guid: https://blogs.msdn.microsoft.com/kaushal/2014/04/19/microsoft-azure-web-sites-deploying-wordpress-to-a-virtual-directory-within-the-azure-web-site/
permalink: /2014/04/19/microsoft-azure-web-sites-deploying-wordpress-to-a-virtual-directory-within-the-azure-web-site/
orig_url:
  - 'http://blogs.msdn.microsoft.com/b/kaushal/archive/2014/04/19/microsoft-azure-web-sites-deploying-wordpress-to-a-virtual-directory-within-the%20-azure-web-site.aspx'
  - 'http://blogs.msdn.microsoft.com/b/kaushal/archive/2014/04/19/microsoft-azure-web-sites-deploying-wordpress-to-a-virtual-directory-within-the%20-azure-web-site.aspx'
orig_site_id:
  - "13803"
  - "13803"
orig_post_id:
  - "10518743"
  - "10518743"
orig_parent_id:
  - "10518743"
  - "10518743"
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
  - http://blogs.msdn.com/b/kaushal/archive/2014/04/19/microsoft-azure-web-sites-deploying-wordpress-to-a-virtual-directory-within-the-azure-web-site.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2014/04/19/microsoft-azure-web-sites-deploying-wordpress-to-a-virtual-directory-within-the-azure-web-site.aspx
orig_post_name:
  - microsoft azure web sites deploying wordpress to a virtual directory within the azure web site
  - microsoft azure web sites deploying wordpress to a virtual directory within the azure web site
orig_thread_id:
  - "870207"
  - "870207"
orig_post_author_email:
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
orig_attachment_count:
  - "0"
  - "0"
total_views:
  - "4817"
  - "4817"
opengraph_tags:
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Microsoft Azure Web Sites: Deploying wordpress to a virtual directory within the azure web site" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2014/04/19/microsoft-azure-web-sites-deploying-wordpress-to-a-virtual-directory-within-the-azure-web-site/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="Microsoft Azure Web Sites allows you to have a virtual directory created within the site. There are many advantages to this. Consider a scenario where you your org&#8217;s site is deployed to root http://&lt;sitename&gt;.azurewebsites.net. You now want to have separate branches for different departments within your org. For example: http://&lt;sitename&gt;.azurewebsites.net/marketing http://&lt;sitename&gt;.azurewebsites.net/sales http://&lt;sitename&gt;.azurewebsites.net/hr Another example could..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/2746.041914_1040_MicrosoftAz1.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Microsoft Azure Web Sites: Deploying wordpress to a virtual directory within the azure web site" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2014/04/19/microsoft-azure-web-sites-deploying-wordpress-to-a-virtual-directory-within-the-azure-web-site/" />
    <meta name="twitter:description" content="Microsoft Azure Web Sites allows you to have a virtual directory created within the site. There are many advantages to this. Consider a scenario where you your org&#8217;s site is deployed to root http://&lt;sitename&gt;.azurewebsites.net. You now want to have separate branches for different departments within your org. For example: http://&lt;sitename&gt;.azurewebsites.net/marketing http://&lt;sitename&gt;.azurewebsites.net/sales http://&lt;sitename&gt;.azurewebsites.net/hr Another example could..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/2746.041914_1040_MicrosoftAz1.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Microsoft Azure Web Sites: Deploying wordpress to a virtual directory within the azure web site" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2014/04/19/microsoft-azure-web-sites-deploying-wordpress-to-a-virtual-directory-within-the-azure-web-site/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="Microsoft Azure Web Sites allows you to have a virtual directory created within the site. There are many advantages to this. Consider a scenario where you your org&#8217;s site is deployed to root http://&lt;sitename&gt;.azurewebsites.net. You now want to have separate branches for different departments within your org. For example: http://&lt;sitename&gt;.azurewebsites.net/marketing http://&lt;sitename&gt;.azurewebsites.net/sales http://&lt;sitename&gt;.azurewebsites.net/hr Another example could..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/2746.041914_1040_MicrosoftAz1.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Microsoft Azure Web Sites: Deploying wordpress to a virtual directory within the azure web site" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2014/04/19/microsoft-azure-web-sites-deploying-wordpress-to-a-virtual-directory-within-the-azure-web-site/" />
    <meta name="twitter:description" content="Microsoft Azure Web Sites allows you to have a virtual directory created within the site. There are many advantages to this. Consider a scenario where you your org&#8217;s site is deployed to root http://&lt;sitename&gt;.azurewebsites.net. You now want to have separate branches for different departments within your org. For example: http://&lt;sitename&gt;.azurewebsites.net/marketing http://&lt;sitename&gt;.azurewebsites.net/sales http://&lt;sitename&gt;.azurewebsites.net/hr Another example could..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/2746.041914_1040_MicrosoftAz1.png" />
    
categories:
  - Uncategorized
tags:
  - Azure
  - Microsoft Azure Web Sites
  - virtual directory
  - webmatrix
  - Windows Azure Web Sites
  - wordpress
---
<span style="font-family:Segoe UI"><strong>Microsoft Azure Web Sites</strong> allows you to have a virtual directory created within the site. There are many advantages to this. Consider a scenario where you your org&#8217;s site is deployed to root <a href="http://<sitename>.azurewebsites.net">http://<sitename>.azurewebsites.net</a>. You now want to have separate branches for different departments within your org. For example:<br /> </span>

<ul style="margin-left: 39pt">
  <li>
    <a href="http://<sitename>.azurewebsites.net/marketing"><span style="font-family:Segoe UI">http://<sitename>.azurewebsites.net/marketing</span></a><span style="font-family:Segoe UI"><br /> </span>
  </li>
  <li>
    <a href="http://<sitename>.azurewebsites.net/sales"><span style="font-family:Segoe UI">http://<sitename>.azurewebsites.net/sales</span></a><span style="font-family:Segoe UI"><br /> </span>
  </li>
  <li>
    <a href="http://<sitename>.azurewebsites.net/hr"><span style="font-family:Segoe UI">http://<sitename>.azurewebsites.net/hr</span></a><span style="font-family:Segoe UI"><br /> </span>
  </li>
</ul>

<span style="font-family:Segoe UI">Another example could be where you would want to setup a blog within your site. In this article I will demonstrate to deploy <strong>wordpress</strong> to virtual directory called <strong>BLOG</strong> within my site.<br /> </span>

<span style="font-family:Segoe UI">Here is my current set-up.<br /> </span>

  * <span style="font-family:Segoe UI"><strong>SiteName</strong>: Kaushal<br /> </span>
  * <span style="font-family:Segoe UI"><strong>HostName</strong>: kaushal.azurewebsites.net<br /> </span>
  * <span style="font-family:Segoe UI"><strong>Application</strong>: ASP.NET MVC<br /> </span>
  * <span style="font-family:Segoe UI"><span style="background-color:yellow">No databases are currently linked to my site</span><br /> </span>

<span style="font-family:Segoe UI">I would host the <strong>wordpress</strong> under my site so that it is accessible under <a href="http://kaushal.azurewebsites.net/blog">http://kaushal.azurewebsites.net/blog</a>. Here is what we need to do.<br /> </span>

  1. <span style="font-family:Segoe UI">Create a virtual directory within my site called <strong>BLOG</strong> via azure portal and link a MySQL database to this site.<br /> </span>
  2. <span style="font-family:Segoe UI">On my Local Machine, download and install WordPress via WebMatrix and deploy it to the virtual directory we created above.<br /> </span>

<span style="font-family:Segoe UI">Sounds easy right? Let&#8217;s go ahead and deploy it.<br /> </span>

# <span style="font-family:Segoe UI; text-decoration:underline">Microsoft Azure Portal<br /> </span>

  * <span style="font-family:Segoe UI">Logon to Azure portal.<br /> </span>
  * <span style="font-family:Segoe UI">Go to the <strong>CONFIGURE</strong> page for the site and scroll to the virtual applications and directories section at the bottom of the page.<br /> </span>
  * <div>
      <span style="font-family:Segoe UI">Add an entry as seen in the below image:<br /> </span>
    </div>
    
<img src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/2746.041914_1040_MicrosoftAz1.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/2746.041914_5F00_1040_5F00_MicrosoftAz1.png" alt="" /> <span style="font-family:Segoe UI"><br /> </span>
    
     

  * <span style="font-family:Segoe UI">Click on <strong>SAVE</strong>.<br /> </span>
  * <span style="font-family:Segoe UI">Now go to the <strong>LINKED RESOURCES</strong> page and link a <strong>MySQL</strong> database to your site.<br /> </span>

<div style="margin-left: 36pt">
  <table style="border-collapse:collapse" border="0">
    <colgroup> <col style="width:623px"/></colgroup> <tr>
      <td style="padding-left: 7px; padding-right: 7px; border-top:  solid #00b0f0 3.0pt; border-left:  solid #00b0f0 3.0pt; border-bottom:  solid #00b0f0 3.0pt; border-right:  solid #00b0f0 3.0pt">
        <p>
          <span style="font-family:Segoe UI; font-size:10pt"><strong>NOTE: </strong>Choose an existing <strong>MySQL DB</strong> or create a new one. Let&#8217;s say you already have a <strong>free</strong><br /> <strong>MySQL DB</strong> associated with your subscription but you want a separate <strong>MySQL</strong> database for the application. You will have to purchase a plan from <strong>CLEARDB </strong>for this</span>
        </p>
      </td>
    </tr>
  </table>
</div>

<p style="margin-left: 36pt">
   
</p>

  * <span style="font-family:Segoe UI">Once, linked. Go to the <strong>DASHBOARD</strong> page.<br /> </span>
  * <span style="font-family:Segoe UI">Under <strong>quick glance</strong> section a hyperlink called <strong>View connection strings</strong> will be created.<br /> </span>

<div style="margin-left: 36pt">
  <table style="border-collapse:collapse" border="0">
    <colgroup> <col style="width:623px"/></colgroup> <tr>
      <td style="padding-left: 7px; padding-right: 7px; border-top:  solid #00b0f0 3.0pt; border-left:  solid #00b0f0 3.0pt; border-bottom:  solid #00b0f0 3.0pt; border-right:  solid #00b0f0 3.0pt">
        <p>
          <span style="font-family:Segoe UI; font-size:10pt"><strong>NOTE: </strong>You could retrieve the connection string parameters from the LINKED RESOURCES page too. Click on MANAGE in the bottom pane for the site. This will redirect you to ClearDB site which will provide you with the following<br /> </span>
        </p>
        
        <ul>
          <li>
            <span style="font-family:Segoe UI; font-size:10pt"><strong>Database<br /> </strong></span>
          </li>
          <li>
            <span style="font-family:Segoe UI; font-size:10pt"><strong>Data Source<br /> </strong></span>
          </li>
          <li>
            <span style="font-family:Segoe UI; font-size:10pt"><strong>User Id<br /> </strong></span>
          </li>
          <li>
            <span style="font-family:Segoe UI; font-size:10pt"><strong>Password</strong></span>
          </li>
        </ul>
      </td>
    </tr>
  </table>
</div>

<p style="margin-left: 36pt">
   
</p>

  * <div>
      <span style="font-family:Segoe UI">Download & save the publishsettings file for the website by clicking the hyperlink &#8220;<strong>Download the publish profile</strong>&#8221; under <strong>quick glance</strong> section of the <strong>DASHBOARD</strong> page.<br /> </span>
    </div>
    
<img src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8637.041914_1040_MicrosoftAz2.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/8637.041914_5F00_1040_5F00_MicrosoftAz2.png" alt="" /> <span style="font-family:Segoe UI"><br /> </span>

# <span style="font-family:Segoe UI; text-decoration:underline">Local Machine<br /> </span>

  * <span style="font-family:Segoe UI">Launch Microsoft WebMatrix<br /> </span>
  * <div>
      <span style="font-family:Segoe UI">Click on <strong>New</strong> -> <strong>App Gallery</strong><br /> </span>
    </div>
    
<img src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6507.041914_1040_MicrosoftAz3.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/6507.041914_5F00_1040_5F00_MicrosoftAz3.png" alt="" /> <span style="font-family:Segoe UI"><br /> </span>

  * <div>
      <span style="font-family:Segoe UI">Select WordPress from the <strong>App Gallery</strong> and click on <strong>Next</strong>.<br /> </span>
    </div>
    
<img src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3718.041914_1040_MicrosoftAz4.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/3718.041914_5F00_1040_5F00_MicrosoftAz4.png" alt="" /> <span style="font-family:Segoe UI"><br /> </span>

  * <span style="font-family:Segoe UI">This will take you to through the WordPress setup.<br /> </span>
  * <div>
      <span style="font-family:Segoe UI">Accept the <strong>EULA</strong> by clicking on &#8220;<strong>I ACCEPT</strong>&#8221;<br /> </span>
    </div>
    
<img src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3821.041914_1040_MicrosoftAz5.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/3821.041914_5F00_1040_5F00_MicrosoftAz5.png" alt="" /> <span style="font-family:Segoe UI"><br /> </span>

  * <div>
      <span style="font-family:Segoe UI">Once done it will start downloading the contents to your local machine (</span><span style="font-family:Consolas"><strong>C:\Users\<username>\Documents\My Web Sites\WordPress</strong></span><span style="font-family:Segoe UI">)<br /> </span>
    </div>
    
<img src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3264.041914_1040_MicrosoftAz6.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/3264.041914_5F00_1040_5F00_MicrosoftAz6.png" alt="" /> <span style="font-family:Segoe UI"><br /> </span>

  * <div>
      <span style="font-family:Segoe UI">During these process it allows you to configure certain application parameters as shown below:<br /> </span>
    </div>
    
<img src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/5430.041914_1040_MicrosoftAz7.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/5430.041914_5F00_1040_5F00_MicrosoftAz7.png" alt="" /> <span style="font-family:Segoe UI"><br /> </span>

  * <div>
      <span style="font-family:Segoe UI">Once you specify the parameters and click on <strong>Next</strong> it proceeds with the installation.<br /> </span>
    </div>
    
<img src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/2605.041914_1040_MicrosoftAz8.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/2605.041914_5F00_1040_5F00_MicrosoftAz8.png" alt="" /> <span style="font-family:Segoe UI"><br /> </span>

  * <span style="font-family:Segoe UI">Once installed, click on &#8220;<strong>Copy user names and passwords</strong>&#8220;. This will copy the details to clipboard which you could save in a text file.<br /> </span>
  * <span style="font-family:Segoe UI">Click on <strong>OK</strong>.<br /> </span>
  *<img src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4377.041914_1040_MicrosoftAz9.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/4377.041914_5F00_1040_5F00_MicrosoftAz9.png" alt="" /> <span style="font-family:Segoe UI"><br /> </span>
  * <div>
      <span style="font-family:Segoe UI">Now click on Publish<br /> </span>
    </div>
    
<img src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6765.041914_1040_MicrosoftAz10.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/6765.041914_5F00_1040_5F00_MicrosoftAz10.png" alt="" /> <span style="font-family:Segoe UI"><br /> </span>

  * <span style="font-family:Segoe UI">This will prompt you with another window.<br /> </span>
  * <div>
      <span style="font-family:Segoe UI">Click on <strong>Import publish profile</strong> and point it to the location where we saved the publishsettings file we downloaded earlier.<br /> </span>
    </div>
    
<img src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4237.041914_1040_MicrosoftAz11.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/4237.041914_5F00_1040_5F00_MicrosoftAz11.png" alt="" /> <span style="font-family:Segoe UI"><br /> </span>

  * <span style="font-family:Segoe UI">Once selected, it will auto-populate the parameters from the publishsettings file.<br /> </span>
  * <div>
      <span style="font-family:Segoe UI">We need to modify the following sections as shown below:<br /> </span>
    </div>
    
      * <span style="font-family:Segoe UI"><strong>Site name</strong>: kaushal\wordpress <span style="font-size:10pt">(<em>physical path location relative to the root site</em>)</span><br /> </span>
      * <span style="font-family:Segoe UI"><strong>Destination URL</strong>: <a href="http://kaushal.azurewebsites.net/blog">http://kaushal.azurewebsites.net/blog</a><br /> <span style="font-size:10pt">(<em>virtual directory name</em>)</span><br /> </span>
    
<img src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/7457.041914_1040_MicrosoftAz12.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/7457.041914_5F00_1040_5F00_MicrosoftAz12.png" alt="" /> <span style="font-family:Segoe UI"><br /> </span>
    
     

<div style="margin-left: 36pt">
  <table style="border-collapse:collapse" border="0">
    <colgroup> <col style="width:623px"/></colgroup> <tr>
      <td style="padding-left: 7px; padding-right: 7px; border-top:  solid #00b0f0 3.0pt; border-left:  solid #00b0f0 3.0pt; border-bottom:  solid #00b0f0 3.0pt; border-right:  solid #00b0f0 3.0pt">
        <p>
          <span style="font-family:Segoe UI; font-size:10pt"><strong>NOTE: </strong>Don&#8217;t chose <span style="color:red"><strong>FTP</strong><br /> </span>as the protocol as it doesn&#8217;t allow you to publish databases.</span>
        </p>
      </td>
    </tr>
  </table>
</div>

<p style="margin-left: 36pt">
   
</p>

  * <span style="font-family:Segoe UI">Click on Validate Connection. Once validated, you will see the confirmation.<br /> </span>
  * <span style="font-family:Segoe UI">Click on <strong>Save.</strong><br /> </span>
  * <span style="font-family:Segoe UI">This will take you to the <strong>Publish Compatibility</strong> page. Click on <strong>Continue</strong>.<br /> </span>
  * <span style="font-family:Segoe UI">Once compatibility check has been performed. Click on <strong>Continue</strong> again.<br /> </span>
  * <div>
      <span style="font-family:Segoe UI">It will display the list of files that will deployed to the server.<br /> </span>
    </div>
    
<img src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/7701.041914_1040_MicrosoftAz13.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/7701.041914_5F00_1040_5F00_MicrosoftAz13.png" alt="" /> <span style="font-family:Segoe UI"><br /> </span>

  * <div>
      <span style="font-family:Segoe UI">Click on <strong>Continue</strong> to start the deployment.<br /> </span>
    </div>
    
<img src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/5241.041914_1040_MicrosoftAz14.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/5241.041914_5F00_1040_5F00_MicrosoftAz14.png" alt="" /> <span style="font-family:Segoe UI"><br /> </span>

  * <span style="font-family:Segoe UI">Once publishing is completed you could open the log file and analyze.<br /> </span>
  * <div>
      <span style="font-family:Segoe UI">Click on the hyperlink as shown below to browse to the site:<br /> </span>
    </div>
    
<img src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3681.041914_1040_MicrosoftAz15.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/3681.041914_5F00_1040_5F00_MicrosoftAz15.png" alt="" /> <span style="font-family:Segoe UI"><br /> </span>
    
<img src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/5277.041914_1040_MicrosoftAz16.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/5277.041914_5F00_1040_5F00_MicrosoftAz16.png" alt="" /> <span style="font-family:Segoe UI"><br /> </span>

<span style="font-family:Segoe UI">HTH,<br /> </span>

<span style="font-family:Segoe UI">Kaushal<br /> </span>

<p style="margin-left: 36pt">
   
</p>

<span style="font-family:Segoe UI"><br /> </span> 