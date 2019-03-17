---
id: 339
title: SSL Handshake and HTTPS Bindings on IIS
date: 2013-08-02T18:43:00+00:00
author: kaushal
layout: post
guid: https://blogs.msdn.microsoft.com/kaushal/2013/08/02/ssl-handshake-and-https-bindings-on-iis/
permalink: /2013/08/02/ssl-handshake-and-https-bindings-on-iis/
orig_url:
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2013/08/03/ssl-handshake-and-https-bindings-on-iis.aspx
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2013/08/03/ssl-handshake-and-https-bindings-on-iis.aspx
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2013/08/03/ssl-handshake-and-https-bindings-on-iis.aspx
orig_site_id:
  - "13803"
  - "13803"
  - "13803"
orig_post_id:
  - "10439121"
  - "10439121"
  - "10439121"
orig_parent_id:
  - "10439121"
  - "10439121"
  - "10439121"
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
  - http://blogs.msdn.com/b/kaushal/archive/2013/08/02/ssl-handshake-and-https-bindings-on-iis.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2013/08/02/ssl-handshake-and-https-bindings-on-iis.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2013/08/02/ssl-handshake-and-https-bindings-on-iis.aspx
orig_post_name:
  - ssl handshake and https bindings on iis
  - ssl handshake and https bindings on iis
  - ssl handshake and https bindings on iis
orig_thread_id:
  - "849493"
  - "849493"
  - "849493"
orig_post_author_email:
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
orig_attachment_count:
  - "0"
  - "0"
  - "0"
total_views:
  - "36546"
  - "36546"
  - "36546"
opengraph_tags:
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="SSL Handshake and HTTPS Bindings on IIS" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2013/08/02/ssl-handshake-and-https-bindings-on-iis/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="Secure Socket Layer (SSL) also known as Transport Layer Security (TLS) is a cryptographic protocol which defines how 2 entities (client and server) communicate with each other securely. TLS is the successor of SSL. You can read more about it here: http://en.wikipedia.org/wiki/Transport_Layer_Security These are the following protocols which are most commonly used: SSL 2.0 SSL..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4336.080613_0416_SSLHandshak1.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="SSL Handshake and HTTPS Bindings on IIS" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2013/08/02/ssl-handshake-and-https-bindings-on-iis/" />
    <meta name="twitter:description" content="Secure Socket Layer (SSL) also known as Transport Layer Security (TLS) is a cryptographic protocol which defines how 2 entities (client and server) communicate with each other securely. TLS is the successor of SSL. You can read more about it here: http://en.wikipedia.org/wiki/Transport_Layer_Security These are the following protocols which are most commonly used: SSL 2.0 SSL..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4336.080613_0416_SSLHandshak1.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="SSL Handshake and HTTPS Bindings on IIS" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2013/08/02/ssl-handshake-and-https-bindings-on-iis/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="Secure Socket Layer (SSL) also known as Transport Layer Security (TLS) is a cryptographic protocol which defines how 2 entities (client and server) communicate with each other securely. TLS is the successor of SSL. You can read more about it here: http://en.wikipedia.org/wiki/Transport_Layer_Security These are the following protocols which are most commonly used: SSL 2.0 SSL..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4336.080613_0416_SSLHandshak1.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="SSL Handshake and HTTPS Bindings on IIS" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2013/08/02/ssl-handshake-and-https-bindings-on-iis/" />
    <meta name="twitter:description" content="Secure Socket Layer (SSL) also known as Transport Layer Security (TLS) is a cryptographic protocol which defines how 2 entities (client and server) communicate with each other securely. TLS is the successor of SSL. You can read more about it here: http://en.wikipedia.org/wiki/Transport_Layer_Security These are the following protocols which are most commonly used: SSL 2.0 SSL..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4336.080613_0416_SSLHandshak1.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="SSL Handshake and HTTPS Bindings on IIS" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2013/08/02/ssl-handshake-and-https-bindings-on-iis/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="Secure Socket Layer (SSL) also known as Transport Layer Security (TLS) is a cryptographic protocol which defines how 2 entities (client and server) communicate with each other securely. TLS is the successor of SSL. You can read more about it here: http://en.wikipedia.org/wiki/Transport_Layer_Security These are the following protocols which are most commonly used: SSL 2.0 SSL..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4336.080613_0416_SSLHandshak1.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="SSL Handshake and HTTPS Bindings on IIS" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2013/08/02/ssl-handshake-and-https-bindings-on-iis/" />
    <meta name="twitter:description" content="Secure Socket Layer (SSL) also known as Transport Layer Security (TLS) is a cryptographic protocol which defines how 2 entities (client and server) communicate with each other securely. TLS is the successor of SSL. You can read more about it here: http://en.wikipedia.org/wiki/Transport_Layer_Security These are the following protocols which are most commonly used: SSL 2.0 SSL..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4336.080613_0416_SSLHandshak1.png" />
    
categories:
  - Uncategorized
tags:
  - Server Authentication
  - SSL
  - SSL Handshake
  - TCP Handshake
  - TLS
  - TLS Handshake
format: link
---
<span style="font-family: Segoe UI;font-size: 10pt"><strong>Secure Socket Layer</strong> (<strong>SSL</strong>) also known as <strong>Transport Layer Security</strong> (<strong>TLS</strong>) is a cryptographic protocol which defines how 2 entities (client and server) communicate with each other securely. TLS is the successor of SSL. You can read more about it here: <a href="http://en.wikipedia.org/wiki/Transport_Layer_Security">http://en.wikipedia.org/wiki/Transport_Layer_Security</a> </span>

<span style="font-family: Segoe UI;font-size: 10pt">These are the following protocols which are most commonly used: </span>

  * <span style="font-family: Segoe UI;font-size: 10pt"><strong>SSL 2.0 </strong></span>
  * <span style="font-family: Segoe UI;font-size: 10pt"><strong>SSL 3.0 </strong></span>
  * <span style="font-family: Segoe UI;font-size: 10pt"><strong>TLS 1.0 (SSL 3.1) </strong></span>
  * <span style="font-family: Segoe UI;font-size: 10pt"><strong>TLS 1.1 (SSL 3.2) </strong></span>
  * <span style="font-family: Segoe UI;font-size: 10pt"><strong>TLS 1.2 (SSL 3.3) </strong></span>

<span style="font-family: Segoe UI;font-size: 10pt"><strong>SSL 2.0 </strong>had many security flaws which led to the development of its successor <strong>SSL 3.0</strong>. It is present only for backward compatibility. I have rarely seen anyone using this version and I would highly recommend against it. </span>

<span style="font-family: Segoe UI;font-size: 10pt">As we know TLS/SSL is an application layer protocol. Below is a diagram depicting the TCP/IP model: </span>

<p style="text-align: center">
  <img src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4336.080613_0416_SSLHandshak1.png" alt="" />
</p>

<span style="font-family: Segoe UI;font-size: 10pt">I am not going to discuss the <strong>SSL/TLS</strong> protocol in this post as it is beyond the scope of this topic. However I would be discussing <strong>SSL handshake</strong> in brief and relate it to <strong>IIS</strong>. </span>

<span style="font-family: Segoe UI;font-size: 10pt">The above diagram makes it clear that <strong>TLS/SSL</strong> runs on top of <strong>TCP/IP</strong> like any other application layer protocol. Before we delve into SSL handshake we need to know something about <strong>TCP handshake</strong> too. </span>

<span style="font-family: Segoe UI;font-size: 24pt"><strong>TCP/IP Handshake </strong></span>

<span style="font-family: Segoe UI;font-size: 10pt">Microsoft has published a support article explaining the 3-way <strong>TCP/IP handshake</strong>. Here is the link: <a href="http://support.microsoft.com/kb/172983">http://support.microsoft.com/kb/172983</a> </span>

<span style="font-family: Segoe UI;font-size: 10pt">Below diagram should give you a gist of the TCP/IP handshake: </span>

<p style="text-align: center">
  <img src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/2021.080613_0416_SSLHandshak2.png" alt="" />
</p>

<span style="font-family: Segoe UI;font-size: 10pt">If we were to capture a network trace (or a TCP Dump) and look at the details available and analyze the details available; the <strong>IP Layer</strong> provides the <strong>TCP layer</strong> with <strong>IP Address</strong> of the <strong>client</strong> and <strong>server</strong>. The <strong>TCP layer</strong> contains the details about the <strong>source port</strong> and the <strong>destination port</strong>, <strong>TCP Flags</strong> and other details like <strong>checksum, Windows Size</strong> etc. </span>

<span style="font-family: Segoe UI;font-size: 10pt">When the user launches a browser and punches in the web address, let&#8217;s say <a href="https://www.kaushalz.com">https://www.kaushalz.com</a>, the client and the server would perform the TCP/IP handshake as seen below </span>

<p style="text-align: center">
  <img src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/5518.080613_0416_SSLHandshak3.png" alt="" />
</p>

<span style="font-family: Segoe UI;font-size: 10pt">So basically this is what is passed on from the <strong>TCP/IP layer</strong> to the application layer: </span>

  * <span style="font-family: Segoe UI;font-size: 10pt">IP Address of the source and destination </span>
  * <span style="font-family: Segoe UI;font-size: 10pt">Source Port and Destination Port </span>

<span style="font-family: Segoe UI;font-size: 10pt">The host header is neither present in the IP or the TCP layer. This actually leads to a problem which was addressed via the introduction of <a href="http://en.wikipedia.org/wiki/Server_Name_Indication">SERVER NAME INDICATION</a> (a TLS Extension). </span>

<span style="color: #c00000;font-family: Segoe UI;font-size: 16pt"><strong>Problem due to above Limitation </strong></span>

<span style="font-family: Segoe UI;font-size: 10pt">Before I describe the problem we need to understand a little about the server side bindings. When routing a HTTP request to a website the server determines which process the request to be routed based on the <strong>IP</strong>, <strong>PORT</strong> & the <strong>HOSTNAME</strong>. These 3 are always available to the server during a normal HTTP communication. So basically the combination of <strong>IP+PORT+HOSTNAME</strong> is used as a unique identity to route the site to a specific process. The server admin can have the same <strong>IP+PORT</strong> for all the HTTP websites and alter only the <strong>HOSTNAME</strong> and maintain the uniqueness throughout. Which also makes the server scalable. </span>

<span style="font-family: Segoe UI;font-size: 10pt">However in case of SSL the server has access to <strong>IP</strong> & <strong>Port</strong> only. Since the <strong>HOSTNAME</strong> is not available, the server has to route the request to the process depending on <strong>IP+PORT</strong>. This limitation leaves the server handicapped, as it has to changes the design for websites running on HTTPS. Due to this, the uniqueness for the websites running on HTTPS is determined through combination of <strong>IP+PORT</strong>. In real world, having a separate IP for a website is not ideal due to hardware & monetary limitations. Also changing the port number for all SSL bindings may not be ideal as changing the port number to anything other than the default SSL port would require the client to specifically put out the port number in the request. As a result, the server is not scalable for HTTPS sites. </span>

<span style="font-family: Segoe UI;font-size: 10pt">This was a protocol limitation and severely affected the scalability of the sites </span>

<span style="font-family: Segoe UI;font-size: 10pt">This problem was addressed by introducing a <strong>TLS Extension</strong> called <strong>Server name Indication</strong>. The client sends the server the hostname it is requesting for as a part of the <strong>CLIENT HELLO</strong> in the form of <strong>TLS EXTENSIONS</strong>. You can read more about it here: <a href="http://tools.ietf.org/html/rfc3546"><strong>RFC 3546 (Section 3.1)</strong></a> </span>

<span style="font-family: Segoe UI;font-size: 24pt"><strong>TLS/SSL Handshake </strong></span>

<span style="font-family: Segoe UI;font-size: 10pt">Let&#8217;s consider a scenario where the client launches the browser and punches in <a href="https://www.kaushalz.com">https://www.kaushalz.com</a>. </span>

<ul style="margin-left: 39pt">
  <li>
    <span style="font-family: Segoe UI;font-size: 10pt">Client will try to resolve the hostname to an IPAddress via <strong>DNS</strong>. </span>
  </li>
  <li>
    <span style="font-family: Segoe UI;font-size: 10pt">Once the client has the <strong>Destination IP</strong>, it will send a <strong>TCP SYN</strong> to the server. </span>
  </li>
  <li>
    <span style="font-family: Segoe UI;font-size: 10pt">The Server responds with <strong>ACK</strong> to this <strong>SYN</strong>. </span>
  </li>
  <li>
    <span style="font-family: Segoe UI;font-size: 10pt">The client responds with an <strong>ACK</strong> to the <strong>ACK</strong> it received from the server. Now a TCP connection has been established between the client and the server. The client will now forward the requests to the <strong>Destination IP</strong> on <strong>port 443</strong> (<strong>Default TLS/SSL port</strong>) </span>
  </li>
  <li>
    <span style="font-family: Segoe UI;font-size: 10pt">The control is now transferred to the <strong>SSL Protocol</strong> in the <strong>application layer</strong>. It has the IP & the Port information handy from previous steps. However, it still has no clue whatsoever about the hostname. </span>
  </li>
  <li>
    <div>
      <span style="font-family: Segoe UI;font-size: 10pt">The client creates a TLS Packet called as <strong>CLIENT HELLO</strong>. This contains the following details: </span>
    </div>
    
    <ul>
      <li>
        <span style="font-family: Segoe UI;font-size: 10pt">SSL Protocol version </span>
      </li>
      <li>
        <span style="font-family: Segoe UI;font-size: 10pt">Session ID </span>
      </li>
      <li>
        <span style="font-family: Segoe UI;font-size: 10pt">List of Cipher Suites supported by the client. </span>
      </li>
      <li>
        <span style="font-family: Segoe UI;font-size: 10pt">List of CLIENT HELLO Extensions </span>
      </li>
    </ul>
    
    <p>
      <span style="font-family: Segoe UI;font-size: 10pt">The Client typically selects the most secure protocol version and sends it to the server. Below is a snippet from the <a href="http://tools.ietf.org/html/rfc3546"><strong>RFC 3546</strong></a>: </span></li> </ul> 
      
      <div style="margin-left: 85pt">
        <table style="border-collapse: collapse;background: none repeat scroll 0% 0% #f2f2f2;width: 650px" border="0" align="center">
          <colgroup> <col style="width: 779px" /></colgroup> <tr>
            <td style="padding-left: 9px;padding-right: 9px;border: solid 0.5pt">
              <p style="text-align: justify">
                <span style="font-family: courier new,courier;font-size: small">Blake-Wilson, et. al.            Standards Track                       [Page 4]<br /> RFC 3546                         TLS Extensions                       June 2003</span>
              </p>
              
              <p style="text-align: justify">
                <span style="font-family: courier new,courier;font-size: small"><br /> 2.1. Extended Client Hello</span>
              </p>
              
              <p style="text-align: justify">
                <span style="font-family: courier new,courier;font-size: small"><br /> Clients MAY request extended functionality from servers by sending the extended client hello message format in place of the client hello message format. The extended client hello message format is:</span>
              </p>
              
              <p style="padding-left: 30px">
                <span style="background-color: #ffff00"><span style="font-family: courier new,courier;font-size: small">struct {<br /> </span></span><span style="font-family: courier new,courier;font-size: small"><span style="font-family: courier new,courier;font-size: small">       </span><span style="font-family: courier new,courier;font-size: small;background-color: #ffff00"> ProtocolVersion client_version;</span><br /> </span><span style="font-family: courier new,courier;font-size: small">        </span><span style="background-color: #ffff00"><span style="font-family: courier new,courier;font-size: small">Random random;<br /> </span></span><span style="font-family: courier new,courier;font-size: small">        </span><span style="background-color: #ffff00"><span style="font-family: courier new,courier;font-size: small">SessionID session_id;<br /> </span></span><span style="font-family: courier new,courier;font-size: small">        </span><span style="background-color: #ffff00"><span style="font-family: courier new,courier;font-size: small">CipherSuite cipher_suites<2..2^16-1>;<br /> </span></span><span style="font-family: courier new,courier;font-size: small">        </span><span style="background-color: #ffff00"><span style="font-family: courier new,courier;font-size: small">CompressionMethod compression_methods<1..2^8-1>;<br /> </span></span><span style="font-family: courier new,courier;font-size: small">        </span><span style="background-color: #ffff00"><span style="font-family: courier new,courier;font-size: small">Extension client_hello_extension_list<0..2^16-1>;<br /> } ClientHello;</span></span>
              </p>
              
              <p style="text-align: justify">
                <span style="font-family: courier new,courier;font-size: small">Here the new &#8220;client_hello_extension_list&#8221; field contains a list of extensions. The actual &#8220;Extension&#8221; format is defined in Section 2.3.</span>
              </p>
              
              <p style="text-align: justify">
                <span style="font-family: courier new,courier;font-size: small">In the event that a client requests additional functionality using</span>  <span style="font-family: courier new,courier;font-size: small">the extended client hello, and this functionality is not supplied by the server, the client MAY abort the handshake.</span>
              </p>
              
              <p style="text-align: justify">
                <span style="font-family: courier new,courier;font-size: small">Note that [TLS], Section 7.4.1.2, allows additional information to be added to the client hello message.  Thus the use of the extended client hello defined above should not &#8220;break&#8221; existing TLS 1.0 servers.</span>
              </p>
              
              <p style="text-align: justify">
                 <span style="font-family: courier new,courier;font-size: small">A server that supports the extensions mechanism MUST accept only client hello messages in either the original or extended ClientHello format, and (as for all other messages) MUST check that the amount of data in the message precisely matches one of these formats; if not <span style="font-family: courier new,courier;font-size: small">then it MUST send a fatal &#8220;decode_error&#8221; alert.  This overrides the &#8220;Forward compatibility note&#8221; in [TLS].</span><br /> </span>
              </p>
            </td>
          </tr>
        </table>
      </div>
      
      <p style="margin-left: 39pt;padding-left: 30px">
         <span style="font-family: Segoe UI;font-size: 10pt">If you were to capture a network trace (or a TCP Dump) this is how the <strong>CLIENT HELLO</strong> would look like: </span>
      </p>
      
      <div style="margin-left: 50pt">
        <table style="border-collapse: collapse;width: 800px;height: 1019px" border="0" align="center">
          <colgroup> <col style="width: 865px" /></colgroup> <tr>
            <td style="padding-left: 9px;padding-right: 9px;border: solid 0.5pt">
              <span style="font-family: courier new,courier;font-size: small"><strong>Frame 310</strong>: 187 bytes on wire (1496 bits), 187 bytes captured (1496 bits) on interface 0</span><br /> <span style="font-family: courier new,courier;font-size: small"><strong>Ethernet II</strong>, Src: WistronI_86:74:54 (3c:97:0e:86:74:54), Dst: Cisco_e5:44:00 (10:bd:18:e5:44:00)</span><br /> <span style="font-family: courier new,courier;font-size: small"><strong>Internet Protocol Version 4</strong>, Src: 10.171.71.21 (10.171.71.21), Dst: 10.168.3.213 (10.168.3.213)</span><br /> <span style="font-family: courier new,courier;font-size: small"><strong>Transmission Control Protocol</strong>, Src Port: 42079 (42079), Dst Port: http (80), Seq: 226, Ack: 116, Len: 133</span><br /> <span style="font-family: courier new,courier;font-size: small"><strong>Secure Sockets Layer<br /> </strong>    TLSv1 Record Layer: Handshake Protocol: Client Hello</span><br /> <span style="font-family: courier new,courier;font-size: small">        Content Type: Handshake (22)</span><br /> <span style="font-family: courier new,courier;font-size: small">        Version: TLS 1.0 (0x0301)</span><br /> <span style="font-family: courier new,courier;font-size: small">        Length: 128</span><br /> <span style="font-size: small"><strong><span style="font-family: courier new,courier">       </span></strong><span style="background-color: #ffff00"><strong><span style="font-family: courier new,courier"> Handshake Protocol: Client Hello</span></strong></span></span><br /> <span style="font-family: courier new,courier;font-size: small">            Handshake Type: Client Hello (1)</span><br /> <span style="font-family: courier new,courier;font-size: small">            Length: 124</span><br /> <span style="font-size: small"><strong><span style="font-family: courier new,courier">           </span></strong><span style="background-color: #ffff00"><strong><span style="font-family: courier new,courier"> Version: TLS 1.0 (0x0301)</span></strong></span></span><br /> <span style="font-family: courier new,courier;font-size: small">            <strong>Random<br /> </strong>                gmt_unix_time: Aug  3, 2013 06:45:04.000000000 India Standard Time</span><br /> <span style="font-family: courier new,courier;font-size: small">                random_bytes: 894966609a64a0b0ba0b4cd5adcc431aad77f0ff6108590e&#8230;</span><br /> <span style="font-family: courier new,courier;font-size: small">            Session ID Length: 0</span><br /> <span style="font-family: courier new,courier;font-size: small">            Cipher Suites Length: 24</span><br /> <span style="font-family: courier new,courier;font-size: small"><strong>           <span style="background-color: #ffff00"> Cipher Suites (12 suites)</span><br /> </strong>                Cipher Suite: TLS_RSA_WITH_AES_128_CBC_SHA (0x002f)</span><br /> <span style="font-family: courier new,courier;font-size: small">                Cipher Suite: TLS_RSA_WITH_AES_256_CBC_SHA (0x0035)</span><br /> <span style="font-family: courier new,courier;font-size: small">                Cipher Suite: TLS_RSA_WITH_RC4_128_SHA (0x0005)</span><br /> <span style="font-family: courier new,courier;font-size: small">                Cipher Suite: TLS_RSA_WITH_3DES_EDE_CBC_SHA (0x000a)</span><br /> <span style="font-family: courier new,courier;font-size: small">                Cipher Suite: TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA (0xc013)</span><br /> <span style="font-family: courier new,courier;font-size: small">                Cipher Suite: TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA (0xc014)</span><br /> <span style="font-family: courier new,courier;font-size: small">                Cipher Suite: TLS_ECDHE_ECDSA_WITH_AES_128_CBC_SHA (0xc009)</span><br /> <span style="font-family: courier new,courier;font-size: small">                Cipher Suite: TLS_ECDHE_ECDSA_WITH_AES_256_CBC_SHA (0xc00a)</span><br /> <span style="font-family: courier new,courier;font-size: small">                Cipher Suite: TLS_DHE_DSS_WITH_AES_128_CBC_SHA (0x0032)</span><br /> <span style="font-family: courier new,courier;font-size: small">                Cipher Suite: TLS_DHE_DSS_WITH_AES_256_CBC_SHA (0x0038)</span><br /> <span style="font-family: courier new,courier;font-size: small">                Cipher Suite: TLS_DHE_DSS_WITH_3DES_EDE_CBC_SHA (0x0013)</span><br /> <span style="font-family: courier new,courier;font-size: small">                Cipher Suite: TLS_RSA_WITH_RC4_128_MD5 (0x0004)</span><br /> <span style="font-family: courier new,courier;font-size: small">            <strong>Compression Methods</strong> Length: 1</span><br /> <span style="font-family: courier new,courier;font-size: small">            <strong>Compression Methods</strong> (1 method)</span><br /> <span style="font-family: courier new,courier;font-size: small">            <strong>Extensions</strong> Length: 59</span><br /> <span style="font-family: courier new,courier;font-size: small">            <strong>Extension</strong>: renegotiation_info</span><br /> <span style="font-size: small"><span style="font-family: courier new,courier">           </span><span style="font-family: courier new,courier;background-color: #ffff00"> <strong>Extension</strong>: server_name</span></span><br /> <span style="font-family: courier new,courier;font-size: small">            <strong>Extension</strong>: status_request</span><br /> <span style="font-family: courier new,courier;font-size: small">            <strong>Extension</strong>: elliptic_curves</span><br /> <span style="font-family: courier new,courier;font-size: small">            <strong>Extension</strong>: ec_point_formats</span><br /> <span style="font-family: courier new,courier;font-size: small">            <strong>Extension</strong>: SessionTicket TLS</span>
            </td>
          </tr>
        </table>
      </div>
      
      <p style="margin-left: 39pt">
        <ul style="margin-left: 39pt">
          <li>
            <span style="font-family: Segoe UI;font-size: 10pt">The client sends a <strong>CLIENT HELLO</strong> to the server on the IP & Port it obtained during TCP handshake. </span>
          </li>
          <li>
            <div>
              <span style="font-family: Segoe UI;font-size: 10pt">For this scenario I will consider IIS 7.5 as the <strong>SERVER</strong> entity. Upon receiving the <strong>CLIENT HELLO</strong>, the server has access to the following information: </span>
            </div>
            
            <ul>
              <li>
                <span style="font-family: Segoe UI;font-size: 10pt">IP Address (<strong>10.168.3.213</strong>) </span>
              </li>
              <li>
                <span style="font-family: Segoe UI;font-size: 10pt">Port Number (<strong>443</strong>) </span>
              </li>
              <li>
                <span style="font-family: Segoe UI;font-size: 10pt">Protocol Version (<strong>TLS 1.0</strong>) </span>
              </li>
              <li>
                <span style="font-family: Segoe UI;font-size: 10pt">List of Cipher Suites </span>
              </li>
              <li>
                <span style="font-family: Segoe UI;font-size: 10pt">Session ID </span>
              </li>
              <li>
                <span style="font-family: Segoe UI;font-size: 10pt">List of <strong>CLIENT HELLO</strong> Extensions etc. </span>
              </li>
            </ul>
            
            <p>
              <span style="font-family: Segoe UI;font-size: 10pt">The Server will first check if it supports the above protocol version and if any of the cipher suites in the provided list. If not, the handshake fails there itself. </span>
            </p>
            
            <p>
              <span style="font-family: Segoe UI;font-size: 10pt">The Server will now try to determine if there is an end point listening on the <strong>IP</strong> and <strong>PORT</strong>. If it finds an endpoint and if it is <strong>IIS</strong>, then the <strong>TCPIP.SYS</strong> driver moves the packet to the <strong>HTTP.SYS</strong> layer. </span>
            </p>
            
            <ul>
              <li>
                <span style="font-family: Segoe UI;font-size: 10pt"><strong>HTTP.SYS</strong> moves the request into the generic <strong>SSL Queue</strong>. </span>
              </li>
              <li>
                <span style="font-family: Segoe UI;font-size: 10pt">Until IIS 7.5 the SSL bindings were IP based i.e., IP+ Port and were associated with a certificate hash. </span>
              </li>
              <li>
                <span style="font-size: 10pt"><span style="font-family: Segoe UI">The <strong>HTTP.SYS</strong> tries to determine the certificate has corresponding to this <strong>IP+Port</strong> combination. It does so by enumerating the following registry key: </span><span style="font-family: Courier New"><strong>HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\HTTP\Parameters\SslBindingInfo </strong></span></span>
              </li>
              <li>
                <span style="font-family: Segoe UI;font-size: 10pt">From the above, the certificate hash corresponding to the <strong>IP+PORT</strong> combination is determined. Now the <strong>HTTP.SYS</strong> calls the <strong>CRYPTO API&#8217;s</strong> by passing on the cert hash to retrieve certificate blob, which calls the certificate store, finds the certificate and sends it back to the <strong>HTTP.SYS</strong>. </span>
              </li>
            </ul>
          </li>
          
          <li>
            <span style="font-family: Segoe UI;font-size: 10pt">The Server responds to the client with <strong>SERVER HELLO</strong>. RFC 3546 defines the <a href="http://tools.ietf.org/html/rfc3546">format of the <strong>SERVER HELLO</strong></a>: </span>
          </li>
        </ul>
        
        <div style="margin-left: 85pt">
          <table style="border-collapse: collapse;background: #f2f2f2 none repeat scroll 0% 0%;width: 632px;height: 643px" border="0" align="center">
            <colgroup> <col style="width: 779px" /></colgroup> <tr>
              <td style="padding-left: 9px;padding-right: 9px;border: solid 0.5pt">
                <span style="font-family: courier new,courier;font-size: small">Blake-Wilson, et. al.            Standards Track                       [Page 5]</span><br /> <span style="font-family: courier new,courier;font-size: small">RFC 3546                          TLS Extensions                      June 2003</span></p> 
                
                <p>
                  <span style="font-family: courier new,courier;font-size: small">2.2. Extended Server Hello</span>
                </p>
                
                <p>
                  <span style="font-family: courier new,courier;font-size: small">The extended server hello message format MAY be sent in place of the server hello message when the client has requested extended functionality via the extended client hello message specified in Section 2.1.  The extended server hello message format is:</span>
                </p>
                
                <p>
                  <span style="font-family: courier new,courier;font-size: small">     </span><span style="font-family: courier new,courier;font-size: small;background-color: #ffff00"> struct {</span><br /> <span style="font-family: courier new,courier;font-size: small">         </span><span style="font-family: courier new,courier;font-size: small;background-color: #ffff00"> ProtocolVersion server_version;</span><br /> <span style="font-family: courier new,courier;font-size: small">         </span><span style="font-family: courier new,courier;font-size: small;background-color: #ffff00"> Random random;</span><br /> <span style="font-family: courier new,courier;font-size: small">         </span><span style="font-family: courier new,courier;font-size: small;background-color: #ffff00"> SessionID session_id;</span><br /> <span style="font-family: courier new,courier;font-size: small">         </span><span style="font-family: courier new,courier;font-size: small;background-color: #ffff00"> CipherSuite cipher_suite;</span><br /> <span style="font-family: courier new,courier;font-size: small">         </span><span style="font-family: courier new,courier;font-size: small;background-color: #ffff00"> CompressionMethod compression_method;</span><br /> <span style="font-family: courier new,courier;font-size: small">         </span><span style="font-family: courier new,courier;font-size: small;background-color: #ffff00"> Extension server_hello_extension_list<0..2^16-1>;</span><br /> <span style="font-family: courier new,courier;font-size: small">     </span><span style="font-family: courier new,courier;font-size: small;background-color: #ffff00"> } ServerHello;</span>
                </p>
                
                <p>
                  <span style="font-family: courier new,courier;font-size: small">Here the new &#8220;server_hello_extension_list&#8221; field contains a list of extensions.  The actual &#8220;Extension&#8221; format is defined in Section 2.3.</span>
                </p>
                
                <p>
                  <span style="font-family: courier new,courier;font-size: small"><span style="font-family: courier new,courier;font-size: small">Note that the extended server hello message is only sent in response to an extended client hello message.  This prevents the possibility that the extended server hello message could &#8220;break&#8221; existing TLS 1.0 clients. </span><br /> </span></td> </tr> </tbody> </table> </div> 
                  
                  <p style="margin-left: 39pt;padding-left: 30px">
                    <span style="font-family: Segoe UI;font-size: 10pt">The Server typically responds back with the following details: </span>
                  </p>
                  
                  <ul style="margin-left: 75pt">
                    <li>
                      <span style="font-family: Segoe UI;font-size: 10pt">SSL/TLS Protocol version. </span>
                    </li>
                    <li>
                      <span style="font-family: Segoe UI;font-size: 10pt">One of the cipher suites from the list of cipher suites provided by client. (whichever is the most secure) </span>
                    </li>
                    <li>
                      <span style="font-family: Segoe UI;font-size: 10pt">Certificate of the server (Without the private key of course) </span>
                    </li>
                    <li>
                      <span style="font-family: Segoe UI;font-size: 10pt">List of <strong>SERVER HELLO</strong> Extensions. </span>
                    </li>
                    <li>
                      <span style="font-family: Segoe UI;font-size: 10pt">(<span style="color: #70ad47"><strong>OPTIONAL</strong></span>)If the web app associated with this binding requires a Client Certificate for authentication then it would request the client to send the certificate. Here the IIS Sever would send the client the distinguished names of the list of <strong>TRUSTED ROOT CA</strong> it supports. </span>
                    </li>
                  </ul>
                  
                  <p style="margin-left: 39pt;padding-left: 30px">
                    <span style="font-family: Segoe UI;font-size: 10pt">Below is a snippet of the network trace:<br /> </span>
                  </p>
                  
                  <div style="margin-left: 50pt">
                    <table style="border-collapse: collapse;width: 796px;height: 971px" border="0" align="center">
                      <colgroup> <col style="width: 857px" /></colgroup> <tr>
                        <td style="padding-left: 9px;padding-right: 9px;border: solid 0.5pt">
                          <span style="font-family: courier new,courier;font-size: small"><strong>Frame 320</strong>: 257 bytes on wire (2056 bits), 257 bytes captured (2056 bits) on interface 0</span><br /> <span style="font-family: courier new,courier;font-size: small"><strong>Ethernet II</strong>, Src: Cisco_e5:44:00 (10:bd:18:e5:44:00), Dst: WistronI_86:74:54 (3c:97:0e:86:74:54)</span><br /> <span style="font-family: courier new,courier;font-size: small"><strong>Internet Protocol Version 4</strong>, Src: 10.168.3.213 (10.168.3.213), Dst: 10.171.71.21 (10.171.71.21)</span><br /> <span style="font-family: courier new,courier;font-size: small"><strong>Transmission Control Protocol</strong>, Src Port: http (80), Dst Port: 42079 (42079), Seq: 1576, Ack: 359, Len: 203</span><br /> <span style="font-family: courier new,courier;font-size: small">[2 Reassembled TCP Segments (1663 bytes): #319(1460), #320(203)]</span><br /> <span style="font-family: courier new,courier;font-size: small"><strong>Secure Sockets Layer<br /> </strong>    <strong>TLSv1 Record Layer</strong>: Handshake Protocol: Multiple Handshake Messages</span><br /> <span style="font-family: courier new,courier;font-size: small">        Content Type: Handshake (22)</span><br /> <span style="font-family: courier new,courier;font-size: small">        Version: TLS 1.0 (0x0301)</span><br /> <span style="font-family: courier new,courier;font-size: small">        Length: 1658</span><br /> <span style="font-family: courier new,courier;font-size: small">       <span style="background-color: #ffff00"> <strong>Handshake Protocol</strong>: </span><strong><span style="background-color: #ffff00">Server Hello</span><br /> </strong>            Handshake Type: Server Hello (2)</span><br /> <span style="font-family: courier new,courier;font-size: small">            Length: 81</span><br /> <span style="font-size: small"><span style="font-family: courier new,courier">           </span><span style="font-family: courier new,courier;background-color: #ffff00"> Version: TLS 1.0 (0x0301)</span></span><br /> <span style="font-family: courier new,courier;font-size: small">            Random</span><br /> <span style="font-family: courier new,courier;font-size: small">            Session ID Length: 32</span><br /> <span style="font-family: courier new,courier;font-size: small">            Session ID: 8d0a0000efffe1ad6a82edc6d6a8967bd759cd0f3bdf70e9&#8230;</span><br /> <span style="font-family: courier new,courier;font-size: small">            <strong><span style="background-color: #ffff00">Cipher Suite: TLS_RSA_WITH_RC4_128_SHA (0x0005)</span><br /> </strong>            Compression Method: null (0)</span><br /> <span style="font-family: courier new,courier;font-size: small">            Extensions Length: 9</span><br /> <span style="font-family: courier new,courier;font-size: small">            Extension: renegotiation_info</span><br /> <span style="font-family: courier new,courier;font-size: small">            Extension: server_name</span><br /> <span style="font-size: small"><span style="font-family: courier new,courier">       </span><span style="font-family: courier new,courier;background-color: #ffff00"> <strong>Handshake Protocol</strong>: Certificate</span></span><br /> <span style="font-family: courier new,courier;font-size: small">            Handshake Type: Certificate (11)</span><br /> <span style="font-family: courier new,courier;font-size: small">            Length: 1565</span><br /> <span style="font-family: courier new,courier;font-size: small">            <strong>Certificates Length: 1562<br /> </strong><strong>            Certificates (1562 bytes)<br /> </strong>                Certificate Length: 1559</span><br /> <span style="font-size: small"><span style="font-family: courier new,courier">               </span><span style="font-family: courier new,courier;background-color: #ffff00"> <strong>Certificate</strong> (id-at-commonName=<strong>www.kaushalz.com</strong>,id-at-organizationalUnitName=Azure,id-at-organizationName=Microsoft,id-at-localityName=Bangalore,id-at-stateOrProvinceName=India,id-at-countryName=IN)</span></span><br /> <span style="font-family: courier new,courier;font-size: small">                    signedCertificate</span><br /> <span style="font-family: courier new,courier;font-size: small">                    algorithmIdentifier (shaWithRSAEncryption)</span><br /> <span style="font-family: courier new,courier;font-size: small">                    Padding: 0</span><br /> <span style="font-family: courier new,courier;font-size: small">                    encrypted: bcd1c6d0a5e548eea94749e950d9ed8d7b73a79ac63306f0&#8230;</span><br /> <span style="font-family: courier new,courier;font-size: small">        <strong>Handshake Protocol</strong>: Server Hello Done</span><br /> <span style="font-family: courier new,courier;font-size: small">            Handshake Type: Server Hello Done (14)</span><br /> <span style="font-family: courier new,courier;font-size: small">            Length: 0</span>
                        </td>
                      </tr>
                    </table>
                  </div>
                  
                  <p style="margin-left: 39pt">
                    <ul style="margin-left: 39pt">
                      <li>
                        <span style="font-family: Segoe UI;font-size: 10pt">The Client uses the <strong>SERVER HELLO</strong> to perform <strong>SERVER AUTHENTICATION</strong>. This is described in detail here: <a href="http://support.microsoft.com/kb/257587">http://support.microsoft.com/kb/257587</a>.If the server cannot be authenticated, the user is warned and informed that an encrypted and authenticated connection cannot be established. If the server is successfully authenticated, the client proceeds to the next step. </span>
                      </li>
                    </ul>
                    
                    <div style="margin-left: 150pt">
                      <table style="border-collapse: collapse;background: none repeat scroll 0% 0% #f2f2f2;width: 575px;height: 41px" border="0" align="center">
                        <colgroup> <col style="width: 779px" /></colgroup> <tr>
                          <td style="padding-left: 9px;padding-right: 9px;border: solid 0.5pt" valign="middle">
                            <span style="font-family: Segoe UI;font-size: 10pt"><strong>NOTE</strong>: If you captured a network trace for a SSL Handshake you could see the details until <strong>SERVER HELLO</strong>, after that the encryption begins and nothing would be available and would make sense as the packets are encrypted.</span>
                          </td>
                        </tr>
                      </table>
                    </div>
                    
                    <ul style="margin-left: 39pt">
                      <li>
                        <span style="font-family: Segoe UI;font-size: 10pt">The Client uses the data provided from the server to generate a <strong>pre-master secret</strong> for the session,<strong> <span style="background-color: yellow">encrypts it with the server&#8217;s public key (obtained from the server&#8217;s certificate),</span></strong> and then sends the encrypted pre-master secret to the server. If the server had requested for <strong>CLIENT CERTIFICATE</strong>, then client also signs another piece of data that is unique to this handshake and known by both the client and server. In this case, the client sends both the signed data and the client&#8217;s own certificate to the server along with the encrypted pre-master secret. </span>
                      </li>
                      <li>
                        <span style="font-family: Segoe UI;font-size: 10pt">If the server had requested for client authentication, the server attempts to authenticate the client. If the client cannot be authenticated, the session ends. If the client is successfully authenticated, the server uses its <strong>private key</strong> to decrypt the <strong>pre-master secret</strong>, and then performs a series of steps (which the client also performs, starting from the same pre-master secret) to <span style="background-color: yellow">generate the <strong>master secret</strong></span>. </span>
                      </li>
                      <li>
                        <span style="font-family: Segoe UI;font-size: 10pt">Both <span style="background-color: yellow"><strong>the client and the server use the master secret to generate the session keys, which are symmetric keys</strong></span> used to encrypt and decrypt information exchanged during the SSL session and to verify its integrity (that is, to detect any changes in the data between the time it was sent and the time it is received over the SSL connection). </span>
                      </li>
                      <li>
                        <span style="font-family: Segoe UI;font-size: 10pt">The <strong>CLIENT</strong> & the <strong>SERVER</strong> send each other a message informing that future messages from them will be encrypted with the session key. It then sends a separate (encrypted) message indicating that its portion of the handshake is finished. </span>
                      </li>
                      <li>
                        <span style="font-family: Segoe UI;font-size: 10pt">The SSL Handshake is done. The Client and the Server send each other messages which are encrypted/decrypted using the session keys generated in the previous step. </span>
                      </li>
                      <li>
                        <span style="font-family: Segoe UI;font-size: 10pt">It is now that the Client sends the actual <strong>HTTP Request</strong> packet to the Server in the encrypted form. </span>
                      </li>
                      <li>
                        <span style="font-family: Segoe UI;font-size: 10pt">The Server decrypts the request via the symmetric key and generates a response, encrypts it and sends it back to the client. </span>
                      </li>
                      <li>
                        <span style="font-family: Segoe UI;font-size: 10pt">This continues normally for the entire session of secure communication. However, at any time either the client or the server may renegotiate the connection. In this case the process repeats again. </span>
                      </li>
                    </ul>
                    
                    <p>
                      <span style="font-family: Segoe UI;font-size: 10pt">Below is a diagrammatic representation of the <strong>SSL Handshake</strong>: </span>
                    </p>
                    
                    <p style="text-align: center">
                      <img class="" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/7608.080613_0416_SSLHandshak4.png" alt="" width="1137" height="600" />
                    </p>
                    
                    <p>
                      <span style="font-family: Segoe UI;font-size: 20pt"><strong>Identifying problems during SSL Handshake </strong></span>
                    </p>
                    
                    <p>
                      <span style="font-family: Segoe UI;font-size: 10pt">Eventually, once the handshake completes and the data exchange has been done, either both or one of the entities will eventually close down the connection gracefully. If there was a problem during the SSL Handshake then you there would be an exception raised within the <strong>SSL Layer (SSL ALERT PROTOCOL)</strong>. These exceptions may or may not be fatal i.e. not all exceptions would cause the handshake to fail. </span>
                    </p>
                    
                    <p>
                      <span style="font-family: Segoe UI;font-size: 10pt">As we know there we can see details only until <strong>SERVER HELLO</strong>. Anything beyond this point is not visible. However, in case of a SSL ALERT we would see some notification which can be viewed in the network traces. </span>
                    </p>
                    
                    <p>
                      <span style="font-family: Segoe UI;font-size: 10pt">Servers also tend to propagate this information through some sort of server logging. On <strong>Windows</strong> we have <strong>SCHANNEL</strong> logging which throws a corresponding <strong>SCHANNEL</strong> event in the <strong>SYSTEM</strong> event logs. Watch out for these events. Below is a snippet of one such event: </span>
                    </p>
                    
                    <div style="margin-left: 120pt">
                      <table style="border-collapse: collapse;width: 541px;height: 339px" border="0" align="center">
                        <colgroup> <col style="width: 721px" /></colgroup> <tr style="height: 229px">
                          <td style="padding-left: 9px;padding-right: 9px;border: solid 0.5pt">
                            <span style="font-family: courier new,courier;font-size: small">Log Name:      System<br /> </span><span style="font-family: courier new,courier;font-size: small"><strong><span style="background-color: #ffff00">Source:        Schannel</span><br /> </strong>Date:          05-08-2013 20:16:02</span><br /> <span style="font-family: courier new,courier;font-size: small">Event ID:      36888</span><br /> <span style="font-family: courier new,courier;font-size: small">Task Category: None</span><br /> <span style="font-family: courier new,courier;font-size: small">Level:         Error</span><br /> <span style="font-family: courier new,courier;font-size: small">Keywords:      </span><br /> <span style="font-family: courier new,courier;font-size: small">User:          SYSTEM</span><br /> <span style="font-family: courier new,courier;font-size: small">Computer:      My-Computer</span><br /> <span style="font-family: courier new,courier;font-size: small">Description:</span></p> 
                            
                            <p>
                              <span style="color: #c00000;font-family: Consolas;font-size: 10pt;background-color: #ffff00"><span style="font-family: courier new,courier;font-size: small">The following fatal alert was generated: 40. The internal error state is 1205.</span><strong><br /> </strong></span></td> </tr> </tbody> </table> </div> 
                              
                              <p>
                                &nbsp;
                              </p>
                              
                              <p>
                                <span style="font-family: Segoe UI;font-size: 10pt">However, do remember that not all the alerts that you see are fatal. Try to reproduce the error and confirm that this was the error message that was logged due to the problem you were facing. </span>
                              </p>
                              
                              <p>
                                <span style="font-family: Segoe UI;font-size: 10pt">You could either use <a href="http://www.wireshark.org/download.html"><strong>WireShark</strong></a> or <a href="http://www.microsoft.com/en-us/download/details.aspx?id=4865"><strong>Network Monitor</strong></a><strong> (NETMON)</strong>. I using both depending on what scenario I am running into. </span>
                              </p>
                              
                              <p>
                                <span style="font-family: Segoe UI;font-size: 10pt">That&#8217;s it for now folks, hopefully this would give you some idea on how SSL handshake works. Let me know if you have any queries/suggestions. </span>
                              </p>
                              
                              <p style="text-align: center">
                                <span style="font-family: Segoe UI;font-size: 24pt;text-decoration: underline"><strong>MORE INFORMATION </strong></span>
                              </p>
                              
                              <p>
                                <span style="font-family: Segoe UI;font-size: 10pt"><strong>TCP/IP Handshake</strong>: <a href="http://support.microsoft.com/kb/172983">http://support.microsoft.com/kb/172983</a> </span>
                              </p>
                              
                              <p>
                                <span style="font-family: Segoe UI;font-size: 10pt"><strong>Description of SSL Handshake</strong>: <a href="http://support.microsoft.com/kb/257591">http://support.microsoft.com/kb/257591</a> </span>
                              </p>
                              
                              <p>
                                <span style="font-family: Segoe UI;font-size: 10pt"><strong>Description of Server Authentication during SSL Handshake</strong>: <a href="http://support.microsoft.com/kb/257587">http://support.microsoft.com/kb/257587</a> </span>
                              </p>
                              
                              <p>
                                <span style="font-family: Segoe UI;font-size: 10pt"><strong>SSL/TLS Alert protocol & the alert codes</strong>: <a href="http://blogs.msdn.com/b/kaushal/archive/2012/10/06/ssl-tls-alert-protocol-amp-the-alert-codes.aspx">http://blogs.msdn.com/b/kaushal/archive/2012/10/06/ssl-tls-alert-protocol-amp-the-alert-codes.aspx</a> </span>
                              </p>
                              
                              <p>
                                <span style="font-family: Segoe UI;font-size: 10pt"><strong>Server Name Indication</strong>: <a href="http://en.wikipedia.org/wiki/Server_Name_Indication">http://en.wikipedia.org/wiki/Server_Name_Indication</a> </span>
                              </p>