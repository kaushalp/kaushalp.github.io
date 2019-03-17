---
id: 1936
title: 'Azure App Service: Understanding TLS Mutual Authentication with Web App'
date: 2017-06-12T14:22:51+00:00
author: kaushal
layout: post
guid: https://blogs.msdn.microsoft.com/kaushal/?p=1936
permalink: /2017/06/12/azure-app-service-understanding-tls-mutual-authentication-with-web-app/
opengraph_tags:
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Azure App Service: Understand TLS Mutual Authentication" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/?p=1936" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="I have published 2 posts in the past on Client Certificate authentication. Client Certificate Authentication (Part 1) Client Certificate Authentication (Part 2) In order to enable Client Certificate authentication on azure web app, we need to flip the clientCertEnabled property to true. Please refer the following article on how to enable TLS mutual auth for..." />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Azure App Service: Understand TLS Mutual Authentication" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/?p=1936" />
    <meta name="twitter:description" content="I have published 2 posts in the past on Client Certificate authentication. Client Certificate Authentication (Part 1) Client Certificate Authentication (Part 2) In order to enable Client Certificate authentication on azure web app, we need to flip the clientCertEnabled property to true. Please refer the following article on how to enable TLS mutual auth for..." />

categories:
  - --cacert
  - "13"
  - Authentication
  - Azure
  - Azure App Service
  - Azure Web App
  - certificate_request
  - client certificate
  - cURL
  - encrypted handshake message
  - IIS
  - request cert
  - Secure Renegotiation
  - Server Hello
  - ssl
  - ssl.handshake.type
  - tls
  - tls mutual auth
  - TLS Mutual Authentication
  - Wireshark
---
I have published 2 posts in the past on Client Certificate authentication.

  * [Client Certificate Authentication (Part 1)](https://kaushalp.github.io/2015/05/27/client-certificate-authentication-part-1/)
  * [Client Certificate Authentication (Part 2)](https://kaushalp.github.io/2017/06/09/client-certificate-authentication-part-2/)

  In order to enable **Client Certificate** authentication on azure web app, we need to flip the **``clientCertEnabled``** property to **``true``**. Please refer the following article on how to enable TLS mutual auth for an Azure Web App:
  [How To Configure TLS Mutual Authentication for Web App](https://docs.microsoft.com/en-us/azure/app-service-web/app-service-web-configure-tls-mutual-auth)

## HOW IT WORKS

The best way to understand this is to capture a network trace by issuing a **HTTPS** request to the **Azure Web App**. You will notice that the **certificate request** is not part of the **Server Hello**. This is because the server supports **Secure Renegotiation**. The **Certificate Request** will be sent as a part of the **Encrypted Handshake Message** to the client. Refer my earlier post [here](https://kaushalp.github.io/2017/06/09/client-certificate-authentication-part-2/)
To demonstrate this, I have enabled client certificate Authentication on one of the staging slots of my web app. Here is the link: https://clientcertauth-demo.azurewebsites.net

I have written a sample code, which accepts any certificate that is provided to it. It reads the client certificate and displays the results in a tabular format. I browsed this web app and captured a network trace using WireShark. Here is a screenshot of this trace:

![SSL Handhshake - Secure Renegotiation](https://kaushalp.github.io/wp-content/uploads/2017/06/image272.png)

So, how do we confirm if the server is requesting for client certificate. You can use one of the following methods:

### Enable SSL traffic decryption in WireShark.
I found a blog post on how to do this and tested it myself. Here is the link: https://jimshaver.net/2015/02/11/decrypting-tls-browser-traffic-with-wireshark-the-easy-way/
Here is a screenshot of the Decrypted message: The server is sending another Server Hello which contains the **Certificate Request** message.

![SSL Handhshake - Decrypted](https://kaushalp.github.io/wp-content/uploads/2017/06/image273.png)

### Using cURL.exe
You can refer to my previous post on client certificate: [Client Certificate Authentication (Part 2)](https://kaushalp.github.io/2017/06/09/client-certificate-authentication-part-2/) to use curl. **cURL** is a built-in tool on **Azure App Service** instances. Path is: **``D:\Program Files (x86)\Git\usr\bin``**. This means you can run cURL inside the command prompt window in the Kudu console.
* Open the following URL in a browser: https://WebAppName.scm.azurewebsites.net/DebugConsole (replace **WebAppName** with the name of the web app)
* Execute the following command: **``curl -v https://www.kaushal.co.in``**
* Review the verbose output and search for **``Request CERT (13)``**.
* Following is a brief output of the command from the Kudu console of the web app. The Server is requesting for the client certificate in the second **Server Hello** message. See the text highlighted in **yellow**.
<span style="font-size: small">

  ```shell_session
   D:\home>curl -v https://clientcertauth-demo.azurewebsites.net

   * STATE: INIT => CONNECT handle 0x80073200; line 1103 (connection #-5000)
  * Rebuilt URL to: https://clientcertauth-demo.azurewebsites.net/
  * Added connection 0. The cache now contains 1 members
  *   Trying 111.221.95.27…
  * STATE: CONNECT => WAITCONNECT handle 0x80073200; line 1156 (connection #0)
    % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                   Dload  Upload   Total   Spent    Left  Speed
    0     0    0     0    0     0      0      0 –:–:– –:–:– –:–:–     0* Connected to clientcertauth-demo.azurewebsites.net (111.221.95.27) port 443 (#0)
  * STATE: WAITCONNECT => SENDPROTOCONNECT handle 0x80073200; line 1253 (connection #0)
  * ALPN, offering http/1.1
  * Cipher selection: ALL:!EXPORT:!EXPORT40:!EXPORT56:!aNULL:!LOW:!RC4:@STRENGTH
  * successfully set certificate verify locations:
  *   CAfile: /usr/ssl/certs/ca-bundle.crt
    CApath: none
  * TLSv1.2 (OUT), TLS header, Certificate Status (22):
  } [5 bytes data]
  * TLSv1.2 (OUT), TLS handshake, Client hello (1):
  } [512 bytes data]
  * STATE: SENDPROTOCONNECT => PROTOCONNECT handle 0x80073200; line 1267 (connection #0)
  ï»¿<!DOCTYPE html>
  <html>

  <————————–Trimmed HTML Response ————————–>

  </html>
  { [5 bytes data]
  * TLSv1.2 (IN), TLS handshake, Server hello (2):
  { [81 bytes data]
  * TLSv1.2 (IN), TLS handshake, Certificate (11):
  { [3245 bytes data]
  * TLSv1.2 (IN), TLS handshake, Server key exchange (12):
  { [333 bytes data]
  * TLSv1.2 (IN), TLS handshake, Server finished (14):
  { [4 bytes data]
  * TLSv1.2 (OUT), TLS handshake, Client key exchange (16):
  } [70 bytes data]
  * TLSv1.2 (OUT), TLS change cipher, Client hello (1):
  } [1 bytes data]
  * TLSv1.2 (OUT), TLS handshake, Finished (20):
  } [16 bytes data]
  * TLSv1.2 (IN), TLS change cipher, Client hello (1):
  { [1 bytes data]
  * TLSv1.2 (IN), TLS handshake, Finished (20):
  { [16 bytes data]
  * SSL connection using TLSv1.2 / ECDHE-RSA-AES256-SHA384
  * ALPN, server did not agree to a protocol
  * Server certificate:
  *      subject: CN=*.azurewebsites.net
  *      start date: Sep 28 21:45:23 2016 GMT
  *      expire date: May  7 17:03:30 2018 GMT
  *      subjectAltName: clientcertauth-demo.azurewebsites.net matched
  *      issuer: C=US; ST=Washington; L=Redmond; O=Microsoft Corporation; OU=Microsoft IT; CN=Microsoft IT SSL SHA2
  *      SSL certificate verify ok.
  * STATE: PROTOCONNECT => DO handle 0x80073200; line 1288 (connection #0)
  } [5 bytes data]
  > GET / HTTP/1.1
  > Host: clientcertauth-demo.azurewebsites.net
  > User-Agent: curl/7.47.1
  > Accept: */*
  >
  * STATE: DO => DO_DONE handle 0x80073200; line 1350 (connection #0)
  * STATE: DO_DONE => WAITPERFORM handle 0x80073200; line 1477 (connection #0)
  * STATE: WAITPERFORM => PERFORM handle 0x80073200; line 1487 (connection #0)
  { [5 bytes data]
  * TLSv1.2 (IN), TLS handshake, Hello request (0):
  { [4 bytes data]
  * TLSv1.2 (OUT), TLS handshake, Client hello (1):
  } [512 bytes data]
  * TLSv1.2 (IN), TLS handshake, Server hello (2):
  { [105 bytes data]
  * TLSv1.2 (IN), TLS handshake, Certificate (11):
  { [3245 bytes data]
  * TLSv1.2 (IN), TLS handshake, Server key exchange (12):
  { [333 bytes data]
  * TLSv1.2 (IN), TLS handshake, Request CERT (13):
  { [30 bytes data]
  * TLSv1.2 (IN), TLS handshake, Server finished (14):
  { [4 bytes data]
  * TLSv1.2 (OUT), TLS handshake, Certificate (11):
  } [7 bytes data]
  * TLSv1.2 (OUT), TLS handshake, Client key exchange (16):
  } [70 bytes data]
  * TLSv1.2 (OUT), TLS change cipher, Client hello (1):
  } [1 bytes data]
  * TLSv1.2 (OUT), TLS handshake, Finished (20):
  } [16 bytes data]
  * TLSv1.2 (IN), TLS change cipher, Client hello (1):
  { [1 bytes data]
  * TLSv1.2 (IN), TLS handshake, Finished (20):
  { [16 bytes data]
  * HTTP 1.1 or later with persistent connection, pipelining supported
  < HTTP/1.1 403 Forbidden
  < Content-Type: text/html
  * Server Microsoft-IIS/8.0 is not blacklisted
  < Server: Microsoft-IIS/8.0
  < Date: Fri, 09 Jun 2017 19:19:37 GMT
  < Connection: close
  < Content-Length: 2399

  <————————–Trimmed ————————–>
  ```

  Hope this clarifies few doubts on how TLS Mutual Auth works on Azure App Service.

## RESTRICTIONS
* Currently, TLS Mutual Authentication is supported for web apps running in **Basic** or higher pricing tiers only. You will receive the following error if you try to enable it for a web app running in **FREE/SHARED** tier.

  ``Cannot enable client certificate for a site '{0}' because current site mode does not allow it``

* when the **``clientCertEnabled``** property is set to **``true``** the web app mandates the client to provide a client certificate. If the client fails to provide a client certificate they will receive a **403** error. Those familiar with **IIS**, this is equivalent to setting the **``sslFlags``** property (inside ``<access>`` tags) in IIS to include "**``SslRequireCert``**".

  ```xml
  <location path="Kaushal">
    <system.webServer>
        <security>
          <access sslFlags="Ssl, SslNegotiateCert, SslRequireCert" />
        </security>
      </system.webServer>
  </location>
  ```

* As of now, **Azure App Service** supports **Secure Renegotiation** and doesn’t entertain **ReNego**. If there are TLS clients, that are not compliant as per the [RFC 5746](https://tools.ietf.org/html/rfc5746#section-3.7) and depend on Re-Negotiation, then they cannot connect to **Azure App Service**.
