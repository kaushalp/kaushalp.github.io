---
id: 233
title: Difference in IIS 6, IIS 7.x and IIS 8 with regards to SSL
date: 2013-05-26T18:40:45+00:00
author: Kaushal Kumar Panday
layout: post
guid: https://blogs.msdn.microsoft.com/kaushal/2013/05/26/difference-in-iis-6-iis-7-x-and-iis-8-with-regards-to-ssl/
permalink: /2013/05/26/difference-in-iis-6-iis-7-x-and-iis-8-with-regards-to-ssl/
orig_url:
  - 'http://blogs.msdn.microsoft.com/b/kaushal/archive/2013/05/27/difference-in-iis-6%20-iis-7-x-and-iis-8-with-regards-to-ssl.aspx'
  - 'http://blogs.msdn.microsoft.com/b/kaushal/archive/2013/05/27/difference-in-iis-6%20-iis-7-x-and-iis-8-with-regards-to-ssl.aspx'
  - 'http://blogs.msdn.microsoft.com/b/kaushal/archive/2013/05/27/difference-in-iis-6%20-iis-7-x-and-iis-8-with-regards-to-ssl.aspx'
orig_site_id:
  - "13803"
  - "13803"
  - "13803"
orig_post_id:
  - "10421460"
  - "10421460"
  - "10421460"
orig_parent_id:
  - "10421460"
  - "10421460"
  - "10421460"
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
  - http://blogs.msdn.com/b/kaushal/archive/2013/05/26/difference-in-iis-6-iis-7-x-and-iis-8-with-regards-to-ssl.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2013/05/26/difference-in-iis-6-iis-7-x-and-iis-8-with-regards-to-ssl.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2013/05/26/difference-in-iis-6-iis-7-x-and-iis-8-with-regards-to-ssl.aspx
orig_post_name:
  - difference in iis 6 iis 7 x and iis 8 with regards to ssl
  - difference in iis 6 iis 7 x and iis 8 with regards to ssl
  - difference in iis 6 iis 7 x and iis 8 with regards to ssl
orig_thread_id:
  - "844621"
  - "844621"
  - "844621"
orig_post_author_email:
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
orig_attachment_count:
  - "0"
  - "0"
  - "0"
total_views:
  - "30705"
  - "30705"
  - "30705"
opengraph_tags:
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Difference in IIS 6, IIS 7.x and IIS 8 with regards to SSL" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2013/05/26/difference-in-iis-6-iis-7-x-and-iis-8-with-regards-to-ssl/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="There were lot of differences with regards to SSL moving from IIS 6 to IIS 7.x and then to IIS 8. IIS 6 in itself was a breaking change, however there were lot of limitations and they were addressed in higher versions. I will try to pen down as I remember them and will update..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/7318.image_thumb_355CF221.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Difference in IIS 6, IIS 7.x and IIS 8 with regards to SSL" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2013/05/26/difference-in-iis-6-iis-7-x-and-iis-8-with-regards-to-ssl/" />
    <meta name="twitter:description" content="There were lot of differences with regards to SSL moving from IIS 6 to IIS 7.x and then to IIS 8. IIS 6 in itself was a breaking change, however there were lot of limitations and they were addressed in higher versions. I will try to pen down as I remember them and will update..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/7318.image_thumb_355CF221.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Difference in IIS 6, IIS 7.x and IIS 8 with regards to SSL" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2013/05/26/difference-in-iis-6-iis-7-x-and-iis-8-with-regards-to-ssl/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="There were lot of differences with regards to SSL moving from IIS 6 to IIS 7.x and then to IIS 8. IIS 6 in itself was a breaking change, however there were lot of limitations and they were addressed in higher versions. I will try to pen down as I remember them and will update..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/7318.image_thumb_355CF221.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Difference in IIS 6, IIS 7.x and IIS 8 with regards to SSL" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2013/05/26/difference-in-iis-6-iis-7-x-and-iis-8-with-regards-to-ssl/" />
    <meta name="twitter:description" content="There were lot of differences with regards to SSL moving from IIS 6 to IIS 7.x and then to IIS 8. IIS 6 in itself was a breaking change, however there were lot of limitations and they were addressed in higher versions. I will try to pen down as I remember them and will update..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/7318.image_thumb_355CF221.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Difference in IIS 6, IIS 7.x and IIS 8 with regards to SSL" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2013/05/26/difference-in-iis-6-iis-7-x-and-iis-8-with-regards-to-ssl/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="There were lot of differences with regards to SSL moving from IIS 6 to IIS 7.x and then to IIS 8. IIS 6 in itself was a breaking change, however there were lot of limitations and they were addressed in higher versions. I will try to pen down as I remember them and will update..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/7318.image_thumb_355CF221.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Difference in IIS 6, IIS 7.x and IIS 8 with regards to SSL" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2013/05/26/difference-in-iis-6-iis-7-x-and-iis-8-with-regards-to-ssl/" />
    <meta name="twitter:description" content="There were lot of differences with regards to SSL moving from IIS 6 to IIS 7.x and then to IIS 8. IIS 6 in itself was a breaking change, however there were lot of limitations and they were addressed in higher versions. I will try to pen down as I remember them and will update..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/7318.image_thumb_355CF221.png" />
    
categories:
  - Uncategorized
tags:
  - architecture
  - IIS 6
  - IIS 7
  - IIS 8
  - kernel mode
  - ksecdd.sys
  - Schannel
  - Schannel.dll
  - SSL
  - user mode
  - Windows Server 2012
---
<font size="2">There were lot of differences with regards to <strong>SSL</strong> moving from <strong>IIS 6</strong> to <strong>IIS 7.x </strong>and then to <strong>IIS 8</strong>. IIS 6 in itself was a breaking change, however there were lot of limitations and they were addressed in higher versions. I will try to pen down as I remember them and will update the blog if I come across other changes.</font>

<font size="2">Before I proceed further, for readers who are not familiar with <strong>IIS</strong> and <strong>Windows </strong>versions, this is a small info to set the stage:</font>

  * <font size="2"><strong>IIS 6 (Windows Server 2003 and Windows XP 64 bit only)</strong></font>
  * <font size="2"><strong>IIS 7 (Windows Server 2008 and Windows Vista)</strong></font>
  * <font size="2"><strong>IIS 7.5 (Windows Server 2008 R2 and Windows 7)</strong></font>
  * <font size="2"><strong>IIS 8 (Windows Server 2012 and Windows 8)</strong></font>

<font size="2">I will be addressing both <strong>IIS 7</strong> and <strong>IIS 7.5</strong> as <strong>IIS 7.x</strong>.</font>

# <font color="#0080ff" size="5" face="Segoe UI"><u><font style="font-weight: bold;">Differences from architectural perspective:</font></u></font>

<font size="2">One major difference between <strong>IIS 6</strong> and the <strong>IIS 7.x</strong> was the way they would handle incoming <strong>HTTPS</strong> requests. Lets discuss how HTTPS requests were handled in IIS 6 before we proceed any further. </font>

<a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/0675.image_6BC6B3B7.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/0675.image_5F00_6BC6B3B7.png"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/7318.image_thumb_355CF221.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/7318.image_5F00_thumb_5F00_355CF221.png" width="823" height="465" /></a>

<font size="2">Taking the above architecture into consideration this is how the IIS 6 request flow looks like:</font>

  1. <font size="2">HTTPS requests comes into <strong>SSL Queue </strong>within <strong>HTTP.SYS</strong>, which is in the <strong>KERNEL Mode</strong>.</font>
  2. <font size="2">The encrypted requests is then sent to a <strong>USER Mode </strong>process called <strong>LSASS.exe</strong> for decryption. The request is decrypted using <strong>SChannel.dll</strong> loaded inside the<strong> lsass.exe</strong> process.</font>
  3. <font size="2">The decrypted request is not sent back to the <strong>HTTP.SYS </strong>In the <strong>Kernel Mode</strong>.</font>
  4. <font size="2">This is now placed in the corresponding <strong>Application Pool queue</strong> and then routed to corresponding worker process in <strong>USER Mode</strong> based upon which <strong>w3wp.exe</strong> a application pool queue corresponds too.</font>
  5. <font size="2">The w3wp.exe generates the response and sends it back to the <strong>HTTP.SYS </strong>in the <strong>KERNEL Mode</strong>.</font>
  6. <font size="2">This response is again sent to the Lsass.exe process in the user mode for encryption.</font>
  7. <font size="2">After encryption, lsass.exe sends it back to the <strong>HTTP.SYS </strong>in the <strong>KERNEL mode</strong>.</font>
  8. <font size="2">The encrypted response is sent back to the client. <br /></font>

<h3 align="center">
  <u><font size="3"><font style="font-weight: bold;" face="Segoe UI">PROBLEM 1:</font></font></u>
</h3>

<font size="2">During the course of the entire processing of request, there were several context switches (<em>Whenever there is a flow of control from <strong>KERNEL MODE </strong>to <strong>USER MODE </strong>or vice versa, it is referred as a <strong>CONTEXT SWITCH</strong></em>). </font>

<font size="2">There were <font style="background-color: rgb(255, 255, 0);" color="#ff0000"><strong>6 context switches in the above flow</strong></font>, out of which <strong><font style="background-color: rgb(255, 255, 0);" color="#ff0000">4 context switches happened for encrypting and decrypting of request and response</font></strong>.</font>

<font size="2">Context switching induces additional overhead and delays the processing of requests. This impacts the performance as this happens for every HTTPS request-response cycle.</font>

<font size="2">These 4 context switches could have been avoided if the encryption and decryption happened in the <strong>KERNEL Mode</strong>. This was addressed in <strong>IIS 7</strong> and the same was retained in later versions.</font>

<h4 align="center">
  <font size="3" face="Segoe UI"><u><font style="font-weight: bold;">PROBLEM 2:</font></u></font>
</h4>

<font size="2">Another problem is the problem with host headers. <strong>Host Headers</strong> were never defined in the original <strong>SSL Specification</strong>, as they were part of the <strong>HTTP RFC</strong> and defined there. The <strong>TCP Layer</strong> never defined the Host headers for obvious reasons. <font style="background-color: rgb(255, 255, 0);" color="#ff0000"><strong>Due to this, a major problem emerged & made SSL applications not scalable</strong></font>.</font>

<font size="2">Due to the unavailability of the Host Header in the <strong>TCP</strong> layer, the incoming encrypted <strong>HTTPS</strong> request provided only <strong>IP+Port</strong> as information to <strong>HTTP.SYS</strong>. In IIS the problem was addressed by allowing only one <strong>SERVER CERTIFICATE</strong> (<strong>Certificate Hash</strong>) per <strong>IP+PORT </strong>binding. The <strong>SSL Host Header</strong> was mostly irrelevant unless the <strong>Server Certificate </strong>was either a <strong>Wild Card Certificate </strong>or a <strong>SAN Certificate</strong>.</font>

<font size="2">This problem was later addressed by the <strong>IEEE </strong>by introducing <strong>Subject Name Indication </strong>(<strong>SNI</strong>). Here the host header was made available in the <strong>Client Hello</strong>,<strong> </strong>sent by the client to the serer during the initiation of the <strong>SSL Handshake</strong>.</font>

<font size="2">This was implemented in <strong>IIS 8</strong>. However, it has its own set of limitations.</font>

<h3 align="center">
  <font face="Segoe UI"><font style="font-weight: bold;" size="4"><u>SOLUTION:</u></font></font>
</h3>

<p align="left">
  <font size="2">In<strong> IIS 6</strong>, the solution was already present in the form of <a href="http://msdn.microsoft.com/en-us/library/windows/desktop/aa364671%28v=vs.85%29.aspx" target="_blank" rel="noopener noreferrer"><strong>KERNEL MODE SSL</strong></a>. However this required tweaking of a registry key and was not a ideal solution as it wasn’t used by most of the customers and was never recommended.</font>
</p>

<table cellspacing="0" cellpadding="2" width="678" align="center" bgcolor="#cccccc" border="2">
  <tr>
    <td valign="top" width="674">
      <ul>
        <li>
          Go to the run prompt and type<strong> Regedit</strong> and click <b>OK</b>.
        </li>
        <li>
          Navigate to and double-click the following key in the registry:
        </li>
        <ul>
          <li>
            <strong><font style="background-color: rgb(255, 255, 0);">HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\HTTP\Parameters</font></strong>
          </li>
        </ul>
        
        <li>
          Add the following <b>DWORD </b>registry key:
        </li>
        <ul>
          <li>
            Name: <b>EnableKernelSSL</b>
          </li>
          <li>
            Type: <b>REG_DWORD</b>
          </li>
        </ul>
        
        <li>
          Data: Set this to <strong>1</strong> to use <strong>kernel-mode SSL;</strong> <strong></strong> is for <strong>user-mode SSL</strong>.
        </li>
      </ul>
    </td>
  </tr>
</table>

* * *

<font size="2">In <strong>IIS 7</strong>, <strong>KERNEL MODE SSL</strong> is the default option and this cannot be changed. The <strong>KSECDD.SYS</strong> driver is responsible for providing the cryptographic functionalities in the kernel mode.</font>

<font size="2">This <strong><font style="background-color: rgb(0, 255, 0);" color="#333333">reduces the context switching</font></strong> during the request response cycle and hence improves the overall performance. Below is the improved request-response flow:</font>

<!--StartFragment-->

<font size="2"></font> </p> 

  1. <font size="2">HTTPS requests comes into <strong>SSL Queue </strong>within <strong>HTTP.SYS</strong>, which is in the <strong>KERNEL Mode</strong>.</font>
<font size="2"></font> 

  2. <font size="2">The encrypted request is decrypted with the help of <strong>KERNEL Mode SSL</strong>.</font>
<font size="2"></font> 

  3. <font size="2">This decrypted request is placed in the corresponding <strong>Application Pool queue</strong> and then routed to corresponding worker process in <strong>USER Mode</strong> based upon which <strong>w3wp.exe</strong> a application pool queue corresponds too.</font>
<font size="2"></font> 

  4. <font size="2">The w3wp.exe generates the response and sends it back to the <strong>HTTP.SYS </strong>in the <strong>KERNEL Mode</strong>.</font>
<font size="2"></font> 

  5. <font size="2">This response is encrypted via the <strong>KERNEL Mode SSL</strong> component.</font>
<font size="2"></font> 

  6. <font size="2">The encrypted response is sent back to the client.</font>
<!--EndFragment--></ol> 

<font size="2">As seen there is a clear performance improvement due to the reduced context switching.</font>

* * *

<font size="2">In IIS 8, this problem 1 was already addressed as it was inheriting the architecture of IIS 7. However, considerable changes were made to the HTTP.SYS and the SSL functionality to incorporate SNI in the server architecture.</font>

<font size="2">A new form of <strong>SSL binding </strong>called <strong>SNI bindings </strong>was introduced, which were in the form of <strong>HostName+Port</strong>.</font>

<font size="2">You can read more about it here:</font>

  * [<font size="2">http://blogs.msdn.com/b/kaushal/archive/2012/08/08/ssl-scalability-with-iis-8-windows-8-server.aspx</font>](http://blogs.msdn.com/b/kaushal/archive/2012/08/08/ssl-scalability-with-iis-8-windows-8-server.aspx "http://blogs.msdn.com/b/kaushal/archive/2012/08/08/ssl-scalability-with-iis-8-windows-8-server.aspx")
  * [<font size="2">http://blogs.msdn.com/b/kaushal/archive/2012/09/04/server-name-indication-sni-in-iis-8-windows-server-2012.aspx</font>](http://blogs.msdn.com/b/kaushal/archive/2012/09/04/server-name-indication-sni-in-iis-8-windows-server-2012.aspx "http://blogs.msdn.com/b/kaushal/archive/2012/09/04/server-name-indication-sni-in-iis-8-windows-server-2012.aspx")
  * [<font size="2">http://blogs.msdn.com/b/kaushal/archive/2012/10/11/central-certificate-store-ccs-with-iis-8-windows-server-2012.aspx</font>](http://blogs.msdn.com/b/kaushal/archive/2012/10/11/central-certificate-store-ccs-with-iis-8-windows-server-2012.aspx "http://blogs.msdn.com/b/kaushal/archive/2012/10/11/central-certificate-store-ccs-with-iis-8-windows-server-2012.aspx") 

<h1 align="center">
  <font size="5" face="Segoe UI"><font style="font-weight: bold;" color="#0080ff"><u>Differences from Configuration Perspective:</u></font></font>
</h1>

<font size="2">In IIS 6, this is how the bindings section looked like within the MetaBase.xml:</font>

<table cellspacing="0" cellpadding="2" width="688" align="center" border="2">
  <tr>
    <td valign="top" width="684">
      <div class="csharpcode">
        <pre class="alt">&lt;IIsWebServer Location=<span class="str">"/LM/W3SVC/1"</span> AppPoolId=<span class="str">"DefaultAppPool"</span></pre>
        
        <pre>...</pre>
        
        <pre class="alt">...</pre>
        
        <pre>...</pre>
        
        <p>
          <strong><font style="background-color: rgb(255, 255, 0);"></font></strong>
        </p>
        
        <pre class="alt"><strong><font style="background-color: rgb(255, 255, 0);">SSLCertHash=<span class="str">"1c25a46a479813472f8d997b3ef4b699130b0737"</span> SSLStoreName=<span class="str">"MY"</span> </font></strong></pre>
        
        <p>
          <strong><font style="background-color: rgb(255, 255, 0);"></font></strong>
        </p>
        
        <pre><strong><font style="background-color: rgb(255, 255, 0);">SecureBindings=<span class="str">":443:"</span></font></strong> </pre>
        
        <pre class="alt">ServerAutoStart=<span class="str">"TRUE"</span> </pre>
        
        <pre>ServerBindings=<span class="str">":80: :80:www.kaushal.com :80:www.kaushal.edu :80:kaushal"</span> </pre>
        
        <pre class="alt">ServerComment=<span class="str">"Default Web Site"</span> ServerSize=<span class="str">"1"</span> </pre>
        
        <pre><strong><font style="background-color: rgb(255, 255, 0);">SslCtlIdentifier=<span class="str">"{6A615835-58F1-4B6F-A779-3F5AE1F1F9E7}"</span> </font></strong></pre>
        
        <pre class="alt"><strong>SslCtlStoreName=<span class="str">"CA"</span></strong> UseHostName=<span class="str">"TRUE"</span>&gt;</pre></p>
      </div>
    </td>
  </tr>
</table>

<font size="2">As seen in the above snippet of the config section, the SSL cert hash was stored within the MetaBase.xml along with the bindings information and SSL related information like SSLStoreName, SSLCtlStoreName etc.</font>

<font size="2">This information was also present in the registry as well. There was supplication of efforts one could say because the user mode processes would refer the MetaBase.xml while kernel mode components would refer the registry related information.</font>

* * *

<font size="2">This changed in IIS 7.x and later versions have incorporated it, all the certificate related information was moved to the registry, no cert related information is stored in the config file. Below is a snippet of the config:</font>

<table cellspacing="0" cellpadding="0" width="793" align="center" bgcolor="#cccccc" border="2">
  <tr>
    <td valign="top" width="789">
      <div class="csharpcode">
        <pre class="alt">&lt;sites&gt;</pre>
        
        <pre>    &lt;site name=<span class="str">"Default Web Site"</span> id=<span class="str">"1"</span> serverAutoStart=<span class="str">"true"</span>&gt;</pre>
        
        <pre class="alt">        &lt;application path=<span class="str">"/"</span>&gt;</pre>
        
        <pre>            &lt;virtualDirectory path=<span class="str">"/"</span> physicalPath=<span class="str">"%SystemDrive%\inetpub\wwwroot"</span> /&gt;</pre>
        
        <pre class="alt">        &lt;/application&gt;</pre>
        
        <pre>        ...</pre>
        
        <pre class="alt">        ...</pre>
        
        <pre>        ...</pre>
        
        <pre class="alt">        &lt;bindings&gt;</pre>
        
        <pre>            &lt;binding protocol=<span class="str">"http"</span> bindingInformation=<span class="str">"*:80:"</span> /&gt;</pre>
        
        <pre class="alt">            <strong><font color="#000000" style="background-color: rgb(255, 255, 0);">&lt;binding protocol=<span class="str">"https"</span> bindingInformation=<span class="str">"*:443:"</span> sslFlags=<span class="str">"0"</span> /&gt;</font></strong></pre>
        
        <pre>        &lt;/bindings&gt;</pre>
        
        <pre class="alt">        &lt;traceFailedRequestsLogging enabled=<span class="str">"true"</span> /&gt;</pre>
        
        <pre>&lt;/site&gt;</pre></p>
      </div>
    </td>
  </tr>
</table>

<div class="csharpcode">
  <pre></pre>
</div>

<font size="2">As seen above lot of information has been removed from the config file. There were no duplication of efforts due to the removal of the cert related section from the config file, mainly due to <strong>KERNEL Mode SSL</strong> dependency. This reduced the size of the overall configuration file as well.</font>

<p align="center">
  <font size="5" face="Segoe UI"><font style="font-weight: bold;" color="#0080ff"><u>Differences from UI Perspective:</u></font></font>
</p>

<font size="2">There was significant change as to what options were available in the IIS UI for the users when configuring SSL. This changed drastically from IIS 6 to IIS 7. Even the latest version of IIS, follows the same UI which was changed in IIS 7 with additions to incorporate the new functionalities.</font>

<font size="2">IIS 6 UI was pretty limited. There were several problems associated with it. The UI allowed only one certificate to be bound to the site irrespective of whether there were 2 or more combinations of IP+Port. The reason for this was that the UI for specifying the<strong> IP+Port</strong> was different than the one which was used to bind the certificate. These were presented to the user as 2 different sections and hence was a problem.</font>

<a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/1805.image_4EE9A0B0.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/1805.image_5F00_4EE9A0B0.png"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4572.image_thumb_2C949BE8.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/4572.image_5F00_thumb_5F00_2C949BE8.png" width="527" height="514" /></a>

<font size="2">To get the above UI:</font>

<font size="2"></font>

<font size="2"></font></p> 

  * <font size="2">Right click and go to the<strong> Web Site</strong> properties:</font>
<font size="2"></font>

  * <font size="2">Go to the <strong>Web Site</strong> tab.</font>
<font size="2"></font>

  * <font size="2">Under <strong>Web site identification </strong>click on <strong>Advanced…</strong></font>
<font size="2"></font>

  * <font size="2">Click on <strong>Add..</strong> under <strong>Multiple identities for this Web site</strong>.</font>
<font size="2"></font></ul> 

<font size="2"></font>

<font size="2">The above image is the UI to add the bindings for the web site. There is no option to choose the certificate or to specify the host header. The user can only specify the <strong>IP</strong> and <strong>Port</strong> and then he has to traverse to another section to choose the certificate for the site. </font>

<a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4555.image_423BA7FA.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/4555.image_5F00_423BA7FA.png"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6507.image_thumb_7C4D058A.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/6507.image_5F00_thumb_5F00_7C4D058A.png" width="544" height="526" /></a>

<font size="2">As shown above the UI to add a certificate is in a different tab altogether. Even if the user adds 3 distinct secureBindings, the UI allows only one certificate to be mapped to the Web site. This is because there was no way in the config to identify which bindings will use what certificate. As a result due to this, all the bindings for that site ended up using only one certificate. Not a ideal situation at all.</font>

* * *

<font size="2">All these short comings were addressed in IIS 7 and this has remained as a base for the future IIS versions too. take a loot at this UI:</font>

<a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/0333.image_3DDCEF32.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/0333.image_5F00_3DDCEF32.png"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8547.image_thumb_5FC851B6.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/8547.image_5F00_thumb_5F00_5FC851B6.png" width="677" height="319" /></a>

<font size="2">The UI is pretty simple. It allows the user to select a certificate for a corresponding <strong>IP+Port</strong> combination. The <strong>Host name</strong> section contains a textbox to specify the value, but is disabled by default (This is another shortcoming in <strong>IIS 7.x</strong> versions). This is enabled only if the certificate is a <strong>Wild Card certificate</strong> (If it’s a <strong>SAN</strong> certificate, the textbox would still remain disabled). When the user selects a certificate from the drop down list, it directly updates the registry values corresponding to the SSL binding.</font>

<p align="left">
  <font size="2"></font>
</p>

<table cellspacing="0" cellpadding="0" width="700" align="center" bgcolor="#cccccc" border="2">
  <tr>
    <td valign="top" width="696">
      <p>
        <font size="2">Here is the registry key where the SSL bindings are stored:</font>
      </p>
      
      <p>
        <font style="background-color: rgb(255, 255, 0);" size="2"><strong>HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\HTTP\Parameters\SslBindingInfo</strong></font>
      </p>
      
      <p>
        <font size="2">This can also be retrieved via <strong>command prompt </strong>by executing the following command:</font>
      </p>
      
      <blockquote>
        <p>
          <font style="background-color: rgb(255, 255, 0);" size="2"><strong>netsh http show sslcert</strong></font>
        </p>
      </blockquote>
    </td>
  </tr>
</table>

* * *

<font size="2">In <strong>IIS 8</strong>, not much was changed, but few additions and improvements were made to the overall SSL functionality. As I mentioned earlier, significant additions were made to make <strong>IIS</strong> scalable from <strong>IIS</strong> perspective, this was done by introducing <strong>SNI </strong>and <strong>CCS </strong>bindings. The above UI was improved slightly to incorporate the new additions and overcome the limitations of the previous version. The <strong>Host name</strong> text box remains enabled regardless of the certificate.</font>

<a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/0508.image_03869AB3.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/0508.image_5F00_03869AB3.png"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3021.image_thumb_754AB273.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/3021.image_5F00_thumb_5F00_754AB273.png" width="780" height="528" /></a>

<font size="2">There are few other changes which exist moving forth from IIS 6 to IIS 7 and are not pleasant. Yes I’m referring to Client Certificates.</font>

<font style="background-color: rgb(255, 255, 0);" color="#c0504d" size="2"><strong>IIS 7 onwards there is no UI to specify Client Certificate mapping.</strong></font>

<font size="2">However, citing these problems, the configuration editor was introduced as separate download for IIS 7 (It is available by default in IIS 7.5 and later versions).</font>

<font size="2">The configuration editor was a blessing in disguise for user who still use <strong>IIS Client Cert Authentication</strong>. However, the IIS 6 UI probably was better in this regards at least.</font>

<font size="2">With this, I am calling an end to the lengthy blog. I will update the list as I come across other differences between these IIS versions.</font>

<font size="2"></font>

<font size="2"></font>

<font size="2"></font>

<font size="2"></font>

<font size="2"></font>

<font size="2"></font>

<font size="2">&#160;</font>