---
id: 118
title: Server Name Indication (SNI) with IIS 8 (Windows Server 2012)
date: 2012-09-04T09:13:00+00:00
author: kaushal
layout: post
guid: https://blogs.msdn.microsoft.com/kaushal/2012/09/04/server-name-indication-sni-with-iis-8-windows-server-2012/
permalink: /2012/09/04/server-name-indication-sni-with-iis-8-windows-server-2012/
orig_url:
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2012/09/04/server-name-indication-sni-with-iis-8-windows-server-2012.aspx
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2012/09/04/server-name-indication-sni-with-iis-8-windows-server-2012.aspx
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2012/09/04/server-name-indication-sni-with-iis-8-windows-server-2012.aspx
orig_site_id:
  - "13803"
  - "13803"
  - "13803"
orig_post_id:
  - "10346227"
  - "10346227"
  - "10346227"
orig_parent_id:
  - "10346227"
  - "10346227"
  - "10346227"
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
  - http://blogs.msdn.com/b/kaushal/archive/2012/09/04/server-name-indication-sni-with-iis-8-windows-server-2012.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2012/09/04/server-name-indication-sni-with-iis-8-windows-server-2012.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2012/09/04/server-name-indication-sni-with-iis-8-windows-server-2012.aspx
orig_post_name:
  - server name indication sni in iis 8 windows server 2012
  - server name indication sni in iis 8 windows server 2012
  - server name indication sni in iis 8 windows server 2012
orig_thread_id:
  - "819481"
  - "819481"
  - "819481"
orig_post_author_email:
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
orig_attachment_count:
  - "0"
  - "0"
  - "0"
total_views:
  - "55402"
  - "55402"
  - "55402"
opengraph_tags:
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Server Name Indication (SNI) with IIS 8 (Windows Server 2012)" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/09/04/server-name-indication-sni-with-iis-8-windows-server-2012/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="&#160; In my previous article I discussed on how scalability was achieved in IIS 8. Here is the link: SSL Scalability with IIS 8. &#160; In this blog I will discuss specifically about Server Name Indication aka SNI. We will learn how scalability is achieved through this. &#160; During SSL handshake when the client sends..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8015.wlEmoticon-smile_2D39D042.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Server Name Indication (SNI) with IIS 8 (Windows Server 2012)" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/09/04/server-name-indication-sni-with-iis-8-windows-server-2012/" />
    <meta name="twitter:description" content="&#160; In my previous article I discussed on how scalability was achieved in IIS 8. Here is the link: SSL Scalability with IIS 8. &#160; In this blog I will discuss specifically about Server Name Indication aka SNI. We will learn how scalability is achieved through this. &#160; During SSL handshake when the client sends..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8015.wlEmoticon-smile_2D39D042.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Server Name Indication (SNI) with IIS 8 (Windows Server 2012)" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/09/04/server-name-indication-sni-with-iis-8-windows-server-2012/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="&#160; In my previous article I discussed on how scalability was achieved in IIS 8. Here is the link: SSL Scalability with IIS 8. &#160; In this blog I will discuss specifically about Server Name Indication aka SNI. We will learn how scalability is achieved through this. &#160; During SSL handshake when the client sends..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8015.wlEmoticon-smile_2D39D042.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Server Name Indication (SNI) with IIS 8 (Windows Server 2012)" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/09/04/server-name-indication-sni-with-iis-8-windows-server-2012/" />
    <meta name="twitter:description" content="&#160; In my previous article I discussed on how scalability was achieved in IIS 8. Here is the link: SSL Scalability with IIS 8. &#160; In this blog I will discuss specifically about Server Name Indication aka SNI. We will learn how scalability is achieved through this. &#160; During SSL handshake when the client sends..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8015.wlEmoticon-smile_2D39D042.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Server Name Indication (SNI) with IIS 8 (Windows Server 2012)" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/09/04/server-name-indication-sni-with-iis-8-windows-server-2012/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="&#160; In my previous article I discussed on how scalability was achieved in IIS 8. Here is the link: SSL Scalability with IIS 8. &#160; In this blog I will discuss specifically about Server Name Indication aka SNI. We will learn how scalability is achieved through this. &#160; During SSL handshake when the client sends..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8015.wlEmoticon-smile_2D39D042.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Server Name Indication (SNI) with IIS 8 (Windows Server 2012)" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/09/04/server-name-indication-sni-with-iis-8-windows-server-2012/" />
    <meta name="twitter:description" content="&#160; In my previous article I discussed on how scalability was achieved in IIS 8. Here is the link: SSL Scalability with IIS 8. &#160; In this blog I will discuss specifically about Server Name Indication aka SNI. We will learn how scalability is achieved through this. &#160; During SSL handshake when the client sends..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8015.wlEmoticon-smile_2D39D042.png" />
    
categories:
  - Uncategorized
---
<div class="WordSection1" align="left">
  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">&#160;</font></span>
</div>

<div class="WordSection1" align="left">
  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">In my previous article I discussed on how scalability was achieved in IIS 8. </font></span>
</div>

<p class="MsoNormal" style="text-align: justify" align="left">
  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">Here is the link: </font></span><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><a href="http://blogs.msdn.com/b/kaushal/archive/2012/08/08/ssl-scalability-with-iis-8-windows-8-server.aspx"><font size="2"><u>SSL Scalability with IIS 8</u></font></a></span><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">.</font></span>
</p>

<p class="MsoNormal" style="text-align: justify" align="left">
  <font size="2"><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;">&#160;</span></font>
</p>

<p class="MsoNormal" style="text-align: justify" align="left">
  <font size="2"><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"></span><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;">In this blog I will discuss specifically about <b>Server Name Indication</b> aka <b>SNI</b>. We will learn how scalability is achieved through this.</span></font>
</p>

<p class="MsoNormal" style="text-align: justify">
  <font size="2"><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;">&#160;</span></font>
</p>

<p class="MsoNormal" style="text-align: justify">
  <font size="2"><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"></span><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;">During SSL handshake when the client sends a <b>HTTPS</b> request (Client Hello) to the web server, the HTTP headers are not available to the server. Once the SSL handshake is completed the client will encrypt the headers and send the encrypted HTTP request to the server. Therefore server cannot access the HTTP headers or the content until the request is encrypted. Hence, the problem. <img class="wlEmoticon wlEmoticon-smile" alt="Smile" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8015.wlEmoticon-smile_2D39D042.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/8015.wlEmoticon_2D00_smile_5F00_2D39D042.png" /></span></font>
</p>

<p class="MsoNormal" style="text-align: justify">
  <font size="2"><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;">&#160;</span></font>
</p>

<p class="MsoNormal" style="text-align: justify">
  <font size="2"><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"></span></font><font size="2"><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;">Before decrypting the request the only information available to the server will be the IP Address and the Port number. This is available through the TCP headers as only the HTTP headers are encrypted. This leads to the limitation of only one certificate can be bound to a combination of </span><font face="Segoe UI"><b><span style="font-family: &quot;Courier New&quot;"><IPAddress>:<Port></span></b><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;">.</span></font></font>
</p>

<p class="MsoNormal" style="text-align: justify">
  <font size="2"><font face="Segoe UI"><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;">&#160;</span></font></font>
</p>

<p class="MsoNormal" style="text-align: justify">
  <b><u><span style="font-size: 12pt; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; line-height: 106%"><font size="4">Legacy SSL handshake between client and IIS 7.x and earlier</font></span></u></b>
</p>

<div class="WordSection1">
</div>

<div class="WordSection1">
  <ol>
    <li>
      <font size="2" face="Segoe UI">The client and the server establish a <b>TCP</b> connection via <b>TCP handshake</b>.</font> <font size="2" face="Segoe UI"></font>
    </li>
    <li>
      <font size="2" face="Segoe UI">The client then sends a <b>Client Hello</b> to the server. The only information available to the server from <b>Client Hello</b> is the <b>IPAddress</b> and the <b>Port</b>. The client sends a specific protocol version and the list of supported cipher suites as part of this client hello.</font> <font size="2" face="Segoe UI"></font>
    </li>
    <li>
      <font face="Segoe UI"><font size="2">The server checks the registry to find a <strong>certificate hash</strong>/<strong>thumbprint </strong>corresponding to the above combination of <b>IP:Port</b>. The server checks the below key to find the combination: <font style="background-color: rgb(255,255,0)"><b>HKLM\SYSTEM\CurrentControlSet\Services\HTTP\Parameters\SslBindingInfo</b><b></b></font></font></font> <font size="2" face="Segoe UI"></font>
    </li>
    <li>
      <font size="2" face="Segoe UI">Once it finds a match, the crypto API’s are called to retrieve the Server Certificate based on the thumbprint from the certificate store. This is then added to the <strong>Server Hello </strong>and sent to the client.</font>
    </li>
    <li>
      <font size="2" face="Segoe UI">The HTTP headers are not sent until the handshake is complete, as a result the server never knows which site/application the request corresponds to until the handshake completes.</font>
    </li>
  </ol>
</div>

<font size="2" face="Segoe UI"><strong>NOTE</strong>: The Public key cryptography is used to decide on a symmetric key (session key), which is then used by the client and the server for both encryption and decryption of the HTTP Headers and the content body. If you realized by now, SSL handshake involves both asymmetric encryption and symmetric encryption. Symmetric encryption is used for encryption of the actual data.</font>

<font size="2" face="Segoe UI"></font> 

<p class="MsoNormal" style="text-align: justify">
  &#160;
</p>

<font size="2" face="Segoe UI"></font> 

<p class="MsoNormal" style="text-align: justify" align="left">
  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">All the SSL bindings on Windows OS prior to <strong>Windows Server 2008 R2/Windows 7 </strong>can be found under following registry key:</font></span>
</p>

<p class="MsoNormal" style="text-align: justify" align="left">
  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">&#160;</font></span>
</p>

<font size="2" face="Segoe UI"></font> 

<p class="MsoNormal" style="text-align: justify">
  <b><span style="font-size: 9pt; font-family: &quot;Courier New&quot;; background: yellow; line-height: 106%"><font size="2" face="Segoe UI">HKLM\SYSTEM\CurrentControlSet\Services\HTTP\Parameters\SslBindingInfo</font></span></b>
</p>

<font size="2" face="Segoe UI"></font> 

<p class="MsoNormal" style="text-align: justify">
  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">&#160;</font></span>
</p>

<p class="MsoNormal" style="text-align: justify">
  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">Even if the client provides the server name in the client hello, the server wasn’t capable of using it. <span style="background: lime">This is addressed in IIS 8</span>. </font></span><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">To solve this problem associated with SSL/TLS, IETF added a new TLS extension called <b>Server Name Indication</b>. It is mentioned in the following RFC’s</font></span>
</p>

  * <u><font size="2" face="Segoe UI"><a href="http://tools.ietf.org/html/rfc3546#section-3.1">RFC 3546</a></font></u> <font size="2" face="Segoe UI">– Section 3.1</font> <font size="2" face="Segoe UI"></font>
  * <u><font size="2" face="Segoe UI"><a href="http://tools.ietf.org/html/rfc4366#section-3.1">RFC 4366</a></font></u> <font size="2" face="Segoe UI">– Section 3.1</font> 
  * <u><font size="2" face="Segoe UI"><a href="http://tools.ietf.org/html/rfc6066#section-3">RFC 6066</a></font></u> <font size="2" face="Segoe UI">– Section 3</font> 

<p class="MsoNormal" style="text-align: justify">
  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"></span><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">You could also read about </font><a href="http://en.wikipedia.org/wiki/Server_Name_Indication"><font size="2"><u>SNI on Wikipedia</u></font></a><font size="2">.</font></span>
</p>

<font size="2" face="Segoe UI"></font> 

<p class="MsoNormal" style="text-align: justify">
  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">As mentioned in the above RFC’s a TLS extension called <b>ServerName </b>was introduced to tackle this problem. Below is a snippet from <a href="http://tools.ietf.org/html/rfc6066#section-3"><u>RFC 6066</u></a>.</font></span>
</p>

<p class="MsoNormal" style="text-align: justify">
  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">&#160;</font></span>
</p>

<table cellspacing="0" cellpadding="2" width="605" border="3">
  <tr>
    <td bgcolor="#6e6a6b" valign="top" width="603">
      <div align="left">
        <pre><b><font size="2">East Lake                  </font></b><b><font size="2">Standards Track                      [Page 5]</font></b></pre></p>
      </div>
      
      <div align="left">
        <pre><b><font size="2">RFC 6066              TLS Extension Definitions               April 2011</font></b></pre></p>
      </div>
      
      <pre><b><font size="2" face="Courier New">3. Server Name Indication</font></b></pre>
      
      <p>
        <b><font size="2" face="Courier New">TLS does not provide a mechanism for a client to tell a server the </font></b><b><font size="2" face="Courier New">name of the server it is contacting. It may be desirable for clients </font></b><b><font size="2" face="Courier New">to provide this information to facilitate secure connections to </font></b><b><font size="2" face="Courier New">servers that host multiple &#8216;virtual&#8217; servers at a single underlying </font></b><b><font size="2" face="Courier New">network address.</font></b>
      </p>
      
      <p>
        <b><font size="2" face="Courier New">In order to provide the server name, clients MAY include an extension </font></b><b><font size="2" face="Courier New">of type "server_name" in the (extended) client hello. The </font></b><b><font size="2" face="Courier New">"extension_data" field of this extension SHALL contain </font></b><b><font size="2" face="Courier New">"ServerNameList" where:</font></b>
      </p>
      
      <p>
        <b><font size="2" face="Courier New"></font></b>
      </p>
      
      <p>
        <b><font size="2" face="Courier New">&#160;&#160;&#160;&#160;&#160; struct {</font></b>
      </p>
      
      <p>
        <b><font size="2" face="Courier New">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; NameType name_type;<br /> <br /></font></b><b><font size="2" face="Courier New">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </font></b><b><font size="2" face="Courier New">select (name_type) {<br /> <br /></font></b><b><font size="2" face="Courier New">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </font></b><b><font size="2" face="Courier New">case host_name: HostName;<br /> <br /></font></b><b><font size="2" face="Courier New">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; } name;<br /> <br /></font></b><b><font size="2" face="Courier New">&#160;&#160;&#160;&#160;&#160; } ServerName;</font></b>
      </p>
      
      <p>
        <b><font size="2" face="Courier New"></font></b>
      </p>
      
      <p>
        <b><font size="2" face="Courier New">&#160;&#160;&#160;&#160;&#160; enum {<br /> <br /></font></b><b><font size="2" face="Courier New">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; host_name(0), (255)<br /> <br />&#160;&#160;&#160;&#160;&#160; </font></b><b><font size="2" face="Courier New">} NameType;</font></b>
      </p>
      
      <p>
        <strong><font size="2" face="Courier New"></font></strong>
      </p>
      
      <p>
        <b><font size="2" face="Courier New">&#160;&#160;&#160;&#160;&#160; opaque HostName<1..2^16-1>;</font></b>
      </p>
      
      <p>
        <strong><font size="2" face="Courier New"></font></strong>
      </p>
      
      <p>
        <b><font size="2" face="Courier New">&#160;&#160;&#160;&#160;&#160;&#160; struct {<br /> <br />&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </font></b><b><font size="2" face="Courier New">ServerName server_name_list<1..2^16-1><br /> <br /></font></b><b><font size="2" face="Courier New">&#160;&#160;&#160;&#160;&#160;&#160; }ServerNameList;</font></b>
      </p>
    </td>
  </tr>
</table>

<font size="2" face="Segoe UI"></font>

<p class="MsoNormal" style="text-align: justify" align="left">
  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">&#160;</font></span>
</p>

<p class="MsoNormal" style="text-align: justify" align="left">
  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">Now the client can send the hostname it wants to access over https as a part of client hello. This helps the server to associate the client hello to a specific request and thus we overcome the limitation which was imposed earlier.</font></span>
</p>

<p class="MsoNormal" style="text-align: justify" align="left">
  <font size="2"><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;">&#160;</span></font>
</p>

<p class="MsoNormal" style="text-align: justify" align="left">
  <font size="2"><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"></span><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;">If you were to capture a network trace of SNI complaint browser accessing a HTTPS site you could see this extension as part of the client hello. I captured a <b>Wireshark</b> trace while accessing <a href="https://www.outlook.com">https://www.outlook.com</a>. I filtered the trace by <b>SSL</b> and searched for <b>Client Hello</b>.</span></font>
</p>

<p class="MsoNormal" style="text-align: justify" align="left">
  <font size="2"><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;">&#160;</span></font>
</p>

<p class="MsoNormal" style="text-align: justify" align="left">
  <a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/2742.image_708FDEC8.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/2742.image_5F00_708FDEC8.png"><img title="image" style="float: none; margin-left: auto; display: block; margin-right: auto" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/0576.image_thumb_3ED4C173.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/0576.image_5F00_thumb_5F00_3ED4C173.png" width="606" height="558" /></a>
</p>

<font size="2" face="Segoe UI"></font>

<p class="MsoNormal" style="text-align: center" align="center">
  <b><span style="font-size: 14pt; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; color: red; line-height: 106%"><font color="#ff0000" size="1"><font color="#000000"><u>snapshot of a SSL trace in Wireshark</u></font>&#160;</font></span></b>
</p>

<p class="MsoNormal" style="text-align: center" align="center">
  <b><span style="font-size: 14pt; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; color: red; line-height: 106%"><font size="1">&#160;</font></span></b>
</p>

<p class="MsoNormal" style="text-align: center" align="center">
  <b><span style="font-size: 14pt; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; color: red; line-height: 106%"><font color="#ff0000" size="4"><u>***IMPORTANT***</u></font></span></b>
</p>

<font size="2" face="Segoe UI"></font>

<p class="MsoNormal" style="text-align: justify">
  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">&#160;</font></span>
</p>

<p class="MsoNormal" style="text-align: justify">
  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">One important thing to note here is that <b>SNI</b> is part of the <b>Client Hello</b>. So it is the client browsers that need to support this extension. Most of the current day browsers support SNI.</font></span>
</p>

<p class="MsoNormal" style="text-align: justify">
  <font size="2"><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;">&#160;</span></font>
</p>

<p class="MsoNormal" style="text-align: justify">
  <font size="2"><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"></span><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;">However, there are few browsers out there that don’t support SNI. For example, on Windows OS any version of IE running on Windows XP or lower versions do not support SNI. Vista onwards support for SNI was included for IE 7 and higher. There is a good list on Wikipedia on browsers that provide support for SNI. Below is a snippet from Wikipedia:</span></font>
</p>

<p class="MsoNormal" style="text-align: justify">
  <font size="2"><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;">&#160;</span></font>
</p>

<p class="MsoNormal" style="text-align: justify">
  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><strong><u><font size="3">List of SNI Compliant Browsers:</font></u></strong></span>
</p>

<table cellspacing="0" cellpadding="2" width="604" border="3">
  <tr>
    <td bgcolor="#47bbff" valign="top" width="602">
      <ul>
        <li>
          <font face="Segoe UI"><font size="2"><b>Internet Explorer</b> 7 or later, on Windows Vista or higher. Does not work on Windows XP, even Internet Explorer 8.</font></font> <font size="2" face="Segoe UI"></font>
        </li>
        <li>
          <font face="Segoe UI"><font size="2"><b>Mozilla Firefox</b> 2.0 or later</font></font> <font size="2" face="Segoe UI"></font>
        </li>
        <li>
          <font face="Segoe UI"><font size="2"><b>Opera 8.0</b> or later (the TLS 1.1 protocol must be enabled)</font></font> <font size="2" face="Segoe UI"></font>
        </li>
        <li>
          <font face="Segoe UI"><font size="2"><b>Opera Mobile</b> at least version 10.1 beta on Android[citation needed]</font></font> <font size="2" face="Segoe UI"></font>
        </li>
        <li>
          <font face="Segoe UI"><font size="2"><b>Google Chrome</b> (Vista or higher. XP on Chrome 6 or newer.[6] OS X 10.5.7 or higher on Chrome 5.0.342.1 or newer)</font></font> <font size="2" face="Segoe UI"></font>
        </li>
        <li>
          <font face="Segoe UI"><font size="2"><b>Safari </b>2.1 or later (Mac OS X 10.5.6 or higher and Windows Vista or higher)</font></font> <font size="2" face="Segoe UI"></font>
        </li>
        <li>
          <font face="Segoe UI"><font size="2"><b>Konqueror/KDE</b> 4.7 or later [7]</font></font> <font size="2" face="Segoe UI"></font>
        </li>
        <li>
          <font face="Segoe UI"><font size="2"><b>MobileSafari</b> in Apple iOS 4.0 or later[8]</font></font> <font size="2" face="Segoe UI"></font>
        </li>
        <li>
          <font face="Segoe UI"><font size="2"><b>Android</b> default browser on Honeycomb (v3.x) or newer[9]</font></font> <font size="2" face="Segoe UI"></font>
        </li>
        <li>
          <b><font size="2" face="Segoe UI">Windows Phone 7</font></b> <font size="2" face="Segoe UI"></font>
        </li>
        <li>
          <font face="Segoe UI"><font size="2"><b>MicroB</b> on <b>Maemo</b></font></font>
        </li>
      </ul>
    </td>
  </tr>
</table>

<p class="MsoNormal" style="text-align: justify">
  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">&#160;</font></span>
</p>

<p class="MsoNormal" style="text-align: justify">
  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">So far I was trying to explain the basics of SNI. We need to know this to understand the server side solution for this.</font></span>
</p>

<p class="MsoNormal" style="text-align: justify">
  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">&#160;</font></span>
</p>

<font size="2" face="Segoe UI"></font><font style="background-color: rgb(165,165,165)"></font>

<p class="MsoNormal" style="text-align: justify">
  <font size="2"><font style="background-color: rgb(165,165,165)"><b><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;">NOTE</span></b><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;">: SNI is available only on IIS 8 and may be future versions. It is not available on any of the previous versions of IIS like IIS 7.x, IIS6 etc.</span></font></font>
</p>

<font size="2" face="Segoe UI"></font>

<p class="MsoNormal" style="text-align: center" align="center">
  <b><u><span style="font-size: 16pt; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; line-height: 106%"><font size="4">SNI on IIS 8</font></span></u></b>
</p>

<font size="2" face="Segoe UI"></font>

<p class="MsoNormal" style="text-align: justify">
  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">&#160;</font></span>
</p>

<p class="MsoNormal" style="text-align: justify">
  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">IIS 8 supports <b>Server Name Indication</b>. <span style="background: lime; color: black">This is enabled by default</span><span style="color: black"> </span>and no separate installation is required. Now while adding a <b>HTTPS</b> binding for a website on IIS 8, the option to enable <b>SNI</b> is available. This is how the UI looks like:</font></span>
</p>

<font size="2" face="Segoe UI"></font>

<p class="MsoNormal" style="text-align: justify">
  <a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/1643.image_748A06CD.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/1643.image_5F00_748A06CD.png"><img title="image" style="background-image: none; display: inline" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8512.image_thumb_532A6131.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/8512.image_5F00_thumb_5F00_532A6131.png" width="517" height="310" /></a>
</p>

<font size="2" face="Segoe UI"></font>

<p class="MsoNormal" style="text-align: justify">
  &#160;
</p>

<font size="2" face="Segoe UI"></font>

<p class="MsoNormal" style="text-align: justify">
  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">There are 2 things to remember when enabling SNI for a specific site on the server.</font></span>
</p>

  * <div class="MsoNormal" style="text-align: justify">
      <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"></span><font size="2"><font face="Segoe UI"><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;">Selecting the above option enforces the site to use <b>SNI</b> i.e., it will expect the client to send a <b>server_name</b> as the part of the <b>Client Hello</b> during <b>SSL handshake</b>. If the <b>server_name</b> extension is not present then the SSL handshake would fail.</span></font></font>
    </div>

  * <div class="MsoNormal" style="text-align: justify">
      <font size="2"><font face="Segoe UI"><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"></span></font></font><font size="2"><font face="Segoe UI"><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;">The hostname has to be provided, this is a strict mandate. The server will use this information to associate an incoming request to a specific site.</span></font></font>
    </div>

<font size="2" face="Segoe UI"></font>

<p class="MsoNormal" style="text-align: justify">
  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">&#160;</font></span><b><span style="font-size: 14pt; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; line-height: 106%"><font size="4"><u>How does the IIS know if a specific binding uses SNI?</u></font></span></b>
</p>

<font size="2" face="Segoe UI"></font>

<p class="MsoNormal" style="text-align: justify">
  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">&#160;</font></span>
</p>

<p class="MsoNormal" style="text-align: justify">
  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">When a SSL bindings is added for a site, there is also a small change in the configuration file i.e., the applicationhost.config. This is how the binding section looks like:</font></span>
</p>

<table cellspacing="0" cellpadding="2" width="582" border="3">
  <tr>
    <td bgcolor="#4c787e" valign="top" width="580">
      <p>
        <font size="2" face="Courier New"><font color="#ffffff"><strong><bindings><br /> <br /><binding protocol="https" bindingInformation="*:443:SNI.IIS8.com"</strong></font> <font style="background-color: rgb(255,255,0)"><b>sslFlags</b>="1"</font> <strong><font color="#ffffff">/></font></strong> </p> 
        
        <p>
          <strong><font color="#ffffff"></bindings></font></strong></font>
        </p></td> </tr> </tbody> </table> 
        
        <p>
          <font size="2" face="Segoe UI"></font>
        </p>
        
        <p class="MsoNormal" style="text-align: justify">
          <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">&#160;</font></span>
        </p>
        
        <p class="MsoNormal" style="text-align: justify">
          <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">The highlighted attribute called <b><font style="background-color: rgb(255,255,0)" size="3">sslFlags</font> </b>is. This attribute tells IIS what type of binding it is. This flag can be thought of as a doing an OR operation on 2 variables x and y. Below table would give you a gist of what this flag signifies.</font></span>
        </p>
        
        <p class="MsoNormal" style="text-align: justify">
          <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">&#160;</font></span>
        </p>
        
        <table cellspacing="0" cellpadding="2" width="574" border="2">
          <tr>
            <td bgcolor="#c35617" valign="top" width="56">
              <font size="4" face="Segoe UI"><strong>Using<br /> <br />&#160; CCS</strong></font>
            </td>
            
            <td bgcolor="#c35617" valign="top" width="59">
              <font size="4" face="Segoe UI"><strong>Using<br /> <br />&#160; SNI</strong></font>
            </td>
            
            <td bgcolor="#c35617" valign="top" width="76">
              <p align="center">
                <font size="4" face="Segoe UI"><strong>sslFlags</strong></font>
              </p>
            </td>
            
            <td bgcolor="#c35617" valign="top" width="381">
              <p align="center">
                <font size="4" face="Segoe UI"><strong>Description</strong></font>
              </p>
            </td>
          </tr>
          
          <tr>
            <td bgcolor="#ffff00" valign="top" width="56">
              <p align="center">
                <font size="4" face="Segoe UI"><strong></strong></font>
              </p>
            </td>
            
            <td bgcolor="#ffff00" valign="top" width="59">
              <p align="center">
                <font size="4" face="Segoe UI"><strong></strong></font>
              </p>
            </td>
            
            <td bgcolor="#95b9c7" valign="top" width="76">
              <p align="center">
                <font size="4" face="Segoe UI"><strong></strong></font>
              </p>
            </td>
            
            <td bgcolor="#95b9c7" valign="top" width="381">
              <p align="center">
                <font size="3" face="Segoe UI">Legacy SSL binding. Neither uses SNI nor CCS</font>
              </p>
            </td>
          </tr>
          
          <tr>
            <td bgcolor="#ffff00" valign="top" width="56">
              <p align="center">
                <font size="4" face="Segoe UI"><strong></strong></font>
              </p>
            </td>
            
            <td bgcolor="#ffff00" valign="top" width="59">
              <p align="center">
                <font size="4" face="Segoe UI"><strong>1</strong></font>
              </p>
            </td>
            
            <td bgcolor="#95b9c7" valign="top" width="76">
              <p align="center">
                <font size="4" face="Segoe UI"><strong>1</strong></font>
              </p>
            </td>
            
            <td bgcolor="#95b9c7" valign="top" width="381">
              <p align="center">
                <font size="3" face="Segoe UI">SSL binding using SNI.</font>
              </p>
            </td>
          </tr>
          
          <tr>
            <td bgcolor="#ffff00" valign="top" width="56">
              <p align="center">
                <font size="4" face="Segoe UI"><strong>1</strong></font>
              </p>
            </td>
            
            <td bgcolor="#ffff00" valign="top" width="59">
              <p align="center">
                <font size="4" face="Segoe UI"><strong></strong></font>
              </p>
            </td>
            
            <td bgcolor="#95b9c7" valign="top" width="76">
              <p align="center">
                <font size="4" face="Segoe UI"><strong>2</strong></font>
              </p>
            </td>
            
            <td bgcolor="#95b9c7" valign="top" width="381">
              <p align="center">
                <font size="3" face="Segoe UI">SSL binding uses CCS, but SNI is not enforced.</font>
              </p>
            </td>
          </tr>
          
          <tr>
            <td bgcolor="#ffff00" valign="top" width="56">
              <p align="center">
                <font size="4" face="Segoe UI"><strong>1</strong></font>
              </p>
            </td>
            
            <td bgcolor="#ffff00" valign="top" width="59">
              <p align="center">
                <font size="4" face="Segoe UI"><strong>1</strong></font>
              </p>
            </td>
            
            <td bgcolor="#95b9c7" valign="top" width="76">
              <p align="center">
                <font size="4" face="Segoe UI"><strong>3</strong></font>
              </p>
            </td>
            
            <td bgcolor="#95b9c7" valign="top" width="381">
              <p align="center">
                <font size="3" face="Segoe UI">SSL binding uses CCS, but SNI is enforced.</font>
              </p>
            </td>
          </tr>
        </table>
        
        <p class="MsoNormal" style="text-align: justify">
          <font size="2"><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"></span></font><font size="2" face="Segoe UI">&#160;</font>
        </p>
        
        <p class="MsoNormal" style="text-align: center" align="center">
          <b><u><span style="font-size: 16pt; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; line-height: 106%"><font size="4">Changes in Registry</font></span></u></b>
        </p>
        
        <p class="MsoNormal" style="text-align: justify">
          <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">&#160;</font></span>
        </p>
        
        <p class="MsoNormal" style="text-align: justify">
          <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">In IIS 8 we have a new registry key where all the SNI bindings are stored. I had mentioned this in my previous blog post. This location of this registry key is </font></span>
        </p>
        
        <p>
          <font size="2" face="Segoe UI"></font>
        </p>
        
        <p class="MsoNormal" style="text-align: justify">
          <b><span style="font-size: 9pt; font-family: &quot;Courier New&quot;; background: yellow; line-height: 106%"><font size="2" face="Segoe UI">HKLM\SYSTEM\CurrentControlSet\Services\HTTP\Parameters\SslSniBindingInfo</font></span></b>
        </p>
        
        <p>
          <font size="2" face="Segoe UI"></font>
        </p>
        
        <p class="MsoNormal" style="text-align: justify">
          <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">&#160;</font></span>
        </p>
        
        <p class="MsoNormal" style="text-align: justify">
          <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">Executing the following command “netsh http show sslcert” will read this key and show a formatted output as shown below:</font></span>
        </p>
        
        <p class="MsoNormal" style="text-align: justify">
          <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">&#160;</font></span>
        </p>
        
        <p>
          <font size="2" face="Courier New"></font><font size="2" face="Courier New"></font><font size="2" face="Courier New"></font>
        </p>
        
        <table class="MsoTableGrid" style="background: rgb(0,32,96); border-collapse: collapse" cellspacing="0" cellpadding="0" width="609" border="1">
          <tr>
            <td style="border-top: windowtext 1pt solid; border-right: windowtext 1pt solid; border-bottom: windowtext 1pt solid; padding-bottom: 0cm; padding-top: 0cm; padding-left: 5.4pt; border-left: windowtext 1pt solid; padding-right: 5.4pt; width: 417.95pt" valign="top" width="607">
              <span style="font-size: 9pt; font-family: &quot;Courier New&quot;; line-height: 106%"><font color="#ffffff" size="2"><font style="background-color: rgb(255,255,0)" color="#000000"><strong>C:\>netsh http show sslcert</strong></font> </p> 
              
              <p>
                SSL Certificate bindings:
              </p>
              
              <p>
                </font></span><span style="font-size: 9pt; font-family: &quot;Courier New&quot;; line-height: 106%"><font color="#ffffff" size="2">&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;-<br /> <br /></font></span><font size="2" face="Courier New"></font><span style="font-size: 9pt; font-family: &quot;Courier New&quot;; line-height: 106%"><font color="#ffffff" size="2"><font style="background-color: rgb(255,255,0)" color="#000000" size="3"><strong>Hostname:port&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; : SNI.IIS8.com:443<br /> <br /></strong></font></font></span><font size="2"><span style="font-size: 9pt; font-family: &quot;Courier New&quot;; line-height: 106%"><font color="#ffffff">Certificate Hash&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; : 8d90a17d2851f802b0a5619bf695b03544b8f5cb<br /> <br /></font></span><span style="font-size: 9pt; font-family: &quot;Courier New&quot;; line-height: 106%"><font color="#ffffff">Application ID&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; : {4dc3e181-e14b-4a21-b022-59fc669b0914}</font></span></font><font size="2" face="Courier New"><br /> <br /></font><span style="font-size: 9pt; font-family: &quot;Courier New&quot;; line-height: 106%"><font color="#ffffff" size="2">Certificate Store Name&#160;&#160;&#160;&#160;&#160;&#160; : My<br /> <br /></font></span><span style="font-size: 9pt; font-family: &quot;Courier New&quot;; line-height: 106%"><font color="#ffffff" size="2">Verify Client Certificate Revocation : Enabled<br /> <br /></font></span><span style="font-size: 9pt; font-family: &quot;Courier New&quot;; line-height: 106%"><font color="#ffffff" size="2">Verify Revocation Using Cached Client Certificate Only : Disabled<br /> <br /></font></span><span style="font-size: 9pt; font-family: &quot;Courier New&quot;; line-height: 106%"><font color="#ffffff" size="2">Usage Check&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; : Enabled<br /> <br /></font></span><span style="font-size: 9pt; font-family: &quot;Courier New&quot;; line-height: 106%"><font color="#ffffff" size="2">Revocation Freshness Time&#160;&#160;&#160; : 0<br /> <br /></font></span><span style="font-size: 9pt; font-family: &quot;Courier New&quot;; line-height: 106%"><font color="#ffffff" size="2">URL Retrieval Timeout&#160;&#160;&#160;&#160;&#160;&#160;&#160; : 0<br /> <br /></font></span><span style="font-size: 9pt; font-family: &quot;Courier New&quot;; line-height: 106%"><font color="#ffffff" size="2">Ctl Identifier&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; : (null)<br /> <br /></font></span><span style="font-size: 9pt; font-family: &quot;Courier New&quot;; line-height: 106%"><font color="#ffffff" size="2">Ctl Store Name&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; : (null)<br /> <br /></font></span><font size="2"><span style="font-size: 9pt; font-family: &quot;Courier New&quot;; line-height: 106%"><font color="#ffffff">DS Mapper Usage&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; : Disabled<br /> <br /></font></span><span style="font-size: 9pt; font-family: &quot;Courier New&quot;; line-height: 106%"><font color="#ffffff">Negotiate Client Certificate&#160;&#160;&#160; : Disabled</font></span><font face="Courier New">&#160; </font></font>
              </p>
              
              <p>
                &#160;&#160;&#160;&#160;&#160;&#160; <font size="2" face="Segoe UI"></font></td> </tr> </tbody> </table> 
                
                <p>
                  <font size="2" face="Segoe UI"></font>
                </p>
                
                <p class="MsoNormal" style="text-align: justify">
                  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">&#160;</font></span>
                </p>
                
                <p class="MsoNormal" style="text-align: justify">
                  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">So now we have 3 types of SSL bindings:</font></span>
                </p>
                
                <ol>
                  <li>
                    <div class="MsoNormal" style="text-align: justify">
                      <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"></span><font size="2"><b><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;">IP:Port</span></b><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"> – Legacy SSL binding.</span></font>
                    </div>
                  </li>
                  
                  <li>
                    <div class="MsoNormal" style="text-align: justify">
                      <font size="2"><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"></span></font><font size="2"><b><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;">Hostname:Port</span></b><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"> – SSL binding using SNI. (new in <b>IIS 8</b>)</span></font>
                    </div>
                  </li>
                  
                  <li>
                    <div class="MsoNormal" style="text-align: justify">
                      <font size="2"><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"></span></font><font size="2"><b><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;">Central Certificate Store</span></b><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"> – SSL binding using Central Certificate Store. I will discuss this in detail in my next blog. (new in <b>IIS 8</b>)</span></font>
                    </div>
                  </li>
                </ol>
                
                <p>
                  <font size="2" face="Segoe UI"></font>
                </p>
                
                <p class="MsoNormal" style="text-align: justify">
                  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">There is a small problem that the administrators have to take care of while configuring SSL bindings to use SNI. If a non-SNI compliant browser connects to a site on which SNI is enforced, as I mentioned earlier the SSL handshake would fail.</font></span>
                </p>
                
                <p class="MsoNormal" style="text-align: justify">
                  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">&#160;</font></span>
                </p>
                
                <p>
                  <font size="2" face="Segoe UI"></font>
                </p>
                
                <p class="MsoNormal" style="text-align: justify">
                  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">To tackle this there is a fall-back mechanism in IIS where the it would try to determine a binding with the combination of IP:Port, if this is not present, then the SSL handshake fails. For this the IIS admin has to configure a binding which neither uses <b>SNI</b> nor <b>CCS</b>.</font></span>
                </p>
                
                <p class="MsoNormal" style="text-align: justify">
                  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">&#160;</font></span>
                </p>
                
                <p>
                  <font size="2" face="Segoe UI"></font>
                </p>
                
                <p class="MsoNormal" style="text-align: justify">
                  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">If legacy binding doesn’t exist, then the IIS UI will throw an alert as shown below. This message is a warning saying that there is no legacy binding, so in case of a failure the SSL handshake would fail.</font></span>
                </p>
                
                <p class="MsoNormal" style="text-align: justify">
                  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">&#160;</font></span>
                </p>
                
                <table cellspacing="0" cellpadding="2" width="187" align="center" border="2">
                  <tr>
                    <td bgcolor="#ede275" valign="top" width="185">
                      <p align="justify">
                        <font size="2" face="Segoe UI">No default SSL site has been created. To support browsers without SNI capabilities, it is recommended to create a default SSL site.</font>
                      </p>
                    </td>
                  </tr>
                </table>
                
                <p>
                  <font size="2" face="Segoe UI"></font>
                </p>
                
                <p class="MsoNormal" style="text-align: justify">
                  <a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8182.image_0A907260.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/8182.image_5F00_0A907260.png"><img title="image" style="display: inline" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4073.image_thumb_0EBA4A25.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/4073.image_5F00_thumb_5F00_0EBA4A25.png" width="588" height="446" /></a>
                </p>
                
                <p>
                  <font size="2" face="Segoe UI"></font>
                </p>
                
                <p class="MsoNormal" style="text-align: justify">
                  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">&#160;</font></span>
                </p>
                
                <p>
                  <font size="2" face="Segoe UI"></font>
                </p>
                
                <p class="MsoNormal">
                  <b><u><span style="font-size: 12pt; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; line-height: 106%">SSL Handshake between a SNI compliant browser and SNI Compliant Server</span></u></b>
                </p>
                
                <p>
                  <font size="2" face="Segoe UI"></font>
                </p>
                
                <p class="MsoNormal" style="text-align: justify">
                  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">&#160;</font></span>
                </p>
                
                <p class="MsoNormal" style="text-align: justify">
                  <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">Below are the steps involved during SSL handshake between a SNI compliant Client and a site hosted on IIS 8 on which a SSL binding is configured to use <b>SNI</b>.</font></span>
                </p>
                
                <ol>
                  <li>
                    <div class="MsoNormal" style="text-align: justify">
                      <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"></span><font size="2"><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;">The client and the server establish a <b>TCP</b> connection via <b>TCP handshake</b>.</span></font>
                    </div>
                  </li>
                  
                  <li>
                    <div class="MsoNormal" style="text-align: justify">
                      <font size="2"><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font face="Segoe UI">The client sends a <strong>Client Hello</strong> to the server. This packet contains the specific protocol version, list of supported cipher suites along with the hostname (let’s say <a href="http://www.outlook.com/">www.outlook.com</a> provided its a SNI compliant browser). The TCP/IP headers in the packet contain the <strong>IPAddress</strong> and the <strong>Port</strong> number.</font></span></font>
                    </div>
                  </li>
                  
                  <li>
                    <div class="MsoNormal" style="text-align: justify">
                      <font face="Segoe UI"><font size="2">The server checks the registry (legacy bindings) to find a <strong>certificate hash</strong>/<strong>thumbprint</strong> corresponding to the above combination of <strong>IP:Port.</strong></font></font>
                    </div>
                  </li>
                  
                  <li>
                    <div class="MsoNormal" style="text-align: justify" align="left">
                      <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"></span><font size="2"><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font face="Segoe UI">If there is no legacy binding for that <strong>IP:Port</strong>, then server uses hostname</font> information available from the Client Hello checks the registry to find a certificate hash corresponding to the above combination of <b>Hostname:Port</b>. The server checks the below key to find the combination: </p> 
                      
                      <p>
                        <strong><font style="background-color: rgb(255,255,0)">HKLM\SYSTEM\CurrentControlSet\Services\HTTP\Parameters\SslSniBindingInfo</font></strong></span></font></div> </li> 
                        
                        <li>
                          <div class="MsoNormal" style="text-align: justify">
                            <b><span style="font-size: 9pt; font-family: &quot;Courier New&quot;; background: yellow; line-height: 106%"></span></b><font size="2"><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;">If the above step fails i.e., if the server couldn’t find a corresponding hostname:port, then it would use the IPAddress available to search for a legacy SSL binding for that <b>IPAddress</b> and <b>PORT</b>. (If this is absent then the SSL handshake would fail)</span></font>
                          </div>
                        </li>
                        
                        <li>
                          <div class="MsoNormal" style="text-align: justify">
                            <font size="2"><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"></span></font><font size="2"><span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;">Once it finds a match, the crypto API’s are called to retrieve the Server Certificate based on the <strong>thumbprint</strong>/<strong>certificate hash</strong> from the certificate store. The retrieved certificate is then added to the <strong>Server Hello </strong>and sent to the client.</span></font> <font size="2" face="Segoe UI"></font>
                          </div>
                        </li></ol> 
                        
                        <p class="MsoNormal" style="text-align: justify" align="center">
                          <b><u><span style="font-size: 14pt; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; line-height: 106%"><font size="4">More Information:</font></span></u></b>
                        </p>
                        
                        <p>
                          <font size="2" face="Segoe UI"></font>
                        </p>
                        
                        <p class="MsoNormal" style="text-align: justify">
                          <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">&#160;</font></span>
                        </p>
                        
                        <p class="MsoNormal" style="text-align: justify">
                          <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font size="2">You could refer the following links on additional information on this topic:</font></span>
                        </p>
                        
                        <p>
                          <font size="2" face="Segoe UI"></font>
                        </p>
                        
                        <p class="MsoNormal" style="text-align: justify">
                          <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font color="#0000ff" size="2"><a href="http://en.wikipedia.org/wiki/Server_Name_Indication"><u>http://en.wikipedia.org/wiki/Server_Name_Indication</u></a></font><u><font color="#0000ff"> </font></u></span>
                        </p>
                        
                        <p>
                          <u><font color="#0000ff"><font size="2" face="Segoe UI"></font></font></u>
                        </p>
                        
                        <p class="MsoNormal" style="text-align: justify">
                          <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font color="#0000ff" size="2"><a href="http://learn.iis.net/page.aspx/1096/iis-80-server-name-indication-sni-ssl-scalability/"><u>http://learn.iis.net/page.aspx/1096/iis-80-server-name-indication-sni-ssl-scalability</u></a></font></span>
                        </p>
                        
                        <p>
                          <u><font color="#0000ff"><font size="2" face="Segoe UI"></font></font></u>
                        </p>
                        
                        <p class="MsoNormal" style="text-align: justify">
                          <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;"><font color="#0000ff" size="2"><a href="http://blogs.iis.net/yaminij/archive/2012/06/25/sni-server-name-indication-readiness-tool-draft.aspx"><u>http://blogs.iis.net/yaminij/archive/2012/06/25/sni-server-name-indication-readiness-tool-draft.aspx</u></a></font></span>
                        </p>