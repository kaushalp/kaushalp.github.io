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
<font size="2">I have published 2 posts in the past on Client Certificate authentication. </font>

  * [<font size="2">Client Certificate Authentication (Part 1)</font>](https://blogs.msdn.microsoft.com/kaushal/2015/05/27/client-certificate-authentication-part-1/ "https://blogs.msdn.microsoft.com/kaushal/2015/05/27/client-certificate-authentication-part-1/") 
      * [<font size="2">Client Certificate Authentication (Part 2)</font>](https://blogs.msdn.microsoft.com/kaushal/2017/06/09/client-certificate-authentication-part-2/ "https://blogs.msdn.microsoft.com/kaushal/2017/06/09/client-certificate-authentication-part-2/") 
        In order to enable **Client Certificate** authentication on azure web app, we need to flip the `clientCertEnabled` property to `true`. Please refer the following article on how to enable TLS mutual auth for an Azure Web App:
        
        [How To Configure TLS Mutual Authentication for Web App](https://docs.microsoft.com/en-us/azure/app-service-web/app-service-web-configure-tls-mutual-auth "https://docs.microsoft.com/en-us/azure/app-service-web/app-service-web-configure-tls-mutual-auth")&nbsp;
        
        ## <font size="5" face="Segoe UI"><u>HOW IT WORKS</u></font>
        
        <font size="2">The best way to understand this is to capture a network trace by issuing a <strong><font style="background-color: #333333" color="#00ff00">HTTPS</font></strong> request to the <strong>Azure Web app</strong>. You will notice that the <strong>certificate request</strong> is not part of the <strong>Server Hello</strong>. This is because the server supports <strong>Secure Renegotiation</strong> and it tends to send this as a part of the <strong>Encrypted Handshake Message</strong> to the client. Refer my earlier post </font>[<font size="2">here</font>](https://blogs.msdn.microsoft.com/kaushal/2017/06/09/client-certificate-authentication-part-2/ "https://blogs.msdn.microsoft.com/kaushal/2017/06/09/client-certificate-authentication-part-2/")<font size="2">. <br />To demonstrate this, I have enabled client certificate Authentication on one of the staging slots of my web app. Here is the link: </font>[<font size="2">https://clientcertauth-demo.azurewebsites.net</font>](https://clientcertauth-demo.azurewebsites.net)  
        <font size="2">I have written a sample code, which accepts any certificate that is provided to it. It reads the client certificate and displays the results in a tabular format.<br />I browsed this web app and captured a network trace using WireShark. Here is a screenshot of this trace:</font>
        
        > [<img title="image" style="border-left-width: 0px;border-right-width: 0px;border-bottom-width: 0px;padding-top: 0px;padding-left: 0px;padding-right: 0px;border-top-width: 0px" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/2017/06/image_thumb255.png" width="1304" height="216" />](https://msdnshared.blob.core.windows.net/media/2017/06/image272.png)
    
    <font size="2">So, how do we confirm if the server is requesting for client certificate. You can use one of the following methods:</font>
    
      1. <font size="2"><strong>Enable SSL traffic decryption in WireShark.</strong> <br />I found a blog post on how to do this and tested it myself. Here is the link: <a title="https://jimshaver.net/2015/02/11/decrypting-tls-browser-traffic-with-wireshark-the-easy-way/" href="https://jimshaver.net/2015/02/11/decrypting-tls-browser-traffic-with-wireshark-the-easy-way/">https://jimshaver.net/2015/02/11/decrypting-tls-browser-traffic-with-wireshark-the-easy-way/</a>&nbsp;<br />Here is a screenshot of the Decrypted message: The server is sending another Server Hello which contains the <strong>Certificate Request </strong>message.<br /><a href="https://msdnshared.blob.core.windows.net/media/2017/06/image273.png"><img title="image" style="border-left-width: 0px;border-right-width: 0px;border-bottom-width: 0px;padding-top: 0px;padding-left: 0px;padding-right: 0px;border-top-width: 0px" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/2017/06/image_thumb256.png" width="1585" height="451" /></a><br /></font> 
          * <font size="2"><strong>Using cURL.exe</strong> <br />You can refer to my previous post on client cert <a title="https://blogs.msdn.microsoft.com/kaushal/2017/06/09/client-certificate-authentication-part-2/" href="https://blogs.msdn.microsoft.com/kaushal/2017/06/09/client-certificate-authentication-part-2/">here</a> to use curl. FYI, <strong>cURL</strong> is included by default on all the Azure App Service instances. Path is <font style="background-color: #cccccc" color="#c0504d" face="Courier New">D:\Program Files (x86)\Git\usr\bin</font>. This means you can do run cURL inside the command prompt window in the Kudu console. </font> 
              * <font size="2">Open the following URL in a browser: <a href="https://<sitename>.scm.azurewebsites.net/DebugConsole">https://<sitename>.<font style="background-color: #ffff00">scm.</font>azurewebsites.net/DebugConsole</a> (replace <strong><sitename></strong> with the name of the web app)</font> 
                  * <font size="2">Execute the following command:<br /><font style="background-color: #000000" color="#ffffff" face="Courier New">curl -v https://<hostname></font></font> 
                      * <font size="2" face="Courier New"></font><font size="2">Review the verbose output and search for “<strong>Request CERT (13)</strong>”. </font> 
                          * <font size="2">Following is a brief output of the command from the Kudu console of the web app. The Server is requesting for the client certificate in the second <strong>Server Hello </strong>message. See the text highlighted in <strong>yellow</strong>.<br /> 
                            
                            <blockquote>
                              <table style="color: #ffffff;background-color: #000000" cellspacing="0" cellpadding="0" width="750" border="2">
                                <tr>
                                  <td valign="top" width="746">
                                    <font size="2"></font> </p> 
                                    
                                    <p>
                                      <font style="background-color: #ffff00" color="#0000ff" size="2" face="Courier New">D:\home>curl -v </font><a href="https://clientcertauth-demo.azurewebsites.net"><font style="background-color: #ffff00" size="2" face="Courier New">https://clientcertauth-demo.azurewebsites.net</font></a><br /><font size="2" face="Courier New">* STATE: INIT => CONNECT handle 0x80073200; line 1103 (connection #-5000) <br />* Rebuilt URL to: </font><a href="https://clientcertauth-demo.azurewebsites.net/"><font size="2" face="Courier New">https://clientcertauth-demo.azurewebsites.net/</font></a><br /><font face="Courier New"><font size="2">* Added connection 0. The cache now contains 1 members<br />*&nbsp;&nbsp; Trying 111.221.95.27&#8230;<br />* STATE: CONNECT => WAITCONNECT handle 0x80073200; line 1156 (connection #0) <br />&nbsp; % Total&nbsp;&nbsp;&nbsp; % Received % Xferd&nbsp; Average Speed&nbsp;&nbsp; Time&nbsp;&nbsp;&nbsp; Time&nbsp;&nbsp;&nbsp;&nbsp; Time&nbsp; Current<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Dload&nbsp; Upload&nbsp;&nbsp; Total&nbsp;&nbsp; Spent&nbsp;&nbsp;&nbsp; Left&nbsp; Speed<br />&nbsp; 0&nbsp;&nbsp;&nbsp;&nbsp; 0&nbsp;&nbsp;&nbsp; 0&nbsp;&nbsp;&nbsp;&nbsp; 0&nbsp;&nbsp;&nbsp; 0&nbsp;&nbsp;&nbsp;&nbsp; 0&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 0&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 0 &#8211;:&#8211;:&#8211; &#8211;:&#8211;:&#8211; &#8211;:&#8211;:&#8211;&nbsp;&nbsp;&nbsp;&nbsp; 0* Connected to clientcertauth-demo.azurewebsites.net (111.221.95.27) port 443 (#0)<br />* STATE: WAITCONNECT => SENDPROTOCONNECT handle 0x80073200; line 1253 (connection #0) <br />* ALPN, offering http/1.1<br /><font color="#ff0000">* Cipher selection: ALL:!EXPORT:!EXPORT40:!EXPORT56:!aNULL:!LOW:!RC4:@STRENGTH</font><br /></font><font size="2"><font color="#ff0000">* successfully set certificate verify locations:<br />*&nbsp;&nbsp; CAfile: /usr/ssl/certs/ca-bundle.crt<br />&nbsp; CApath: none<br />* TLSv1.2 (OUT), TLS header, Certificate Status (22):<br />} [5 bytes data]<br />* TLSv1.2 (OUT), TLS handshake, Client hello (1):<br />} [512 bytes data]<br />* STATE: SENDPROTOCONNECT => PROTOCONNECT handle 0x80073200; line 1267 (connection #0) <br /></font><font color="#00ff00">ï»¿<!DOCTYPE html></font><br /></font><font size="2"><font color="#00ff00"><html></font></font></font>
                                    </p>
                                    
                                    <p align="center">
                                      <font face="Courier New"><font size="2"><font color="#00ff00"><&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8211;Trimmed HTML Response </font></font></font><font face="Courier New"><font size="2"><font color="#00ff00">&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8211;></font></font></font>
                                    </p>
                                    
                                    <p>
                                      <font face="Courier New"><font size="2"><font color="#00ff00"></html></font><br /></font><font size="2"><font color="#ff0000">{ [5 bytes data]<br />* TLSv1.2 (IN), TLS handshake, Server hello (2):<br />{ [81 bytes data]<br />* TLSv1.2 (IN), TLS handshake, Certificate (11):<br />{ [3245 bytes data]<br />* TLSv1.2 (IN), TLS handshake, Server key exchange (12):<br />{ [333 bytes data]<br />* TLSv1.2 (IN), TLS handshake, Server finished (14):<br />{ [4 bytes data]<br />* TLSv1.2 (OUT), TLS handshake, Client key exchange (16):<br />} [70 bytes data]<br />* TLSv1.2 (OUT), TLS change cipher, Client hello (1):<br />} [1 bytes data]<br />* TLSv1.2 (OUT), TLS handshake, Finished (20):<br />} [16 bytes data]<br />* TLSv1.2 (IN), TLS change cipher, Client hello (1):<br />{ [1 bytes data]<br />* TLSv1.2 (IN), TLS handshake, Finished (20):</font><br /><font color="#ff0000">{ [16 bytes data]</font><br /><font color="#ff0000">* SSL connection using TLSv1.2 / ECDHE-RSA-AES256-SHA384<br />* ALPN, server did not agree to a protocol<br />* Server certificate:<br />*&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; subject: CN=*.azurewebsites.net<br />*&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; start date: Sep 28 21:45:23 2016 GMT<br />*&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; expire date: May&nbsp; 7 17:03:30 2018 GMT<br />*&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; subjectAltName: clientcertauth-demo.azurewebsites.net matched<br />*&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; issuer: C=US; ST=Washington; L=Redmond; O=Microsoft Corporation; OU=Microsoft IT; CN=Microsoft IT SSL SHA2<br />*&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; SSL certificate verify ok.<br />* STATE: PROTOCONNECT => DO handle 0x80073200; line 1288 (connection #0) <br />} [5 bytes data]</font><br /><font color="#00ff00">> GET / HTTP/1.1<br />> Host: clientcertauth-demo.azurewebsites.net<br />> User-Agent: curl/7.47.1<br />> Accept: */*<br />> <br />* STATE: DO => DO_DONE handle 0x80073200; line 1350 (connection #0) <br />* STATE: DO_DONE => WAITPERFORM handle 0x80073200; line 1477 (connection #0) <br />* STATE: WAITPERFORM => PERFORM handle 0x80073200; line 1487 (connection #0) <br />{ [5 bytes data]</font><br /></font><font size="2"><font color="#ff0000">* TLSv1.2 (IN), TLS handshake, Hello request (0):<br />{ [4 bytes data]<br />* TLSv1.2 (OUT), TLS handshake, Client hello (1):<br />} [512 bytes data]<br />* TLSv1.2 (IN), TLS handshake, Server hello (2):<br />{ [105 bytes data]<br />* TLSv1.2 (IN), TLS handshake, Certificate (11):<br />{ [3245 bytes data]<br />* TLSv1.2 (IN), TLS handshake, Server key exchange (12):<br />{ [333 bytes data]<br /><font style="background-color: #ffff00" size="4"><strong>* TLSv1.2 (IN), TLS handshake, Request CERT (13):</strong></font><br />{ [30 bytes data]<br />* TLSv1.2 (IN), TLS handshake, Server finished (14):<br />{ [4 bytes data]<br />* TLSv1.2 (OUT), TLS handshake, Certificate (11):<br />} [7 bytes data]<br />* TLSv1.2 (OUT), TLS handshake, Client key exchange (16):<br />} [70 bytes data]<br />* TLSv1.2 (OUT), TLS change cipher, Client hello (1):<br />} [1 bytes data]<br />* TLSv1.2 (OUT), TLS handshake, Finished (20):<br />} [16 bytes data]<br />* TLSv1.2 (IN), TLS change cipher, Client hello (1):<br />{ [1 bytes data]<br />* TLSv1.2 (IN), TLS handshake, Finished (20):<br />{ [16 bytes data]<br /></font><font color="#00ff00">* HTTP 1.1 or later with persistent connection, pipelining supported<br />< HTTP/1.1 403 Forbidden<br />< Content-Type: text/html<br />* Server Microsoft-IIS/8.0 is not blacklisted<br />< Server: Microsoft-IIS/8.0<br />< Date: Fri, 09 Jun 2017 19:19:37 GMT<br />< Connection: close<br />< Content-Length: 2399</font></font></font>
                                    </p>
                                    
                                    <p align="center">
                                      <font face="Courier New"><font size="2"><font color="#00ff00"><&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8211;Trimmed </font></font></font><font face="Courier New"><font size="2"><font color="#00ff00">&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8211;></font></font></font>
                                    </p>
                                  </td>
                                </tr>
                              </table>
                            </blockquote>
                            
                            <p>
                              </font>
                            </p>
                            
                            <p>
                              <font size="2"></font>Hope this clarifies few doubts on how TLS Mutual Auth works on Azure App Service.
                            </p>
                            
                            <h3>
                              <u>RESTRICTIONS</u>
                            </h3>
                            
                            <li>
                              <font size="2">Currently, TLS Mutual Authentication is supported for web apps running in <strong>Basic</strong> or higher pricing tiers only. You will receive the following error if you try to enable it for a web app running in <strong>FREE/SHARED</strong> tier.</font><br /> <blockquote>
                                <table style="background-color: #e5e4e2" cellspacing="0" cellpadding="2" width="558" border="2">
                                  <tr>
                                    <td valign="top" width="554">
                                      <font size="2">&#8220;<font color="#c0504d">Cannot enable client certificate for a site &#8216;{0}&#8217; because current site mode does not allow it.</font>&#8220;</font>
                                    </td>
                                  </tr>
                                </table>
                              </blockquote>
                              
                              <li>
                                <font size="2">When the <code>clientCertEnabled</code> property is set to <code>true</code> the web app mandates the client to provide a client certificate. If the client fails to provide a client certificate they will receive a <strong>403 </strong>error. Those familiar with <strong>IIS</strong>, this is equivalent to setting the <strong>sslFlags</strong> property (<em>inside <strong><access></strong> tags</em>) in IIS to include “<code>SslRequireCert</code>”. <br /> <br /> 
                                
                                <blockquote>
                                  <table cellspacing="0" cellpadding="2" width="600" border="2">
                                    <tr>
                                      <td valign="top" width="596">
                                        <p>
                                          <font size="2" face="Courier New"><<font color="#c0504d">location </font><font color="#ff0000">path</font><font color="#0000ff">=&#8221;Kaushal&#8221;</font>><br />&nbsp;&nbsp;&nbsp; <<font color="#c0504d">system.webServer</font>><br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <<font color="#c0504d">security</font>><br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <font style="background-color: #ffff00"><<font color="#c0504d">access</font> <font color="#ff0000">sslFlags</font><font color="#0000ff">=&#8221;Ssl, SslNegotiateCert, SslRequireCert&#8221;</font> /><br /></font>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </<font color="#c0504d">security</font>><br />&nbsp;&nbsp;&nbsp; </<font color="#c0504d">system.webServer</font>><br /></<font color="#c0504d">location</font>></font>
                                        </p>
                                      </td>
                                    </tr>
                                  </table>
                                </blockquote>
                                
                                <p>
                                  </font>
                                </p>
                                
                                <li>
                                  <font size="2">As of now, <strong>Azure App Service </strong>supports Secure Renegotiation and doesn’t entertain <strong>ReNego</strong>. If there are TLS clients, that are not compliant as per the <a href="https://tools.ietf.org/html/rfc5746#section-3.7">RFC 5746</a> and depend on Re-Negotiation, then they cannot connect to <strong>Azure App Service</strong>.</font> <p>
                                    <font size="2"></font>
                                  </p>
                                </li>