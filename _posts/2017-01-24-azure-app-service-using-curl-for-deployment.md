---
id: 1495
title: 'Azure App Service: Using cURL for deployment'
date: 2017-01-24T10:56:48+00:00
author: Kaushal Kumar Panday
layout: post
guid: https://blogs.msdn.microsoft.com/kaushal/?p=1495
permalink: /2017/01/24/azure-app-service-using-curl-for-deployment/
opengraph_tags:
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Azure App Service: Using cURL for deployment" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2017/01/24/azure-app-service-using-curl-for-deployment/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="cURL is a command line tool that can be used to send or receive files. cURL.exe supports numerous protocols like HTTP, HTTPS, FTP, FTPS, SFTP, LDAP, TELNET, SMTP, POP3 etc. For more information please refer the below links: https://en.wikipedia.org/wiki/CURL https://curl.haxx.se/docs/ Syntax  curl.exe -T &lt;path-to-file-that-needs-to-be-deployed&gt; -u &#8220;username:password&#8221; &#8220;FTP URL&#8221; From curl documentation &#8211;T, &#8212;upload-file FILE Transfer..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2017/01/image_thumb521.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Azure App Service: Using cURL for deployment" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2017/01/24/azure-app-service-using-curl-for-deployment/" />
    <meta name="twitter:description" content="cURL is a command line tool that can be used to send or receive files. cURL.exe supports numerous protocols like HTTP, HTTPS, FTP, FTPS, SFTP, LDAP, TELNET, SMTP, POP3 etc. For more information please refer the below links: https://en.wikipedia.org/wiki/CURL https://curl.haxx.se/docs/ Syntax  curl.exe -T &lt;path-to-file-that-needs-to-be-deployed&gt; -u &#8220;username:password&#8221; &#8220;FTP URL&#8221; From curl documentation &#8211;T, &#8212;upload-file FILE Transfer..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2017/01/image_thumb521.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Azure App Service: Using cURL for deployment" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2017/01/24/azure-app-service-using-curl-for-deployment/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="cURL is a command line tool that can be used to send or receive files. cURL.exe supports numerous protocols like HTTP, HTTPS, FTP, FTPS, SFTP, LDAP, TELNET, SMTP, POP3 etc. For more information please refer the below links: https://en.wikipedia.org/wiki/CURL https://curl.haxx.se/docs/ Syntax  curl.exe -T &lt;path-to-file-that-needs-to-be-deployed&gt; -u &#8220;username:password&#8221; &#8220;FTP URL&#8221; From curl documentation &#8211;T, &#8212;upload-file FILE Transfer..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2017/01/image_thumb521.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Azure App Service: Using cURL for deployment" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2017/01/24/azure-app-service-using-curl-for-deployment/" />
    <meta name="twitter:description" content="cURL is a command line tool that can be used to send or receive files. cURL.exe supports numerous protocols like HTTP, HTTPS, FTP, FTPS, SFTP, LDAP, TELNET, SMTP, POP3 etc. For more information please refer the below links: https://en.wikipedia.org/wiki/CURL https://curl.haxx.se/docs/ Syntax  curl.exe -T &lt;path-to-file-that-needs-to-be-deployed&gt; -u &#8220;username:password&#8221; &#8220;FTP URL&#8221; From curl documentation &#8211;T, &#8212;upload-file FILE Transfer..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2017/01/image_thumb521.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Azure App Service: Using cURL for deployment" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2017/01/24/azure-app-service-using-curl-for-deployment/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="cURL is a command line tool that can be used to send or receive files. cURL.exe supports numerous protocols like HTTP, HTTPS, FTP, FTPS, SFTP, LDAP, TELNET, SMTP, POP3 etc. For more information please refer the below links: https://en.wikipedia.org/wiki/CURL https://curl.haxx.se/docs/ Syntax  curl.exe -T &lt;path-to-file-that-needs-to-be-deployed&gt; -u &#8220;username:password&#8221; &#8220;FTP URL&#8221; From curl documentation &#8211;T, &#8212;upload-file FILE Transfer..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2017/01/image_thumb521.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Azure App Service: Using cURL for deployment" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2017/01/24/azure-app-service-using-curl-for-deployment/" />
    <meta name="twitter:description" content="cURL is a command line tool that can be used to send or receive files. cURL.exe supports numerous protocols like HTTP, HTTPS, FTP, FTPS, SFTP, LDAP, TELNET, SMTP, POP3 etc. For more information please refer the below links: https://en.wikipedia.org/wiki/CURL https://curl.haxx.se/docs/ Syntax  curl.exe -T &lt;path-to-file-that-needs-to-be-deployed&gt; -u &#8220;username:password&#8221; &#8220;FTP URL&#8221; From curl documentation &#8211;T, &#8212;upload-file FILE Transfer..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2017/01/image_thumb521.png" />
    
categories:
  - --cacert
  - "550"
  - Azure
  - Azure App Service
  - Azure Web App
  - Azure Websites
  - cURL
  - FTP
  - FTPS
---
**cURL** is a command line tool that can be used to send or receive files. <span style="font-size: small">cURL.exe supports numerous protocols like HTTP, HTTPS, FTP, FTPS, SFTP, LDAP, TELNET, SMTP, POP3 etc. For more information please refer the below links:</span>

> [<span style="font-size: small">https://en.wikipedia.org/wiki/CURL</span>](https://en.wikipedia.org/wiki/CURL "https://en.wikipedia.org/wiki/CURL")  
> [<span style="font-size: small">https://curl.haxx.se/docs/</span>](https://curl.haxx.se/docs/ "https://curl.haxx.se/docs/")

## <span style="text-decoration: underline">Syntax</span>

> ** <span style="font-size: small;font-family: 'Courier New';background-color: #cccccc">curl.exe -T <path-to-file-that-needs-to-be-deployed> -u &#8220;username:password&#8221; &#8220;FTP URL&#8221; </span>**

<span style="font-size: small">From curl documentation<br /></span>

> <table cellspacing="0" cellpadding="2" width="476" border="2">
>   <tr>
>     <td bgcolor="#e0e0e0" valign="top" width="472">
>       <span style="font-family: consolas"><span style="font-size: small">&#8211;<strong>T</strong>, &#8212;<strong>upload-file</strong> FILE Transfer FILE to destination</span><br /></span><span style="font-family: consolas"><span style="font-size: small">&#8212;<strong>url</strong> URL URL to work with</span> </span><span style="font-family: consolas"><span style="font-size: small">-u, <strong>&#8211;user</strong> USER[:PASSWORD] Server user and password</span><br /></span><span style="font-family: consolas"><span style="font-size: small">&#8212;<strong>tlsuser</strong> USER TLS username</span><br /></span><span style="font-family: consolas"><span style="font-size: small">&#8212;<strong>tlspassword</strong> STRING TLS password</span><br /></span><span style="font-size: small;font-family: consolas">&#8212;<strong>tlsauthtype</strong> STRING TLS authentication type (default SRP)</span>
>     </td>
>   </tr>
> </table>

### <span style="text-decoration: underline"><font size="6" face="Segoe UI Semilight">Pre-Requisites:</font></span>

  * <span style="font-size: small">Deployment over <strong>FTPS</strong> will work only if the version of the curl is SSL aware. Download it from here:</span> 

[<span style="font-size: small">https://curl.haxx.se/download.html</span>](https://curl.haxx.se/download.html)

  * <span style="font-size: small">FTP endpoint of the web app. You can get this from portal or from the publish profile of the web app (under FTP section search for publishURL)</span> 
      * <span style="font-size: small">Username and password for authentication (Either deployment or publish profile credentials. See </span>[<span style="font-size: small">this</span>](https://github.com/projectkudu/kudu/wiki/Deployment-credentials)<span style="font-size: small">)</span> 
          * <span style="font-size: small">With user-level credentials (User specific): sitename\username</span> 
              * <span style="font-size: small">With site-level credentials (Site specific/publish profile) : sitename\$sitename</span> </ul> 
        
        > <table cellspacing="0" cellpadding="2" width="731" border="2">
        >   <tr>
        >     <td bgcolor="#e0e0e0" valign="top" width="727">
        >       <h4>
        >         <span style="font-size: large;font-family: 'Segoe UI Semibold'">For FTPS<br /></span>
        >       </h4>
        >       
        >       <ul>
        >         <ul>
        >           <li>
        >             <span style="font-size: small">Browse to the following location: </span><a href="http://curl.haxx.se/docs/caextract.html"><span style="font-size: small">http://curl.haxx.se/docs/caextract.html</span></a> <li>
        >               <span style="font-size: small">Right click and download the &#8220;cacert.pem&#8221; file and rename the file extension to &#8220;.crt&#8221; (Use Chrome)</span>
        >             </li></ul> </ul> </td> </tr> </tbody> </table> </blockquote> 
        >             <h2>
        >               <span style="text-decoration: underline"><span style="font-family: 'Segoe UI Semibold'"><font size="6" face="Segoe UI Semilight">Deploying via FTP</font></span></span>
        >             </h2>
        >             
        >             <ul>
        >               <li>
        >                 <span style="font-size: small">Launch command prompt</span> <li>
        >                   <span style="font-size: small">Browse to the folder location where curl was downloaded and execute the following command:</span>
        >                 </li></ul> 
        >                 <blockquote>
        >                   <table cellspacing="0" cellpadding="2" width="870" border="2">
        >                     <tr>
        >                       <td bgcolor="#a4a4a4" valign="top" width="907">
        >                         <span style="font-size: small;font-family: consolas">C:\>curl -T C:\sample.war -u &#8220;<span style="background-color: #00ff00">kaushalp\$kaushalp</span>:<password>&#8221; </span><a href="ftp://waws-prod-sg1-005.ftp.azurewebsites.windows.net/site/wwwroot/"><span style="font-size: small;font-family: consolas">ftp://waws-prod-sg1-005.ftp.azurewebsites.windows.net/site/wwwroot/</span></a><span style="font-family: consolas"> </span>
        >                       </td>
        >                     </tr>
        >                   </table>
        >                 </blockquote>
        >                 
        >                 <blockquote>
        >                   <p>
        >                     <a href="https://msdnshared.blob.core.windows.net/media/2017/01/image603.png"><img title="image" style="border-left-width: 0px;border-right-width: 0px;border-bottom-width: 0px;padding-top: 0px;padding-left: 0px;padding-right: 0px;border-top-width: 0px" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/2017/01/image_thumb521.png" width="876" height="161" /></a>
        >                   </p>
        >                 </blockquote>
        >                 
        >                 <h2>
        >                   <span style="text-decoration: underline"><span style="font-family: 'Segoe UI Semibold'"><font size="6" face="Segoe UI Semilight">Deploying via FTPS</font></span></span>
        >                 </h2>
        >                 
        >                 <p>
        >                   <span style="font-size: small">While using <strong>cURL </strong>via FTPS (FTP over SSL), the following error may be encountered when trying to connect over HTTP.</span>
        >                 </p>
        >                 
        >                 <blockquote>
        >                   <p>
        >                     <a href="https://msdnshared.blob.core.windows.net/media/2017/01/image604.png"><img title="image" style="border-left-width: 0px;border-right-width: 0px;border-bottom-width: 0px;padding-top: 0px;padding-left: 0px;padding-right: 0px;border-top-width: 0px" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/2017/01/image_thumb522.png" width="790" height="365" /></a>
        >                   </p>
        >                 </blockquote>
        >                 
        >                 <p>
        >                   <span style="font-size: small">The following error is seen because curl will try to verify the certificate received in the Server Hello and it fails as it couldn’t verify the CA who issued the certificate.</span>
        >                 </p>
        >                 
        >                 <p>
        >                   <span style="font-size: small">This problem can be addressed by using an additional parameter either <strong><span style="background-color: #ffff00">&#8211;cacert </span></strong>or <strong><span style="background-color: #ffff00">-k</span> </strong>can be specified.</span>
        >                 </p>
        >                 
        >                 <blockquote>
        >                   <table cellspacing="0" cellpadding="2" width="798" border="2">
        >                     <tr>
        >                       <td bgcolor="#a4a4a4" valign="top" width="794">
        >                         <span style="font-family: consolas"><span style="font-size: small">C:\>curl -T C:\sample.war -u &#8220;<span style="background-color: #00ff00">kaushalp\$kaushalp</span>:<password>&#8221; ftps://waws-prod-sg1-005.ftp.azurewebsites.windows.net/site/wwwroot/ <span style="background-color: #ffff00">-k</span></span> </span>
        >                       </td>
        >                     </tr>
        >                   </table>
        >                 </blockquote>
        >                 
        >                 <p>
        >                   <span style="font-size: small"><strong><span style="background-color: #ffff00">-k, &#8211;insecure</span></strong> Allow connections to SSL sites without certs (H)</span>
        >                 </p>
        >                 
        >                 <blockquote>
        >                   <table cellspacing="0" cellpadding="2" width="794" border="2">
        >                     <tr>
        >                       <td bgcolor="#a4a4a4" valign="top" width="790">
        >                         <span style="font-family: consolas"><span style="font-size: small">C:\>curl -T C:\sample.war -u &#8220;<span style="background-color: #00ff00">kaushalp\$kaushalp</span>:<password>&#8221; ftps://waws-prod-sg1-005.ftp.azurewebsites.windows.net/site/wwwroot/ <span style="background-color: #ffff00">&#8211;cacert e:\tools\kaushal-bundle.crt</span></span> </span>
        >                       </td>
        >                     </tr>
        >                   </table>
        >                 </blockquote>
        >                 
        >                 <p>
        >                   <span style="font-size: small"><strong><span style="background-color: #ffff00">&#8211;cacert</span></strong> FILE CA certificate to verify peer against (SSL)</span>
        >                 </p>
        >                 
        >                 <h1 align="center">
        >                   <span style="text-decoration: underline"><span style="font-family: 'Segoe UI Semibold'"><font size="6" face="Segoe UI Semilight">TROUBLESHOOTING</font></span></span>
        >                 </h1>
        >                 
        >                 <p style="padding-left: 30px">
        >                   <span style="font-size: small">Error: &#8220;<span style="color: #ff0000">curl: (25) Failed FTP upload: 550</span>&#8220;<br /><a href="https://msdnshared.blob.core.windows.net/media/2017/01/image605.png"><img title="image" style="border-left-width: 0px;border-right-width: 0px;border-bottom-width: 0px;padding-top: 0px;padding-left: 0px;padding-right: 0px;border-top-width: 0px" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/2017/01/image_thumb523.png" width="903" height="149" /><br /></a>This error is seen when the FTP URL does not contain a trailing slash &#8220;/&#8221;.</span>
        >                 </p>
        >                 
        >                 <h2>
        >                   <span style="text-decoration: underline"><span style="font-size: large">More Information:</span></span>
        >                 </h2>
        >                 
        >                 <p>
        >                   <span style="font-size: small">Here is the default list of CA&#8217;s that are supported by curl: </span><a href="https://curl.haxx.se/ca/cacert.pem"><span style="font-size: small">https://curl.haxx.se/ca/cacert.pem</span></a><span style="font-size: small"> (This was the file that was downloaded under pre-requisites)</span>
        >                 </p>
        >                 
        >                 <p>
        >                   <span style="font-size: small">Users can generate their own crt file and pass it to CURL. </span>
        >                 </p>
        >                 
        >                 <p>
        >                   <span style="font-size: small"></span>
        >                 </p>