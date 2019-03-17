---
id: 1875
title: Client Certificate Authentication (Part 2)
date: 2017-06-09T21:49:59+00:00
author: kaushal
layout: post
guid: https://blogs.msdn.microsoft.com/kaushal/?p=1875
permalink: /2017/06/09/client-certificate-authentication-part-2/
opengraph_tags:
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Client Certificate Authentication (Part 2)" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/?p=1875" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="table { font-family: arial, sans-serif; border-collapse: collapse; background-color:#f0ffff } td, th { border: 1px solid #dddddd; text-align: left; } tr:nth-child(even) { background-color: #dddddd; } This is a continuation of my earlier post on Client Certificate Authentication (Part 1) aka TLS Mutual Authentication. Earlier, I had discussed on what Client Certificates are and how they work..." />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Client Certificate Authentication (Part 2)" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/?p=1875" />
    <meta name="twitter:description" content="table { font-family: arial, sans-serif; border-collapse: collapse; background-color:#f0ffff } td, th { border: 1px solid #dddddd; text-align: left; } tr:nth-child(even) { background-color: #dddddd; } This is a continuation of my earlier post on Client Certificate Authentication (Part 1) aka TLS Mutual Authentication. Earlier, I had discussed on what Client Certificates are and how they work..." />
    
categories:
  - "13"
  - Certificate Request
  - certificate_request
  - client certificate
  - cURL
  - openssl
  - pem
  - pfx
  - Secure Renegotiation
  - Server Hello
  - ssl
  - ssl.handshake.type
  - tls
  - tls mutual auth
  - TLS Mutual Authentication
  - Wireshark
---
<span style="font-size: small">This is a continuation of my earlier post on </span>[<span style="font-size: small">Client Certificate Authentication (Part 1)</span>](https://blogs.msdn.microsoft.com/kaushal/2015/05/27/client-certificate-authentication-part-1/) <span style="font-size: small">aka <strong>TLS </strong>Mutual Authentication. Earlier, I had discussed on what Client Certificates are and how they work in <strong>SSL/TLS </strong>Handshake. </span>

<span style="font-size: small">In this post, I will explain how to review <strong>SSL/TLS handshake </strong>with help of tools like <strong><a href="https://www.wireshark.org/download.html">WireShark</a> </strong>& <strong><a href="https://curl.haxx.se/dlwiz/?type=bin&os=Win64&flav=-&ver=*&cpu=x86_64">Curl</a></strong>. </span>

<span style="font-size: small">Before proceeding further, lets review the <strong>SERVER HELLO</strong> definition in </span>[<span style="font-size: small">RFC 5246</span>](https://tools.ietf.org/html/rfc5246#section-7.4)<span style="font-size: small">.  As per the RFC, the server will request the certificate from the client in the Server hello by including <strong>certificate_request</strong> message, which has the decimal code of <strong>13 (0d </strong>in Hex<strong>)</strong>. This will help us in determining the <strong>Certificate Request </strong>in <strong>Server Hello</strong>.</span>

<table style="background-color: #e5e4e2" cellspacing="0" cellpadding="0" width="500" border="0">
  <tr>
    <td>
      <pre style="background-color: #e5e4e2;font-size: 13px">enum { 
    hello_request(0), 
    client_hello(1), 
    server_hello(2), 
    certificate(11), 
    server_key_exchange (12), 
    certificate_request(13), 
    server_hello_done(14), 
    certificate_verify(15), 
    client_key_exchange(16), 
    finished(20), 
    (255) 
} HandshakeType; 
struct { 
    HandshakeType msg_type;    /* handshake type */ 
    uint24 length;             /* bytes in message */ 
    select (HandshakeType) { 
        case hello_request:       HelloRequest; 
        case client_hello:        ClientHello; 
        case server_hello:        ServerHello; 
        case certificate:         Certificate; 
        case server_key_exchange: ServerKeyExchange; 
        case certificate_request: CertificateRequest;
        case server_hello_done:   ServerHelloDone; 
        case certificate_verify:  CertificateVerify; 
        case client_key_exchange: ClientKeyExchange; 
        case finished:            Finished; 
    } body; 
} Handshake;
</pre>
    </td>
  </tr>
</table>

<span style="font-size: small">Once the client sees the <strong>certificate_request </strong>message it will provide the certificate to the server. </span>

### <u><span style="font-weight: bold">Real world example:</span></u>

<span style="font-size: small"><strong>Setup</strong>: Hosted a site on IIS inside an <strong>Azure VM. </strong>This requires a <strong>client certificate </strong>for authentication. Here is the endpoint <a href="https://azurevm.kaushal.co.in">https://azurevm.kaushal.co.in</a> </span>

<span style="font-size: small">I have added the SSL binding via <strong>netsh </strong>using the following command:</span>

> <table style="color: #ffffff;background-color: #2b1b17" cellspacing="0" cellpadding="0" width="800" border="0">
>   <tr>
>     <td width="798">
>       <span style="font-size: small"><span style="font-family: Consolas"><b>netsh</b> http add sslcert <b>ipport</b>=0.0.0.0:443 <b>certhash</b>=<certificate thumbprint goes here> <b>appid</b>={4dc3e181-e14b-4a21-b022-59fc669b0914} <b>certstorename</b>=My <strong>clientcertnegotiation=enable</strong></span></span>
>     </td>
>   </tr>
> </table>
> 
> <span style="font-size: small"></span>

#### <span style="font-size: large"><u><span style="font-weight: bold">Analyzing the TLS/SSL handshake in WireShark</span></u></span>

<span style="font-size: small">As shown below, the server has sent a <strong>certificate request </strong>message to the client and the client has then responded with the certificate in the next communication.</span>

> [<img title="image" style="padding-top: 0px;padding-left: 0px;padding-right: 0px;border-width: 0px" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/2017/06/image_thumb243.png" width="1385" height="549" />](https://msdnshared.blob.core.windows.net/media/2017/06/image259.png)

<span style="font-size: small"><span style="font-family: 'Segoe UI'">In WireShark you can set the filter to “<strong>ssl.handshake.type == 13</strong>” to specifically look for <strong>certificate_request </strong>message in <strong>Server Hello</strong></span>. </span>

> [<img title="image" style="padding-top: 0px;padding-left: 0px;padding-right: 0px;border-width: 0px" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/2017/06/image_thumb244.png" width="1271" height="96" />](https://msdnshared.blob.core.windows.net/media/2017/06/image260.png)

> <table style="background-color: #e5e4e2" cellspacing="0" cellpadding="0" width="819" border="2">
>   <tr>
>     <td valign="top" width="815">
>       <span style="font-size: small"><strong>NOTE:</strong> <span style="font-size: small"><span style="font-family: 'Segoe UI'">Some SSL/TLS servers support only <strong>Secure negotiation</strong>. Therefore you may not see the <strong><span style="background-color: #a5a5a5;color: #333333;font-family: Consolas">Certificate Request</span></strong> message explicitly in the <strong>Server Hello</strong>. In this case, the server will send the <span style="font-family: 'Segoe UI'"><strong>Certificate Request</strong> message as a part of the <span style="background-color: #a5a5a5;color: #000000;font-family: Consolas">Encrypted Handshake Message</span></span></span>.</span></span>
>     </td>
>   </tr>
> </table>

<u><span style="font-size: large"><strong>Analyzing the TLS/SSL handshake in cURL</strong></span></u>

<span style="font-size: small">By far, <strong>cURL </strong>has made it easier to determine if the server is sending the <strong>Certificate Request </strong>in Server Hello. You will have to download the version of curl that includes support SSL Protocol. This works in scenarios where the server supports only <strong>Secure Negotiation</strong>. I</span>

<span style="font-size: small">You can find various builds of <strong>cURL </strong>available for download here: <a href="https://curl.haxx.se/dlwiz/?type=bin&os=Win64&flav=-&ver=*&cpu=x86_64" title="https://curl.haxx.se/dlwiz/?type=bin&os=Win64&flav=-&ver=*&cpu=x86_64">https://curl.haxx.se/dlwiz/?type=bin&os=Win64&flav=-&ver=*&cpu=x86_64</a><a href="http://www.confusedbycode.com/curl/#downloads" title="http://www.confusedbycode.com/curl/#downloads"> </a></span>

<span style="font-size: small">I am using the following</span>

<span style="font-size: small"><strong>curl version</strong>: <strong>7.54.0 &#8211; SSL enabled SSH enabled</strong><br /> <strong>URL</strong>: </span>[<span style="font-size: small">https://bintray.com/artifact/download/vszakats/generic/curl-7.54.0-win64-mingw.7z</span>](https://bintray.com/artifact/download/vszakats/generic/curl-7.54.0-win64-mingw.7z "https://bintray.com/artifact/download/vszakats/generic/curl-7.54.0-win64-mingw.7z")<span style="font-size: small"> </span>

<span style="font-size: small">Execute the following from command prompt</span>

> <table style="background-color: #e5e4e2" cellspacing="0" cellpadding="0" width="618" border="2">
>   <tr>
>     <td valign="top" width="614">
>       <span style="background-color: #cccccc;color: #000000;font-family: 'Courier New';font-size: small"></span><span style="font-family: 'Courier New';font-size: small">curl –v https://<hostname> –k –cert clientcert.pem:<password></span>
>     </td>
>   </tr>
>   
>   <tr>
>     <td valign="top" width="614">
>       <span style="font-size: small"><strong><span style="color: #000000;font-family: 'Courier New';font-size: small">Where,<br /> </span><span style="font-size: small"><strong><span style="color: #000000;font-family: 'Courier New';font-size: small">     -v, &#8211;verbose       Make the operation more talkative<br /> </span></strong></span><span style="font-size: small"><strong><span style="font-size: small"><strong><span style="color: #000000;font-family: 'Courier New';font-size: small">     </span></strong></span></strong></span><span style="color: #000000;font-family: 'Courier New';font-size: small">-k, &#8211;insecure      Allow connections to SSL sites without certs (H)<br /> -E, &#8211;cert CERT[:PASSWD] Client certificate file and password (SSL)</span></strong></span>
>     </td>
>   </tr>
> </table>

<span style="font-size: small">Once the request has been issued via <strong>cURL</strong>. In the verbose output, search for TLS handshake message “<span style="background-color: #cccccc;font-family: 'Courier New'"><strong>Request CERT (13)</strong></span>” as highlighted in the below example.</span>

<table style="background-color: #2b1b17" border="2" width="600" cellspacing="0" cellpadding="0">
  <tr>
    <td valign="top" width="796">
      <pre style="background-color: #2b1b17;color: white;font-size: 13px">C:\&gt;curl -v https://azurevm.kaushal.co.in -k --cert ClientCert.pem:Password
* Rebuilt URL to: https://azurevm.kaushal.co.in/
* Adding handle: conn: 0x34a6540
* Adding handle: send: 0
* Adding handle: recv: 0
* Curl_addHandleToPipeline: length: 1
* - Conn 0 (0x34a6540) send_pipe: 1, recv_pipe: 0
* About to connect() to azurevm.kaushal.co.in port 443 (#0)
*   Trying 13.71.126.36...
* Connected to azurevm.kaushal.co.in (13.71.126.36) port 443 (#0)
* SSLv3, TLS handshake, Client hello (1):
* SSLv3, TLS handshake, Server hello (2):
* SSLv3, TLS handshake, CERT (11):
* SSLv3, TLS handshake, Request CERT (13):
* SSLv3, TLS handshake, Server finished (14):
* SSLv3, TLS handshake, CERT (11):
* SSLv3, TLS handshake, Client key exchange (16):
* SSLv3, TLS handshake, CERT verify (15):
* SSLv3, TLS change cipher, Client hello (1):
* SSLv3, TLS handshake, Finished (20):
* SSLv3, TLS change cipher, Client hello (1):
* SSLv3, TLS handshake, Finished (20):
* SSL connection using AES256-SHA
* Server certificate:
*        subject: OU=Domain Control Validated; CN=*.kaushal.co.in
*        start date: 2017-05-10 09:05:00 GMT
*        expire date: 2018-05-10 09:05:00 GMT
*        issuer: C=US; ST=Arizona; L=Scottsdale; O=GoDaddy.com, Inc.; OU=http://certs.godaddy.com/repository/; CN=Go Daddy Secure Certificate Authority - G2
*        SSL certificate verify result: unable to get local issuer certificate (20), continuing anyway.
&gt; GET / HTTP/1.1
&gt; User-Agent: curl/7.33.0
&gt; Host: azurevm.kaushal.co.in
&gt; Accept: */*
&gt;
&lt; HTTP/1.1 200 OK
&lt; Cache-Control: private
&lt; Content-Type: text/html; charset=utf-8 * Server Microsoft-IIS/8.5 is not blacklisted
&lt; Server: Microsoft-IIS/8.5 &lt; X-AspNetMvc-Version: 5.2
&lt; X-AspNet-Version: 4.0.30319
&lt; X-Powered-By: ASP.NET
&lt; Date: Fri, 09 Jun 2017 16:51:13 GMT
&lt; Content-Length: 5767
. . .</pre>
    </td>
  </tr>
</table>

<span style="font-size: small"><br /> On Windows, in order to pass the client certificate via <strong>cURL</strong>, you will have to extract the<strong> .pem</strong> file out of the<strong> .pfx</strong>. Use the following </span><span style="font-size: small">command:</span>

<table style="background-color: #2b1b17" border="2" width="600" cellspacing="0" cellpadding="0">
  <tr>
    <td valign="top" width="796">
      <pre style="background-color: #2b1b17;color: white;font-size: 13px">openssl pkcs12 -in clientcertificate.pfx -out clientcertificate.pem –clcerts
Enter Import Password:
MAC verified OK
Enter PEM pass phrase:
Verifying - Enter PEM pass phrase:</pre>
    </td>
  </tr>
</table>

<span style="font-size: small">HTH,</span>

<span style="font-size: small">Kaushal</span>

<span style="font-size: small"></span>