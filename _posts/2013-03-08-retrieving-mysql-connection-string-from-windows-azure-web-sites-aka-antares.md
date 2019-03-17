---
id: 192
title: Retrieving MySQL connection string from Windows Azure Web Sites aka ANTARES
date: 2013-03-08T03:46:43+00:00
author: kaushal
layout: post
guid: https://blogs.msdn.microsoft.com/kaushal/2013/03/08/retrieving-mysql-connection-string-from-windows-azure-web-sites-aka-antares/
permalink: /2013/03/08/retrieving-mysql-connection-string-from-windows-azure-web-sites-aka-antares/
orig_url:
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2013/03/08/retrieving-mysql-connection-string-from-windows-azure-web-sites-aka-antares.aspx
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2013/03/08/retrieving-mysql-connection-string-from-windows-azure-web-sites-aka-antares.aspx
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2013/03/08/retrieving-mysql-connection-string-from-windows-azure-web-sites-aka-antares.aspx
orig_site_id:
  - "13803"
  - "13803"
  - "13803"
orig_post_id:
  - "10400628"
  - "10400628"
  - "10400628"
orig_parent_id:
  - "10400628"
  - "10400628"
  - "10400628"
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
  - http://blogs.msdn.com/b/kaushal/archive/2013/03/08/retrieving-mysql-connection-string-from-windows-azure-web-sites-aka-antares.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2013/03/08/retrieving-mysql-connection-string-from-windows-azure-web-sites-aka-antares.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2013/03/08/retrieving-mysql-connection-string-from-windows-azure-web-sites-aka-antares.aspx
orig_post_name:
  - retrieving mysql connection string from windows azure web sites aka antares
  - retrieving mysql connection string from windows azure web sites aka antares
  - retrieving mysql connection string from windows azure web sites aka antares
orig_thread_id:
  - "837324"
  - "837324"
  - "837324"
orig_post_author_email:
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
orig_attachment_count:
  - "0"
  - "0"
  - "0"
total_views:
  - "4573"
  - "4573"
  - "4573"
opengraph_tags:
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Retrieving MySQL connection string from Windows Azure Web Sites aka ANTARES" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2013/03/08/retrieving-mysql-connection-string-from-windows-azure-web-sites-aka-antares/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="In my previous post, click here, I mentioned and described few of the features of WAWS, cloud offering from Microsoft. As I mentioned we could associate a application with either the MySQL db or Microsoft’s own SQL Server db. There is a small twist in the story though. MySQL is owned by ClearDB and there..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4010.image_thumb_0C205CE8.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Retrieving MySQL connection string from Windows Azure Web Sites aka ANTARES" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2013/03/08/retrieving-mysql-connection-string-from-windows-azure-web-sites-aka-antares/" />
    <meta name="twitter:description" content="In my previous post, click here, I mentioned and described few of the features of WAWS, cloud offering from Microsoft. As I mentioned we could associate a application with either the MySQL db or Microsoft’s own SQL Server db. There is a small twist in the story though. MySQL is owned by ClearDB and there..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4010.image_thumb_0C205CE8.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Retrieving MySQL connection string from Windows Azure Web Sites aka ANTARES" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2013/03/08/retrieving-mysql-connection-string-from-windows-azure-web-sites-aka-antares/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="In my previous post, click here, I mentioned and described few of the features of WAWS, cloud offering from Microsoft. As I mentioned we could associate a application with either the MySQL db or Microsoft’s own SQL Server db. There is a small twist in the story though. MySQL is owned by ClearDB and there..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4010.image_thumb_0C205CE8.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Retrieving MySQL connection string from Windows Azure Web Sites aka ANTARES" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2013/03/08/retrieving-mysql-connection-string-from-windows-azure-web-sites-aka-antares/" />
    <meta name="twitter:description" content="In my previous post, click here, I mentioned and described few of the features of WAWS, cloud offering from Microsoft. As I mentioned we could associate a application with either the MySQL db or Microsoft’s own SQL Server db. There is a small twist in the story though. MySQL is owned by ClearDB and there..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4010.image_thumb_0C205CE8.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Retrieving MySQL connection string from Windows Azure Web Sites aka ANTARES" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2013/03/08/retrieving-mysql-connection-string-from-windows-azure-web-sites-aka-antares/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="In my previous post, click here, I mentioned and described few of the features of WAWS, cloud offering from Microsoft. As I mentioned we could associate a application with either the MySQL db or Microsoft’s own SQL Server db. There is a small twist in the story though. MySQL is owned by ClearDB and there..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4010.image_thumb_0C205CE8.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Retrieving MySQL connection string from Windows Azure Web Sites aka ANTARES" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2013/03/08/retrieving-mysql-connection-string-from-windows-azure-web-sites-aka-antares/" />
    <meta name="twitter:description" content="In my previous post, click here, I mentioned and described few of the features of WAWS, cloud offering from Microsoft. As I mentioned we could associate a application with either the MySQL db or Microsoft’s own SQL Server db. There is a small twist in the story though. MySQL is owned by ClearDB and there..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4010.image_thumb_0C205CE8.png" />
    
categories:
  - Uncategorized
---
<font size="2" face="Segoe UI">In my previous post, <a href="http://blogs.msdn.com/b/kaushal/archive/2013/03/06/introduction-to-windows-azure-web-sites-aka-antares.aspx" target="_blank" rel="noopener noreferrer">click here</a>, I mentioned and described few of the features of <strong>WAWS</strong>, cloud offering from <strong>Microsoft</strong>. As I mentioned we could associate a application with either the <strong>MySQL</strong> db or <strong>Microsoft</strong>’s own <strong>SQL Server </strong>db. There is a small twist in the story though. <strong>MySQL </strong>is owned by <strong>ClearDB </strong>and there is no UI on <strong>Windows Azure </strong>to manage <strong>MySQL </strong>db.</font>

<font size="2" face="Segoe UI"><strong>Windows Azure </strong>has a web interface/UI for managing <strong>SQL Server </strong>db. Here is a snapshot of the same:</font>

<a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8547.image_26CCF901.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/8547.image_5F00_26CCF901.png"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block;" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4010.image_thumb_0C205CE8.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/4010.image_5F00_thumb_5F00_0C205CE8.png" width="772" height="627" /></a>

<p align="center">
  <font size="2" face="Segoe UI"><u>Windows Azure portal for managing SQL Server databases</u></font>
</p>

<font size="2" face="Segoe UI"></font>

<font size="2" face="Segoe UI">Last week, one of the consumers of the <strong>Windows Azure </strong>wanted to know how to retrieve the <strong>MySQL</strong> connection string so that he could use it with other application that he had on <strong>Azure</strong>. This could get tricky. As I said earlier, there is no UI for managing <strong>MySQL </strong>database. So the question is how does one retrieve the connection string if he wishes to.</font>

<font size="2" face="Segoe UI">Before I proceed ahead on how to retrieve the connection string let me show you how do you create a <strong>MySQL </strong>db on <strong>Windows Azure</strong>.</font>

<font size="2" face="Segoe UI"></font>

<font color="#0080c0" size="5" face="Segoe UI"><strong><u>Creating a MySQL db on Windows Azure Web Sites</u></strong></font>

<font size="2" face="Segoe UI"></font>

  * <font size="2" face="Segoe UI">Go to <strong>WEB SITES</strong> and click on <strong>NEW</strong>.</font>
  * <font size="2" face="Segoe UI">Select <strong>COMPUTE</strong> and then <strong>WEB SITE </strong>and then click on <strong>CUSTOM CREATE</strong>.</font>

<p align="center">
  <a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/7380.image_5344062A.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/7380.image_5F00_5344062A.png"><img title="image" style="display: inline;" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8688.image_thumb_03F70DD6.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/8688.image_5F00_thumb_5F00_03F70DD6.png" width="531" height="232" /></a>
</p>

  * <font size="2" face="Segoe UI">This will show up another portal where you will get the following options </font>
  * <font size="2" face="Segoe UI">Chose the URL for the Web Site.</font>
  * <font size="2" face="Segoe UI">Chose the subscription you want to use, in case you have more than one.</font>
  * <font size="2" face="Segoe UI">The geographical location where you want this to be created.</font>
  * <font size="2" face="Segoe UI">Create either a new <strong>SQL Server</strong> or <strong>MySQL</strong> db or chose from the existing one.</font>

<p align="center">
  <a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3051.image_22614EBF.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/3051.image_5F00_22614EBF.png"><img title="image" style="display: inline;" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4544.image_thumb_6805D8DD.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/4544.image_5F00_thumb_5F00_6805D8DD.png" width="492" height="334" /></a>
</p>

  * <font size="2" face="Segoe UI">Once you have created or selected the database, you will see the <strong>DB CONNECTION STRING NAME</strong>. This can be edited.</font>

<p align="center">
  <a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/5611.image_4D593CC4.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/5611.image_5F00_4D593CC4.png"><img title="image" style="display: inline;" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4137.image_thumb_59E6E9E0.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/4137.image_5F00_thumb_5F00_59E6E9E0.png" width="490" height="331" /></a>
</p>

  * <font size="2" face="Segoe UI">Click on&#160; <a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6201.image_78512AC9.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/6201.image_5F00_78512AC9.png"><img title="image" style="display: inline;" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8741.image_thumb_77E4F7D4.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/8741.image_5F00_thumb_5F00_77E4F7D4.png" width="24" height="23" /></a> to confirm the creation of both the site and the database.</font>

<font size="2" face="Segoe UI">So I created a site (<strong>kaushal-mysql</strong>) to use a <strong>MySQL </strong>database successfully. Now lets proceed to the next step where we can retrieve/view the connection string. </font>

<font size="2" face="Segoe UI"></font>

<font color="#0080c0" size="4" face="Segoe UI"><strong><u>Retrieving/Viewing the MySQL Connection String</u></strong></font>

<font size="2" face="Segoe UI"></font>

<font size="2" face="Segoe UI">In order to be able to the view the connection string the <strong>MySQL </strong>Db should be linked to the site i.e., if you go to the <strong>LINKED RESOURCES </strong>section then you should see that the corresponding <strong>MySQL </strong>db.</font>

  * <font size="2" face="Segoe UI">Click on <strong>WEB SITES</strong>.</font>
  * <font size="2" face="Segoe UI">Click on the site which is using the <strong>MySQL</strong> db. In my case it is <strong>kaushal-mysql</strong>.</font>
  * <font size="2" face="Segoe UI">Click on <strong>DASHBOARD</strong>.</font>
  * <font size="2" face="Segoe UI">Towards the RHS of the portal under <strong>quick glance </strong>you will see the option “<strong>View connection strings.</strong>” Click on this to view the connection string.</font>

<p align="center">
  <a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/1207.image_71078DD9.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/1207.image_5F00_71078DD9.png"><img title="image" style="display: inline; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3757.image_thumb_2EB47596.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/3757.image_5F00_thumb_5F00_2EB47596.png" width="857" height="530" /></a>
</p>



<font size="2" face="Segoe UI">There you go! Here is the <strong>MySQL </strong>connection string that you were looking for. Obviously this will also show the <strong>SQL Server </strong>connection string in case the site was created with a <strong>SQL Server db</strong>.</font>

<font size="2" face="Segoe UI"></font>

<table cellspacing="0" cellpadding="2" width="506" align="center" bgcolor="gray" border="1">
  <tr>
    <td valign="top" width="504">
      <font face="Segoe UI"><font size="2"><strong>NOTE</strong>: If the MySQL database is unlinked then clicking on “<strong>View connection strings</strong>.” will not display anything.</font></font>
    </td>
  </tr>
</table>

<font size="2" face="Segoe UI">&#160; </font> 

<a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/1884.image_45517495.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/1884.image_5F00_45517495.png"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block;" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6266.image_thumb_4B2C182E.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/6266.image_5F00_thumb_5F00_4B2C182E.png" width="475" height="406" /></a>

<font size="2" face="Segoe UI">So ensure that the database is linked to the site in order to view the connection string. Once you have copied the connection string. You could unlink and use that connection string in another application.</font>

<font size="2" face="Segoe UI">That&#8217;s it for today folks. Hope this helps someone. Until then ciao! <img class="wlEmoticon wlEmoticon-smile" alt="Smile" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6663.wlEmoticon-smile_29CC7292.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/6663.wlEmoticon_2D00_smile_5F00_29CC7292.png" /></font>