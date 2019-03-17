---
id: 343
title: 'Windows Azure Web Sites: PHP, .user.ini and WAWS'
date: 2014-01-01T11:05:56+00:00
author: kaushal
layout: post
guid: https://blogs.msdn.microsoft.com/kaushal/2014/01/01/windows-azure-web-sites-php-user-ini-and-waws/
permalink: /2014/01/01/windows-azure-web-sites-php-user-ini-and-waws/
orig_url:
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2014/01/02/php-user-ini-and-windows-azure-web-sites.aspx
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2014/01/02/php-user-ini-and-windows-azure-web-sites.aspx
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2014/01/02/php-user-ini-and-windows-azure-web-sites.aspx
orig_site_id:
  - "13803"
  - "13803"
  - "13803"
orig_post_id:
  - "10486402"
  - "10486402"
  - "10486402"
orig_parent_id:
  - "10486402"
  - "10486402"
  - "10486402"
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
  - http://blogs.msdn.com/b/kaushal/archive/2014/01/01/windows-azure-web-sites-php-user-ini-and-waws.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2014/01/01/windows-azure-web-sites-php-user-ini-and-waws.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2014/01/01/windows-azure-web-sites-php-user-ini-and-waws.aspx
orig_post_name:
  - php user ini and windows azure web sites
  - php user ini and windows azure web sites
  - php user ini and windows azure web sites
orig_thread_id:
  - "862968"
  - "862968"
  - "862968"
orig_post_author_email:
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
orig_attachment_count:
  - "0"
  - "0"
  - "0"
total_views:
  - "8824"
  - "8824"
  - "8824"
opengraph_tags:
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Windows Azure Web Sites: PHP, .user.ini and WAWS" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2014/01/01/windows-azure-web-sites-php-user-ini-and-waws/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="Happy New Year 2014 to all the readers!! Its been quite some time I wrote a blog post. I am back and today I will be writing a small post on the importance of .user.ini file w.r.t Windows Azure Web Sites (WAWS) As you know WAWS supports PHP framework. As of today it supports the..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4667.wlEmoticon-smile_3A1771D5.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Windows Azure Web Sites: PHP, .user.ini and WAWS" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2014/01/01/windows-azure-web-sites-php-user-ini-and-waws/" />
    <meta name="twitter:description" content="Happy New Year 2014 to all the readers!! Its been quite some time I wrote a blog post. I am back and today I will be writing a small post on the importance of .user.ini file w.r.t Windows Azure Web Sites (WAWS) As you know WAWS supports PHP framework. As of today it supports the..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4667.wlEmoticon-smile_3A1771D5.png" />

  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Windows Azure Web Sites: PHP, .user.ini and WAWS" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2014/01/01/windows-azure-web-sites-php-user-ini-and-waws/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="Happy New Year 2014 to all the readers!! Its been quite some time I wrote a blog post. I am back and today I will be writing a small post on the importance of .user.ini file w.r.t Windows Azure Web Sites (WAWS) As you know WAWS supports PHP framework. As of today it supports the..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4667.wlEmoticon-smile_3A1771D5.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Windows Azure Web Sites: PHP, .user.ini and WAWS" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2014/01/01/windows-azure-web-sites-php-user-ini-and-waws/" />
    <meta name="twitter:description" content="Happy New Year 2014 to all the readers!! Its been quite some time I wrote a blog post. I am back and today I will be writing a small post on the importance of .user.ini file w.r.t Windows Azure Web Sites (WAWS) As you know WAWS supports PHP framework. As of today it supports the..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4667.wlEmoticon-smile_3A1771D5.png" />

  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Windows Azure Web Sites: PHP, .user.ini and WAWS" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2014/01/01/windows-azure-web-sites-php-user-ini-and-waws/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="Happy New Year 2014 to all the readers!! Its been quite some time I wrote a blog post. I am back and today I will be writing a small post on the importance of .user.ini file w.r.t Windows Azure Web Sites (WAWS) As you know WAWS supports PHP framework. As of today it supports the..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4667.wlEmoticon-smile_3A1771D5.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Windows Azure Web Sites: PHP, .user.ini and WAWS" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2014/01/01/windows-azure-web-sites-php-user-ini-and-waws/" />
    <meta name="twitter:description" content="Happy New Year 2014 to all the readers!! Its been quite some time I wrote a blog post. I am back and today I will be writing a small post on the importance of .user.ini file w.r.t Windows Azure Web Sites (WAWS) As you know WAWS supports PHP framework. As of today it supports the..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4667.wlEmoticon-smile_3A1771D5.png" />

categories:
  - Uncategorized
tags:
  - .user.ini
  - PHP
  - php.ini
  - WAWS
  - Windows Azure
  - Windows Azure Web Sites
---
<font size="2">Happy New Year 2014 to all the readers!! <img class="wlEmoticon wlEmoticon-smile" alt="Smile" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4667.wlEmoticon-smile_3A1771D5.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/4667.wlEmoticon_2D00_smile_5F00_3A1771D5.png" /></font>

<font size="2">Its been quite some time I wrote a blog post. I am back and today I will be writing a small post on the importance of <strong>.user.ini</strong> file w.r.t <strong>Windows Azure Web Sites (WAWS)</strong></font>

<font size="2">As you know <strong>WAWS</strong> supports <strong>PHP</strong> framework. As of today it supports the following versions of the framework:</font>

  * <font size="2"><strong>PHP 5.3 (5.3.19)</strong></font>
  * <font size="2"><strong>PHP 5.4 (5.4.9)</strong></font>
  * <font size="2"><strong>PHP 5.5 (5.5.3)</strong></font>

<a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6811.image_09F02712.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/6811.image_5F00_09F02712.png"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block;" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/0878.image_thumb_2C47BC8B.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/0878.image_5F00_thumb_5F00_2C47BC8B.png" width="457" height="63" /></a>

Go to the **CONFIGURE** page under your **WAWS** site to configure this setting. As seen in the above image the user can choose any one of the framework versions which are supported by WAWS.

<table cellspacing="0" cellpadding="2" width="732" align="center" bgcolor="#f0f0f0" border="1">
  <tr>
    <td valign="top" width="730">
      <strong>NOTE:</strong> WAWS supports specific runtime version of a framework version as they have been tested against WAWS. The user can also configure their own customized version of PHP framework which their application supports. This way they will have complete control over the php.ini. Please refer this URL: <font size="2"><a href="http://www.windowsazure.com/en-us/documentation/articles/web-sites-php-configure/#UseCustomPHP" target="_blank" rel="noopener noreferrer">How to: Use a custom PHP runtime</a></font>
    </td>
  </tr>
</table>

<font size="2">You can check the <strong>PHP</strong> runtime configuration by adding a sample php page to your <strong>WAWS</strong> site with the following one line of code:</font>

```php5
<?php
    phpinfo();
?>
```

      <p>
        <font size="2"><strong>PHP</strong> picks up its configuration from the file <strong>php.ini</strong> when it starts up. If you access the above page for your site, you will see that this file resides under: <font face="Courier New"><u><strong>C:\DWASFiles\Sites\<SiteName>\Config\PHP-5.5.3\php.ini</strong></u></font></font>
      </p>

      <p>
        <font size="2">You can read more <strong>PHP.ini</strong> here: </font>
      </p>

      <ul>
        <li>
          <font size="2"><a title="http://www.php.net/manual/en/configuration.file.php" href="http://www.php.net/manual/en/configuration.file.php">http://www.php.net/manual/en/configuration.file.php</a></font>
        </li>
        <li>
          <a title="http://www.php.net/manual/en/ini.list.php" href="http://www.php.net/manual/en/ini.list.php"><font size="2">http://www.php.net/manual/en/ini.list.php</font></a>
        </li>
      </ul>

      <p>
        <font size="2">On premise, the server admins would modify the contents of this file to configure the <strong>PHP</strong> runtime to tailor to the needs of the application. </font>
      </p>

      <p>
        <font size="2">On <strong>WAWS</strong>, with the default runtime versions that are provided the users cannot modify the contents of the <strong>php.ini </strong>file, so there is hardly any room for customization of PHP runtime configuration. However, the users aren’t completely helpless here. There is another configuration file, .user.ini.</font>
      </p>

      <p>
        <font size="2">Support for these files were included in <strong>PHP Version 5.3.0</strong> as they added support for configuration INI files on a per-directory basis. </font><font size="2">You can read more about it here: <a href="http://www.php.net/manual/en/configuration.file.per-user.php" target="_blank" rel="noopener noreferrer">.user.ini files</a>.</font>
      </p>

      <p>
        <font size="2">So we can use the above file to customize/override the PHP runtime settings with the modes <strong><font face="Courier New">PHP_INI_PERDIR</font></strong> and <strong><font face="Courier New">PHP_INI_USER</font></strong>. List of php.ini directives is available here: <a title="http://www.php.net/manual/en/ini.list.php" href="http://www.php.net/manual/en/ini.list.php">http://www.php.net/manual/en/ini.list.php</a></font>
      </p>

      <table cellspacing="0" cellpadding="2" width="573" align="center" bgcolor="#f0f0f0" border="1">
        <tr>
          <td valign="top" width="571">
            <strong>NOTE:</strong> PHP directives with modes set to <strong>PHP_INI_SYSTEM</strong> cannot be overridden.
          </td>
        </tr>
      </table>

      <p>
        <font size="2">So the question remains where do we place this <strong>.user.ini </strong>file? On WAWS the recommended place is to place this file in the root of the website which is <strong>wwwroot</strong> folder. </font>
      </p>

      <ul>
        <li>
          <font size="2">connect to your website via <strong>FTP</strong> using <strong>FileZilla</strong></font>
        </li>
        <li>
          <font size="2">Under <strong>Remote site:</strong> expand ”<strong>/</strong>” and then expand the <strong>site </strong>node.</font>
        </li>
        <li>
          <font size="2">Click on <strong>wwwroot</strong></font>
        </li>
        <li>
          <font size="2">Right click and select “<strong>Create new file</strong>”. enter the name of the file as “<strong>.user.ini</strong>” (remove quotes).</font>
        </li>
        <li>
          <font size="2">Right click the <strong>.user.ini </strong>and select “<strong>View/Edit</strong>” to edit the file in notepad.</font>
        </li>
        <li>
          <font size="2">Override the <strong>PHP</strong> settings here. Save it and then close the file.</font>
        </li>
        <li>
          <font size="2">You will receive a prompt notifying the file content has been changed. </font>
        </li>
        <li>
          <font size="2">Select the check box “<strong>Finish editing and delete local file</strong>” and click on <strong>Yes</strong>.</font>
        </li>
        <li>
          <font size="2">Start and stop the website to force the settings to be read immediately.</font>
        </li>
        <li>
          <font size="2">Browse the <strong>phpinfo</strong> page you created earlier to see the changes yourself.</font>
        </li>
      </ul>

      <p>
        <font size="2">I will write further posts on how to take advantage of the <strong>.user.ini</strong> configuration file. Until then CIAO <img class="wlEmoticon wlEmoticon-smile" alt="Smile" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4667.wlEmoticon-smile_3A1771D5.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/4667.wlEmoticon_2D00_smile_5F00_3A1771D5.png" /></font>
      </p>
