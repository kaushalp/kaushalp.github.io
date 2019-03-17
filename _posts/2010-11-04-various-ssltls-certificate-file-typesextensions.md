---
id: 17
title: Various SSL/TLS Certificate File Types/Extensions
date: 2010-11-04T20:48:00+00:00
author: Kaushal Kumar Panday
layout: post
guid: https://blogs.msdn.microsoft.com/kaushal/2010/11/04/various-ssltls-certificate-file-typesextensions/
permalink: /2010/11/04/various-ssltls-certificate-file-typesextensions/
orig_url:
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2010/11/05/ssl-certificates.aspx
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2010/11/05/ssl-certificates.aspx
orig_site_id:
  - "13803"
  - "13803"
orig_post_id:
  - "10086470"
  - "10086470"
orig_parent_id:
  - "10086470"
  - "10086470"
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
  - http://blogs.msdn.com/b/kaushal/archive/2010/11/04/various-ssltls-certificate-file-typesextensions.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2010/11/04/various-ssltls-certificate-file-typesextensions.aspx
orig_post_name:
  - ssl certificates
  - ssl certificates
orig_thread_id:
  - "739387"
  - "739387"
orig_post_author_email:
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
orig_attachment_count:
  - "0"
  - "0"
total_views:
  - "95915"
  - "95915"
opengraph_tags:
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Various SSL/TLS Certificate File Types/Extensions" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2010/11/04/various-ssltls-certificate-file-typesextensions/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="Its not easy to determine by looking at a file extension whether it would carry a certificate or not. I will be discussing file extensions related to certificates . This would give you some idea on what are the different types of certificates that exist. My area of expertise is in IIS, so I would..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/0601.image_thumb_570CEB2F.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Various SSL/TLS Certificate File Types/Extensions" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2010/11/04/various-ssltls-certificate-file-typesextensions/" />
    <meta name="twitter:description" content="Its not easy to determine by looking at a file extension whether it would carry a certificate or not. I will be discussing file extensions related to certificates . This would give you some idea on what are the different types of certificates that exist. My area of expertise is in IIS, so I would..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/0601.image_thumb_570CEB2F.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Various SSL/TLS Certificate File Types/Extensions" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2010/11/04/various-ssltls-certificate-file-typesextensions/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="Its not easy to determine by looking at a file extension whether it would carry a certificate or not. I will be discussing file extensions related to certificates . This would give you some idea on what are the different types of certificates that exist. My area of expertise is in IIS, so I would..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/0601.image_thumb_570CEB2F.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Various SSL/TLS Certificate File Types/Extensions" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2010/11/04/various-ssltls-certificate-file-typesextensions/" />
    <meta name="twitter:description" content="Its not easy to determine by looking at a file extension whether it would carry a certificate or not. I will be discussing file extensions related to certificates . This would give you some idea on what are the different types of certificates that exist. My area of expertise is in IIS, so I would..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/0601.image_thumb_570CEB2F.png" />
    
categories:
  - Uncategorized
tags:
  - .cer
  - .crl
  - .key
  - .p7b
  - .sst
  - .stl
  - Certificates
  - PEM
  - PFS
  - PKCS
  - 'PKCS#12'
  - 'PKCS#7'
  - Private keys
  - SSL
---
<span style="font-family: Segoe UI; font-size: small;">Its not easy to determine by looking at a file extension whether it would carry a certificate or not.</span>

<span style="font-family: Segoe UI; font-size: small;">I will be discussing file extensions related to certificates . This would give you some idea on what are the different types of certificates that exist. My area of expertise is in IIS, so I would be discussing related to that mostly.</span>

<span style="font-family: Segoe UI; font-size: small;">SSL certificates are being used for various purposes such as:</span>

  * <span style="font-family: Segoe UI; font-size: small;"><strong>Authentication</strong>, The digital certificate is a common credential that provides a means to verify the identity of either the sender or the recipient.</span>
  * <span style="font-family: Segoe UI; font-size: small;"><strong>Privacy</strong>, which ensures that information, is only available to the intended audience. Certificates enable privacy of transmitted data using a number of different methods</span>
  * <span style="font-family: Segoe UI; font-size: small;"><strong>Encryption</strong>, which disguises information so that unauthorized readers are unable to decipher the message. On computers, sensitive data in the form of e-mail messages, files on a disk, and files being transmitted across the network can be encrypted using a key.</span>
  * <span style="font-family: Segoe UI; font-size: small;"><strong>Digital signatures</strong>, it provides strong evidence that the data has not been altered since it was signed and it confirms the identity of the person or entity who signed the data.</span>

<span style="font-size: small;"><strong><span style="font-family: Segoe UI;">Different types of Certificates:</span></strong></span>

<span style="font-family: Segoe UI; font-size: small;">Different file format exists for certificates based upon how they are encoded and what information store. They can be classified as ones that contain the private key and the ones that doesn&rsquo;t. We have many certificate file types that are supported on Windows. <span style="background-color: #ffff00;">The most commonly used file type which allows private key to be exported is the <strong>.pfx/.p12</strong> extension</span>.</span>

* * *

<p align="center">
  <span style="font-family: Segoe UI; font-size: small;"><span style="text-decoration: underline;"><strong>Certificate Signing Request (.csr)</strong></span></span>
</p>

<span style="font-family: Segoe UI; font-size: small;">This file type is sued by applications to submit requests to the <strong>Certification Authority</strong> or <strong>CA</strong>. The request can be base64 encoded as shown below and is enclosed between <span style="font-family: Segoe UI;">&#8220;</span><span style="font-family: Courier New;"><strong>&#8212;&#8211;BEGIN NEW CERTIFICATE REQUEST&#8212;&#8211;</strong></span><span style="font-family: Segoe UI;">&#8221; and &#8220;</span><span style="font-family: Courier New;"><strong>&#8212;&#8211;END NEW CERTIFICATE REQUEST&#8212;&#8211;</strong></span><span style="font-family: Segoe UI;">&#8220;. </span></span>

<table style="width: 519px;" border="1" cellspacing="0" cellpadding="2" align="center">
  <tr>
    <td valign="top" width="517">
      <p>
        <span style="font-family: Courier New; font-size: small;"><strong><span style="background-color: #ffff00;">&#8212;&#8211;BEGIN NEW CERTIFICATE REQUEST&#8212;&#8211;</span></strong> <br /> MIIERDCCAywCAQAwZDELMAkGA1UEBhMCVVMxEjAQBgNVBAgTCUthcm5hdGFrYTES <br /> MBAGA1UEBxMJQmFuZ2Fsb3JlMQswCQYDVQQKEwJNUzEMMAoGA1UECxMDQ1NTMRIw <br /> EAYDVQQDEwlhbmdlbC0yazMwggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAwggEKAoIB <br /> AQC8se11hL7I+nqePXGWaT9FNS9LisDbzG8Cb4IKIrLOlvtF7emO4mUxOzmBtXr+ <br /> nbpJkwZoY3/u9/0j6jpI8Uwh/VuWhWe16pIU0T0FODKGXhBre4E7aVsE0HyC/DRL <br /> tpkV2cQZPBmO5ZcXchLkh8H63aiBuqLH4kOZht3JGGllqa5GjPjShGYLAm7SqIJJ <br /> jbLFnKNW8ztdUn8cZhQfDlzpykqTAPY5XBo064D6fspKziGqgMiqMAW7ZKhAHWkF <br />Yrzp/YJCXHkajU+s79tdLk9X6+tn4qHEnOVILW0UWgw77QPvaNNFF0gmDYyUZje6 <br /> W2uaTjlcsQzgqbECSJVmT+cxAgMBAAGgggGZMBoGCisGAQQBgjcNAgMxDBYKNS4y <br /> LjM3OTAuMjB7BgorBgEEAYI3AgEOMW0wazAOBgNVHQ8BAf8EBAMCBPAwRAYJKoZI <br /> hvcNAQkPBDcwNTAOBggqhkiG9w0DAgICAIAwDgYIKoZIhvcNAwQCAgCAMAcGBSsO <br /> AwIHMAoGCCqGSIb3DQMHMBMGA1UdJQQMMAoGCCsGAQUFBwMBMIH9BgorBgEEAYI3 <br /> DQICMYHuMIHrAgEBHloATQBpAGMAcgBvAHMAbwBmAHQAIABSAFMAQQAgAFMAQwBo <br /> AGEAbgBuAGUAbAAgAEMAcgB5AHAAdABvAGcAcgBhAHAAaABpAGMAIABQAHIAbwB2 <br /> AGkAZABlAHIDgYkAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA <br /> AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA <br /> AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA <br /> AAAAADANBgkqhkiG9w0BAQUFAAOCAQEANR/QwFBkvXx7WVlnGWpsZNjMyNoBuwsP <br /> Wmjwu2FQ90+TSGexY0NI6cS1Xc9E0NlFuONcxJjaLclcW4Ptz1IpEUzK6t1CYV5q <br /> zJnyt7Fb2d6qY4Is6wrWo9IGOA0G814oxk8oMbBIXsjTZaE6JRW2NUts3lHSlgEY <br /> E1POkVex84jbmmIhJlqyBlSLH3d6rRYy8WaXMkaUTSBlp6vb3ealIsu5YTKtE1YW <br /> 9BYv1MHhVVIXoGts10y9s/NRrdVqDnVjgdYR+bjZaxbIca5loyYaMRCUBzFFIC7F <br /> W80lqPN3EcpySUoZbdDBM8R5M6sGWIbiagwToVMkx1KNpNA3lxYh5g== <br /><strong><span style="background-color: #ffff00;">&#8212;&#8211;END NEW CERTIFICATE REQUEST&#8212;&#8211;</span></strong></span>
      </p>
    </td>
  </tr>
</table>

* * *

<p align="center">
  <span style="font-size: small;"><strong></strong>&nbsp;<span style="font-family: Segoe UI;"><span style="text-decoration: underline;"><strong>Base64-encoded X.509 Certificate (.cer or .crt)</strong></span></span></span>
</p>

<span style="font-size: small;"><span style="font-family: Segoe UI;">The <strong>Base64</strong> format supports storage of a single certificate. This format does not support storage of the private key or certification path. They are Base64 encoded ASCII files. The encoded string is enclosed between &#8220;</span><span style="font-family: Courier New;"><strong>&#8212;&#8211;BEGIN CERTIFICATE&#8212;&#8211;</strong></span><span style="font-family: Segoe UI;">&#8221; and &#8220;</span><span style="font-family: Courier New;"><strong>&#8212;&#8211;END CERTIFICATE&#8212;&#8211;</strong></span><span style="font-family: Segoe UI;">&#8220;. Right click and open a certificate (<strong>exported in the base 64 format</strong>) in a notepad:</span></span>

<table style="width: 509px;" border="1" cellspacing="0" cellpadding="2" align="center">
  <tr>
    <td valign="top" width="507">
      <p>
        <span style="font-family: Courier New; font-size: small;"><span style="background-color: #ffff00;">&#8212;&#8211;BEGIN CERTIFICATE&#8212;&#8211;</span> <br /> MIIB0TCCATqgAwIBAgIQUq+2SdEkLr5K6xqjSEvRsDANBgkqhkiG9w0BAQUFADAU MRIwEAYDVQQDEwlsb2NhbGhvc3QwHhcNMTIwODA0MDA0OTEyWhcNMTcwODA0MDAw <br /> MDAwWjAUMRIwEAYDVQQDEwlsb2NhbGhvc3QwgZ8wDQYJKoZIhvcNAQEBBQADgY0A <br /> MIGJAoGBAKjGuGT8NN5chlGSHIqEgjgceLQOX41f46MvYZMbGecoaFcl4yGAcU21 <br /> 0oJeZyAjoZiuKueNdugqN4sTNq7IKpnK+cqNOr44aH1lCh6zAPz+KT/KtKuOBhXv <br /> Ypv6QL4eDVVYpMfHNk120xaItE+pk75ZKh6aXmh+v4HIFD/Off8XAgMBAAGjJDAi <br /> MAsGA1UdDwQEAwIEsDATBgNVHSUEDDAKBggrBgEFBQcDATANBgkqhkiG9w0BAQUF <br />AAOBgQCIBC/BE4ObFNbI6UV7bpg4abxrQDG+HYhMrLyw29jB4KNyeJPzkDHUkTua <br /> Y2nd44bYEpmaBy7XJ5UIGEkuD3VIxT2S+2bCwkRR+9/+7vggR2q7l7YEktM2mFBI <br />yqOMOroAw+5cdc06c/B7UimwKFczsyhi9LUIr3rXI42FdXBHWw== <br /><span style="background-color: #ffff00;">&#8212;&#8211;END CERTIFICATE&#8212;&#8211;</span></span>
      </p>
    </td>
  </tr>
  
  <tr>
    <td align="center" width="507">
      <span style="font-family: Segoe UI; font-size: small;"><strong>Base-64 encoded Certificate</strong></span>
    </td>
  </tr>
</table>

<span style="font-family: Segoe UI; font-size: small;">This file type is used more often for exporting certificates.</span>

* * *

<p align="center">
  <span style="font-size: small;"><strong><span style="font-family: Segoe UI;"><span style="text-decoration: underline;">DER-encoded binary X.509 Certificate (.cer, .der or .crt)</span></span></strong></span>
</p>

<span style="font-family: Segoe UI; font-size: small;">The <strong>Distinguished Encoding Rules (DER)</strong> format supports storage of a single certificate. This format does not support storage of the private key or certification path.</span>

<span style="font-family: Segoe UI; font-size: small;"><strong>DER </strong>is on of the encoding formats defined by <strong>ASN.1 </strong>in <strong>X.690</strong>. It is a variant or a subset of <strong>BER</strong>. You can refer the following Wiki article for further read:</span>

  * <span style="font-family: Segoe UI; font-size: small;"><a title="http://en.wikipedia.org/wiki/Distinguished_Encoding_Rules#DER_encoding" href="http://en.wikipedia.org/wiki/Distinguished_Encoding_Rules#DER_encoding">http://en.wikipedia.org/wiki/Distinguished_Encoding_Rules#DER_encoding</a></span>
  * <span style="font-size: small;"><a title="http://tools.ietf.org/html/rfc2986#ref-14" href="http://tools.ietf.org/html/rfc2986#ref-14"><span style="font-family: Segoe UI;">http://tools.ietf.org/html/rfc2986#ref-14</span></a></span>
  * <span style="font-size: small;"><a title="http://www.itu.int/ITU-T/studygroups/com17/languages/X.690-0207.pdf" href="http://www.itu.int/ITU-T/studygroups/com17/languages/X.690-0207.pdf"><span style="font-family: Segoe UI;">http://www.itu.int/ITU-T/studygroups/com17/languages/X.690-0207.pdf</span></a></span>

&nbsp;

* * *

<p align="center">
  <span style="font-family: Segoe UI; font-size: small;"><strong><span style="text-decoration: underline;">Cryptographic Message Syntax Standard (PKCS#7) Certificate (.p7b, .p7r or .spc)</span></strong></span>
</p>

<p align="left">
  <span style="font-family: Segoe UI; font-size: small;">The <strong>PKCS #7</strong> format supports storage of certificates and all certificates in the certification path. A <strong>PKCS #7</strong> file typically has a <strong>.p7b</strong> file name extension, but this is not always the case. This again doesn&rsquo;t support storage of private keys. It is generally used by the CA to provide certificate chain to clients.</span>
</p>

<span style="font-family: Segoe UI; font-size: small;">However as in the case of any other data file, the creator has the authority to use the existing .p7b extension or change it as desired.</span>

* * *

<p align="center">
  <span style="font-family: Segoe UI; font-size: small;"><strong><span style="text-decoration: underline;">Personal Information Exchange Format (PKCS#12) Certificate (.pfx or .p12)</span></strong></span>
</p>

<span style="font-family: Segoe UI; font-size: small;">The <strong>Personal Information Exchange format</strong> (PFX, also called PKCS #12) defines a file format that can be used for secure storage of certificates (containing both private and public keys), and all certificates in a certification path, protected with a password-based symmetric key. PFX is a predecessor to PKCS#12.</span>

<span style="font-family: Segoe UI; font-size: small;"><strong><span style="background-color: #ffff00;">The PKCS #12 formats is the only file format that can be used to export a certificate and its private key</span>.</strong> A PKCS#12 certificate containing a private key is shown below: </span>

<span style="font-size: small;"><a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8524.image_03961B16.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/8524.image_5F00_03961B16.png"><img style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" title="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/0601.image_thumb_570CEB2F.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/0601.image_5F00_thumb_5F00_570CEB2F.png" alt="image" width="388" height="484" border="0" /></a></span>

<span style="font-family: Segoe UI; font-size: small;"><span style="text-decoration: underline;"><strong>Certificate containing a private key</strong></span></span>

* * *

<p align="center">
  <span style="font-family: Segoe UI; font-size: small;"><strong><span style="text-decoration: underline;">Certificate Revocation List (.crl extension)</span></strong></span>
</p>

<span style="font-family: Segoe UI; font-size: small;">The <strong>Certificate Revocation List or CRL</strong> is a file type that identifies whether a certificate has been revocated or not. These files are provided by <strong>CA&rsquo;s</strong>. The client browser while accessing a site on <strong>HTTPS</strong> will use the <strong>CRL Distribution Points</strong> field in the certificate to download the CRL. Here is one example:</span>

<span style="font-size: small;"><a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/5074.image_152605E1.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/5074.image_5F00_152605E1.png"><img style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" title="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4807.image_thumb_41628CC5.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/4807.image_5F00_thumb_5F00_41628CC5.png" alt="image" width="396" height="494" border="0" /></a></span>

<span style="font-family: Segoe UI; font-size: small;"><span style="text-decoration: underline;"><strong>Certificate from login.live.com depicting the CRL Distribution Points</strong></span></span>

<span style="font-family: Segoe UI; font-size: small;"><span style="background-color: #cccccc;"><strong>NOTE</strong>: Not all certificates may have CRL distribution points. One good example is a Self-Signed certificate.</span></span>

<span style="font-family: Segoe UI; font-size: small;">Now, once the client (browser) gets the CRL information from the server certificate, it downloads the <strong>CRL</strong> file and checks the list to ensure that the current certificate is not part of that list. The <strong>CA</strong> can make the <strong>CRL</strong> available for download to the client, via <strong>HTTP</strong>, <strong>FTP</strong> or any other protocol. Here is the downloaded CRL from the CA:</span>

<p style="text-align: center;">
  <span style="font-size: small;"><a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/2744.image_58415E41.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/2744.image_5F00_58415E41.png"><img style="display: inline; background-image: none;" title="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6560.image_thumb_68D9592F.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/6560.image_5F00_thumb_5F00_68D9592F.png" alt="image" width="295" height="364" border="0" /></a><a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4426.image_1515E014.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/4426.image_5F00_1515E014.png"><img style="display: inline; background-image: none;" title="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/1108.image_thumb_25ADDB02.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/1108.image_5F00_thumb_5F00_25ADDB02.png" alt="image" width="296" height="365" border="0" /></a></span>
</p>

<span style="font-family: Segoe UI; font-size: small;"><span style="text-decoration: underline;"><strong>CRL file downloaded from the CA</strong></span></span>

* * *

<p align="center">
  <span style="font-family: Segoe UI; font-size: small;"><span style="text-decoration: underline;"><strong>Microsoft serialized certificate store (.sst)</strong></span></span>
</p>

<span style="font-family: Segoe UI; font-size: small;">This is one of the most rarely used file types. This format allows storage of multiple certificates in one single file. Typically it contains the <strong>ROOT CA</strong> certificates. It is the only file type which allows to save the certificate store. It preserves the properties of the certificate stores. There is another extension viz. &ldquo;<strong>.STO</strong>&rdquo;. However, I have rarely seen the usage of either of these file types.</span>

<span style="font-family: Segoe UI; font-size: small;">Not much documentation is available except this:</span>

<span style="font-size: small;"><a title="http://msdn.microsoft.com/en-us/library/dd921035(v=office.12).aspx" href="http://msdn.microsoft.com/en-us/library/dd921035(v=office.12).aspx"><span style="font-family: Segoe UI;">http://msdn.microsoft.com/en-us/library/dd921035(v=office.12).aspx</span></a></span>

* * *

<p align="center">
  <span style="font-family: Segoe UI; font-size: small;"><span style="text-decoration: underline;"><strong>Certificate Trust List (.stl)</strong></span></span>
</p>

<span style="font-family: Segoe UI; font-size: small;"><strong>Certificate Trust List </strong>is generally used during <strong>SSL/TLS handshake </strong>when <em>Client Certificate Authentication</em> comes in to picture. During SSL Handshake the server sends the client the list of the distinguished CA names that it supports as a part of <strong>Server Hello</strong> message. The Client uses this list to draw up a list of client certificates that is issued by any of the CA&rsquo;s in the list i.e., only those client certificates which are issued by any of the CA&rsquo;s in the CTL will be populated. Below is an example of how a CTL looks like</span>

<span style="font-size: small;"><a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6472.image_63C6F5B3.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/6472.image_5F00_63C6F5B3.png"><img style="margin-right: auto; margin-left: auto; display: block; background-image: none;" title="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3264.image_thumb_621629DF.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/3264.image_5F00_thumb_5F00_621629DF.png" alt="image" width="603" height="373" border="0" /></a></span>

* * *

<p align="center">
  <span style="font-family: Segoe UI; font-size: small;"><span style="text-decoration: underline;"><strong>Privacy-enhanced Electronic Mail (.pem)</strong></span></span>
</p>

<span style="font-family: Segoe UI; font-size: small;"><strong>PEM</strong> format is a refinement of base64 encoding. It has been documented in the following RFC&rsquo;s:</span>

<!--StartFragment--></p> 

  * <span style="font-family: Segoe UI; font-size: small;"><strong><a href="http://tools.ietf.org/html/rfc1421">RFC 1421: Part I: Message Encryption and Authentication Procedures</a></strong></span>

  * <span style="font-size: small;"><strong><span style="font-family: Segoe UI;"><a href="http://tools.ietf.org/html/rfc1422">RFC 1422: Part II: Certificate-Based Key Management</a></span></strong></span>

  * <span style="font-family: Segoe UI; font-size: small;"><strong><a href="http://tools.ietf.org/html/rfc1423">RFC 1423: Part III: Algorithms, Modes, and Identifiers</a></strong></span>

  * <span style="font-size: small;"><strong><span style="font-family: Segoe UI;"><a href="http://tools.ietf.org/html/rfc1424">RFC 1424: Part IV: Key Certification and Related Services</a></span></strong></span>

<!--EndFragment-->

<!--EndFragment-->

<!--EndFragment--></ul> 

<span style="font-family: Segoe UI; font-size: small;">This file format is typically used by <strong>OpenSSL</strong> to make Private Key available from a <strong>.pfx/.p12 </strong>file. So this is more widely used in the <strong>UNIX/LINUX </strong>world and not much in Windows. Once extracted to PEM format, this is how it looks:</span>

<table style="width: 570px;" border="1" cellspacing="0" cellpadding="2" align="center">
  <tr>
    <td valign="top" width="568">
      <p align="left">
        <span style="font-family: Segoe UI; font-size: small;">Command used to convert <strong>PFX</strong> to <strong>PEM</strong>:</span>
      </p>
      
      <p align="left">
        <span style="font-family: Courier New; font-size: small;">openssl.exe pkcs12 -in <strong><span style="background-color: #ffff00;">Certificate.pfx</span></strong> -nocerts -out <strong><span style="background-color: #ffff00;">Certificate.pem</span></strong></span>
      </p>
    </td>
  </tr>
  
  <tr>
    <td valign="top" width="568">
      <p>
        <span style="font-family: Courier New; font-size: small;">Bag Attributes <br />&nbsp;&nbsp;&nbsp; localKeyID: 01 00 00 00 <br />&nbsp;&nbsp;&nbsp; friendlyName: le-cd130455-259a-4b96-a900-94cc74670020 <br />&nbsp;&nbsp;&nbsp; Microsoft CSP Name: Microsoft Enhanced Cryptographic Provider v1.0 <br /> Key Attributes <br />&nbsp;&nbsp;&nbsp; X509v3 Key Usage: 10 <br /><strong><span style="background-color: #ffff00;">&#8212;&#8211;BEGIN RSA PRIVATE KEY&#8212;&#8211;</span></strong> <br />Proc-Type: 4,ENCRYPTED <br /> DEK-Info: DES-EDE3-CBC,4F53AB2E5701A52B</span>
      </p>
      
      <p>
        <span style="font-family: Courier New; font-size: small;">5XAtCElFXut0HuvYcKefoc+a++xm7tNXgzLGvIQiBgJbBipPLrnqxLr37xofX21u <br /> G5lnnPHyPSDTdna9fFryIM5sZQuZsvy1JjFyV4yOu1nl2wdzVRJyW/LSdN964lZV <br /> gj3CLaxMce5KL319i3t2A3SeFhMc6KnqxW8XEkkG7MpEhsL3Kz6bf5LJmuVeTfKx <br /> 0Ad3lr6t8ct6N8yPIFpqpMR/lHRevHvNilyAeU8dyxg7tzIFQOoapz+s/LjhbZWI <br /> XCdz2a/pH2ERFTKzCRg57dmmQ4znyHpiIxn92WOKQChQiDaIysGYBj4hbSZqaB8p <br /> 8H4x4t+TDjWcnIKLp5JxUJt3DN3qlzwP2Vdo/KTlFNvnmmEMmoTd931jALuk0+xC <br /> PaAz7KM1nDwe7zRwpIXCHkTTPp519icQrXj52tEO7sWhFVkjBaoaBVMeYPnpjb88 <br /> i9UcRUR908UtyT7lpkWPnD/I/Winm5rX/In2/743kZzNvYs/hz9S16DHHDY76S0o <br /> 0a6WKUlDtcE8EMHnVQqiFvpVWYVb01rh//EPbLB+F9AEvyuJ90SDAWHLK+7/qOoz <br /> 5ziFCsQJXTqL1GwORs06kIBMQQBJicznzqHnbebP5lWpfD5BI2rG1vPxxTob9Jh1 <br /> jObiX3z69QZmWPBqEjUzO/ByEtrBLJM8pJdIKNbYP/n6IcvX9ZekL3wRc6gc484M <br />Wx/RdPO2bpM0bY/Rxl2hx/nxV/X1Xu3LhQbSM6FibG5eLitT6gfJMCw/35zP7Ruc <br /> C+eDjPZfD5vm7xhal0yBDaYcmscPwM6jH87Cnn0RkyLjyeU4osvQNg== <br /><strong><span style="background-color: #ffff00;">&#8212;&#8211;END RSA PRIVATE KEY&#8212;&#8211;</span></strong></span>
      </p>
    </td>
  </tr>
</table>

<span style="font-size: small;"><span style="font-family: Segoe UI;">The two headers &rdquo;</span><span style="font-family: Courier New; background-color: #ffff00;"><strong>Proc-Type</strong></span><span style="font-family: Segoe UI;">&ldquo; and &ldquo;</span><span style="font-family: Courier New; background-color: #ffff00;"><strong>DEK-Info</strong></span><span style="font-family: Segoe UI;">&rdquo; specify the type of encryption. The string following afterwards with &ldquo;</span><span style="font-family: Courier New;">5XAtC&#8230;</span><span style="font-family: Segoe UI;">&rdquo; is <strong>Base64-encoded</strong>, <strong>encrypted</strong>, <strong>ASN.1</strong>-encoded object. Sometimes it also referred to as <strong><span style="text-decoration: underline;">Base-64 encoded DER Certificate</span></strong>.</span></span>

<span style="font-family: Segoe UI; font-size: small;">It is very similar to the PFX file format and can contain any/all of the following information in one single file.</span>

  * <span style="font-family: Segoe UI; font-size: small;"><strong>Issued Public Certificate (Client/Server)</strong></span>
  * <span style="font-family: Segoe UI; font-size: small;"><strong>Intermediate CA Certificate</strong></span>
  * <span style="font-family: Segoe UI; font-size: small;"><strong> Root CA certificate</strong></span>
  * <span style="font-family: Segoe UI; font-size: small;"><strong> Private Key</strong></span>

<span style="font-family: Segoe UI; font-size: small;"><span style="background-color: #ffff00;">A single PEM file can also be split into multiple PEM files each containing a part of the original PEM file</span>.</span>

<p align="center">
  <span style="font-family: Segoe UI; font-size: small;"><strong><span style="text-decoration: underline;">PEM for storing Public Key</span></strong></span>
</p>

<span style="font-family: Segoe UI; font-size: small;">This format can also be used for storing only the public key information of a certificate. I found this article: <a title="http://www.bo.infn.it/alice/introgrd/certmgr/node20.html" href="http://www.bo.infn.it/alice/introgrd/certmgr/node20.html,">http://www.bo.infn.it/alice/introgrd/certmgr/node20.html,</a> which talks about extracting only the public part of the certificate. Even in this case the file is a Base-64 encoded string enclosed between <span style="font-family: Segoe UI;">&#8220;</span><span style="font-family: Courier New;"><strong>&#8212;&#8211;BEGIN PUBLIC KEY&#8212;&#8211;</strong></span><span style="font-family: Segoe UI;">&#8221; and &#8220;</span><span style="font-family: Courier New;"><strong>&#8212;&#8211;END PUBLIC KEY&#8212;&#8211;</strong></span><span style="font-family: Segoe UI;">&#8220;. </span></span>

<table style="width: 522px;" border="1" cellspacing="0" cellpadding="2" align="center">
  <tr>
    <td valign="top" width="520">
      <p>
        <span style="font-size: small;"><span style="font-family: Courier New;"><strong><span style="background-color: #ffff00;">&#8212;&#8211;BEGIN PUBLIC KEY&#8212;&#8211;</span></strong> <br />MIICXQIBAAKBgQDedH/Kb8d0oqAu2+huQTHhQbqP1gx2Ae6LOtVejTt1Tg54f/iF <br /> 79E8wD/EUKNJ9omWCj4rFsPF6aiN+QNjmJc5zJqH4uCuIS7NeB2DCIeZxtS6f5oS <br />&#8230; <br /></span><span style="font-family: Courier New;">&#8230; <br /></span><span style="font-family: Courier New;">&#8230; <br /></span><span style="font-family: Courier New;">&#8230; <br /></span><span style="font-family: Courier New;">&#8230; <br /></span><span style="font-family: Courier New;">&#8230;</span><span style="font-family: Courier New;"> <br /></span><span style="font-family: Courier New;">qIco7Hxh0B71QnL/22lxAkAXcqs0Ah0yw3+3yBFDJgu1Wj/8gzMMRTrw8B07v13k <br /> gFlJxAuPc2ckMXsegTJf+mMaoS59KXMqcNh3B8P4V2ko <br /><strong><span style="background-color: #ffff00;">&#8212;&#8211;END PUBLIC KEY&#8212;&#8211;</span></strong></span></span>
      </p>
      
      <p>
        &nbsp;
      </p>
    </td>
  </tr>
</table>

<span style="font-family: Segoe UI; font-size: small;">I have personally never encountered any situation or a usage scenario where the public key information of the certificate had to be extracted.</span>

* * *

<p align="center">
  <span style="font-family: Segoe UI; font-size: small;"><span style="text-decoration: underline;"><strong>Private Key(.key)</strong></span></span>
</p>

<span style="font-family: Segoe UI; font-size: small;">This file format contains the private key of the certificate. On Windows&nbsp; there is no mechanism available to extract only the private key from the certificate, as it is not required. However, <strong>OpenSSL</strong> allows only the <strong>Private Key </strong>to be extracted from the certificate. <span style="font-family: Segoe UI;">If you open the file in a notepad, you would find that it is a Base-64 encoded string enclosed between <span style="font-family: Segoe UI;">&#8220;</span><span style="font-family: Courier New;"><strong>&#8212;&#8211;BEGIN RSA PRIVATE KEY&#8212;&#8211;</strong></span><span style="font-family: Segoe UI;">&#8221; and &#8220;</span><span style="font-family: Courier New;"><strong>&#8212;&#8211;END RSA PRIVATE KEY&#8212;&#8211;</strong></span><span style="font-family: Segoe UI;">&#8220;. </span></span></span>

<table style="width: 552px;" border="1" cellspacing="0" cellpadding="2" align="center">
  <tr>
    <td valign="top" width="550">
      <p align="left">
        <span style="font-family: Segoe UI; font-size: small;">Command used to convert <strong>PFX</strong> to <strong>PEM</strong>:</span>
      </p>
      
      <p align="left">
        <span style="font-family: Courier New; font-size: small;">openssl.exe pkcs12 -in <strong><span style="background-color: #ffff00;">Certificate.pfx</span></strong> -nocerts -out <strong><span style="background-color: #ffff00;">Certificate.pem</span></strong></span>
      </p>
    </td>
  </tr>
  
  <tr>
    <td valign="top" width="550">
      <p>
        <span style="font-family: Courier New; font-size: small;"><strong><span style="background-color: #ffff00;">&#8212;&#8211;BEGIN RSA PRIVATE KEY&#8212;&#8211;</span></strong> <br />MIICXQIBAAKBgQDedH/Kb8d0oqAu2+huQTHhQbqP1gx2Ae6LOtVejTt1Tg54f/iF <br /> 79E8wD/EUKNJ9omWCj4rFsPF6aiN+QNjmJc5zJqH4uCuIS7NeB2DCIeZxtS6f5oS <br />BWyoQ/eAjmFE0T/6P/aupsjrrB9qI7mELQnJEikzWCwsiBzSlM+bjdTDeQIDAQAB <br /> AoGBAItNyPisJusTK9wsOdFRYjr9Pib0k7kSXJ8zqIodRy6eQtGS0b6N/ylb+pKl <br /> LJwUlvQuVeAF0XMOb074sPadh5Suyos/Sa8OuHDDRmhxTQjk03EUhXrpGkA7WCU6 <br /> VdIf7xyCZFOc4RXy222xHfweZohEZ6qEdqyn7Cy6yQrHJKkBAkEA/15+gomP9rt4 <br /> M3Pyp+r2GsCm6aq1lHzF+/Req1Tzj/h4DlBN9dCNH2NnRFJ3S1GbrSsPR9YTpitu <br /> U+eah7+JXQJBAN8BMFa6bye1gc7Y/4McOfeNzUXzQc1TCCwdRxlF7VBxJkOcD3FD <br /> 53Ur/TSQL++TaE+ihsuQLUBnO31aJXOSlM0CQQCd83yckSmSmvIGITl90z7V3UNg <br /> VE5rwaFT7hqALtNXwX/AmrsdyBkBySIeiENxOtDnkzKoZClTJpnfG+ng/P+hAkA7 <br /> aWGreXfrqFuw8/b+wyJeZZTuseQyA5EFz7cFcK/M4phDIuyqTGD5woJu4osi1K7R <br /> qIco7Hxh0B71QnL/22lxAkAXcqs0Ah0yw3+3yBFDJgu1Wj/8gzMMRTrw8B07v13k <br /> gFlJxAuPc2ckMXsegTJf+mMaoS59KXMqcNh3B8P4V2ko <br /><strong><span style="background-color: #ffff00;">&#8212;&#8211;END RSA PRIVATE KEY&#8212;&#8211;</span></strong></span>
      </p>
      
      <p>
        &nbsp;
      </p>
    </td>
  </tr>
</table>

<span style="font-family: Segoe UI; font-size: small;">This is more widely used in <strong>JAVA </strong>& <strong>UNIX </strong>world.</span>

* * *

<p align="center">
  <span style="font-size: small;"><strong><span style="font-family: Segoe UI;"><span style="text-decoration: underline;">More on Certificates:</span></span></strong></span>
</p>

<span style="font-family: Segoe UI; font-size: small;">When a certificate request is created for a website in IIS 6, corresponding private key is also created. The requests are stored under the <strong>Certificate Enrollment Requests</strong> store under Computer account. This contains the private key information corresponding to the request raised.</span>

<span style="font-family: Segoe UI; font-size: small;">Once you have submitted the request to the CA. It will process the request and provide a certificate in .cer, crt or .der extension (<strong>DER or Base64 encoded</strong>). Now the pending request can be processed in the IIS Manager by installing the certificate which was provided by the CA.</span>

<span style="font-family: Segoe UI; font-size: small;">Consider, if somehow the request for the certificate was lost i.e., the request under the <strong>Certificate Enrollment Requests </strong>was removed. Now if you install the certificate on the website you are bound to see some issues due to the missing key information. The SSL handshake will not complete and you will see a &ldquo;<strong><span style="color: #ff0000;">Page cannot be displayed error message</span></strong>&rdquo; on the browser.</span>

<span style="font-family: Segoe UI; font-size: small;"><strong><span style="color: #ff0000; background-color: #ffff00;">By default a .cer file doesn&rsquo;t contain a private key</span>.</strong> The notion of such file is that the private key already exists on the server and during installation the binds to the certificate. Now since the request (private key) no longer exists the server doesn&rsquo;t know how to decrypt the information received from client (encrypted using the public key). However, we are not totally helpless. We can try to retrieve the private key for the certificate. Here are the steps to do it:</span>

<span style="font-family: Segoe UI; font-size: small;">1. Import the certificate to the personal store of computer account.</span>

<span style="font-family: Segoe UI; font-size: small;">2. Now double click the certificate and go to the <strong>Details</strong> tab. Select the Thumbprint section and copy the value as shown below:</span>

<span style="font-size: small;"><a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/2678.image_14998752.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/2678.image_5F00_14998752.png"><img style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" title="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/0624.image_thumb_77442F87.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/0624.image_5F00_thumb_5F00_77442F87.png" alt="image" width="400" height="499" border="0" /></a></span>

<span style="font-family: Segoe UI; font-size: small;">3. We will use <strong>certutil</strong> tool to map the private key to the certificate. Open a command prompt and execute the following:</span>

<span style="font-family: Segoe UI; font-size: small;"><span style="font-family: Segoe UI;">&nbsp;</span></span>

<table style="width: 600px;" border="1" cellspacing="0" cellpadding="2">
  <tr>
    <td valign="top" width="600">
      <span style="font-size: small;"><span style="font-family: Courier New;"><strong>Certutil -repairstore my &#8220;73 14 b2 20 1c 57 f9 fe 19 36 cf ff 9f cb c9 1e 8c 0f 1a 02</strong>&#8220;</span></span>
    </td>
  </tr>
</table>

<span style="font-family: Segoe UI; font-size: small;">If the command is successful then you will see a confirmation message as shown below:</span>

<span style="font-size: small;"><a href="http://kaushalkp.files.wordpress.com/2010/11/clip_image0091.jpg"><span style="font-family: Segoe UI;"><img style="margin-right: auto; margin-left: auto; display: block;" title="clip_image009" src="http://kaushalkp.files.wordpress.com/2010/11/clip_image009_thumb.jpg?w=642&h=185" alt="clip_image009" width="642" height="185" /></span></a></span>

<span style="font-family: Segoe UI; font-size: small;">More information on <strong>certutil </strong>tool can be found here: <br /><a title="http://technet.microsoft.com/en-us/library/cc772898%28WS.10%29.aspx" href="http://technet.microsoft.com/en-us/library/cc772898%28WS.10%29.aspx">http://technet.microsoft.com/en-us/library/cc772898%28WS.10%29.aspx</a></span>

<span style="font-size: small;"><span style="font-family: Segoe UI;"><strong><span style="text-decoration: underline;">Scenarios:</span></strong></span></span>

<span style="font-family: Segoe UI; font-size: small;">Sometimes the web-administrator has to install the same certificate across various servers in a load balanced server. So, continuing from the above scenario let&rsquo;s assume the web-admin has to install the cert on other 12 servers. Manually copying the .cer file to every server and running the above command is quite tedious. </span>

<span style="font-family: Segoe UI; font-size: small;">Why can&rsquo;t we export the certificate along with the private key to the other servers and then install it? Well, it can be done, <strong>provided the private key has been marked as exportable</strong>. Generally, you would see this if the certificate was renewed again with the private key not being exported earlier.</span>

<span style="font-family: Segoe UI; font-size: small;">Go to the websites on which the certificate has been installed. </span>

  1. <span style="font-family: Segoe UI; font-size: small;">Right click and select <strong>Properties</strong>-> <strong>Directory Security</strong>-> <strong>View Certificate</strong>. </span>
  2. <span style="font-family: Segoe UI; font-size: small;">Now go to the details tab and click on &ldquo;<strong>Copy to File&hellip;</strong>&rdquo;</span>
  3. <span style="font-family: Segoe UI; font-size: small;">Click on Next, you will now see a window provided with 2 radio buttons</span>
  * <span style="font-family: Segoe UI; font-size: small;"><strong>Yes, export the private key</strong></span>
  * <span style="font-family: Segoe UI; font-size: small;"><strong>No, do not export the private key</strong></span>

  4. <span style="font-family: Segoe UI; font-size: small;">If the private key was not marked as exportable, earlier when the certificate was created the first time, then the first option would be grayed out.</span>
  5. <span style="font-family: Segoe UI; font-size: small;">Select the first option &ldquo;<strong>Yes, export the private key</strong>&rdquo; and click on Next.</span>
  6. <span style="font-family: Segoe UI; font-size: small;">In the next window the &ldquo;<strong>Personal Information Exchange &ndash; PKCS#12 (.PFX)</strong>&rdquo; will be selected provided with three checkboxes. Select the first and third option and&nbsp;then click on <strong>Next</strong>.</span>
  * <span style="font-size: small;"><a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/7571.image_3C1053BC.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/7571.image_5F00_3C1053BC.png"><img style="margin-right: auto; margin-left: auto; display: block; background-image: none;" title="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/2275.image_thumb_0F8723D6.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/2275.image_5F00_thumb_5F00_0F8723D6.png" alt="image" width="501" height="488" border="0" /></a></span>

  7. <span style="font-family: Segoe UI; font-size: small;">Type in the password if required and then click on Next.</span>
  8. <span style="font-family: Segoe UI; font-size: small;">Browse to the location where you want to save the file (in .pfx format) and then click on Next.</span>
  9. <span style="font-family: Segoe UI; font-size: small;">Click on Finish, you would get a small prompt saying &ldquo;The export was successful&rdquo;</span>
 10. <span style="font-family: Segoe UI; font-size: small;">Click on OK and it&rsquo;s done.</span>

<span style="font-size: small;"><span style="font-family: Segoe UI;">Now you have a SSL certificate containing the Private Key. You can copy this to other servers and then install it on the website. You may also choose to install the certificate programmatically on IIS using the KB article </span><a href="http://support.microsoft.com/kb/313624"><span style="font-family: Segoe UI;">313624</span></a><span style="font-family: Segoe UI;">.</span></span>