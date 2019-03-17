---
id: 131
title: 'Error HRESULT: 0x80070520 when adding SSL binding in IIS'
date: 2012-10-07T05:36:58+00:00
author: Kaushal Kumar Panday
layout: post
guid: https://blogs.msdn.microsoft.com/kaushal/2012/10/07/error-hresult-0x80070520-when-adding-ssl-binding-in-iis/
permalink: /2012/10/07/error-hresult-0x80070520-when-adding-ssl-binding-in-iis/
orig_url:
  - 'http://blogs.msdn.microsoft.com/b/kaushal/archive/2012/10/07/error-hresult-0x80070520-when-adding-ssl-binding-in%20-iis.aspx'
  - 'http://blogs.msdn.microsoft.com/b/kaushal/archive/2012/10/07/error-hresult-0x80070520-when-adding-ssl-binding-in%20-iis.aspx'
orig_site_id:
  - "13803"
  - "13803"
orig_post_id:
  - "10357119"
  - "10357119"
orig_parent_id:
  - "10357119"
  - "10357119"
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
  - http://blogs.msdn.com/b/kaushal/archive/2012/10/07/error-hresult-0x80070520-when-adding-ssl-binding-in-iis.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2012/10/07/error-hresult-0x80070520-when-adding-ssl-binding-in-iis.aspx
orig_post_name:
  - error hresult 0x80070520 when adding ssl binding in iis
  - error hresult 0x80070520 when adding ssl binding in iis
orig_thread_id:
  - "822998"
  - "822998"
orig_post_author_email:
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
orig_attachment_count:
  - "0"
  - "0"
total_views:
  - "71671"
  - "71671"
opengraph_tags:
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Error HRESULT: 0x80070520 when adding SSL binding in IIS" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/10/07/error-hresult-0x80070520-when-adding-ssl-binding-in-iis/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="Today I will be discussing the very infamous error that is seen while adding a SSL binding in IIS 7 &amp; higher. Below is a snapshot of the error message while trying to add the SSL binding in IIS. Well, the error is definitely not descriptive enough, neither does it provide any vital information to..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/0741.image_thumb_7AFE7B16.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Error HRESULT: 0x80070520 when adding SSL binding in IIS" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/10/07/error-hresult-0x80070520-when-adding-ssl-binding-in-iis/" />
    <meta name="twitter:description" content="Today I will be discussing the very infamous error that is seen while adding a SSL binding in IIS 7 &amp; higher. Below is a snapshot of the error message while trying to add the SSL binding in IIS. Well, the error is definitely not descriptive enough, neither does it provide any vital information to..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/0741.image_thumb_7AFE7B16.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Error HRESULT: 0x80070520 when adding SSL binding in IIS" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/10/07/error-hresult-0x80070520-when-adding-ssl-binding-in-iis/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="Today I will be discussing the very infamous error that is seen while adding a SSL binding in IIS 7 &amp; higher. Below is a snapshot of the error message while trying to add the SSL binding in IIS. Well, the error is definitely not descriptive enough, neither does it provide any vital information to..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/0741.image_thumb_7AFE7B16.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Error HRESULT: 0x80070520 when adding SSL binding in IIS" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/10/07/error-hresult-0x80070520-when-adding-ssl-binding-in-iis/" />
    <meta name="twitter:description" content="Today I will be discussing the very infamous error that is seen while adding a SSL binding in IIS 7 &amp; higher. Below is a snapshot of the error message while trying to add the SSL binding in IIS. Well, the error is definitely not descriptive enough, neither does it provide any vital information to..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/0741.image_thumb_7AFE7B16.png" />
    
categories:
  - Uncategorized
tags:
  - 0x80070520
  - keyspec
  - SSL
---
<font size="2" face="Segoe UI">Today I will be discussing the very infamous error that is seen while adding a SSL binding in IIS 7 & higher. Below is a snapshot of the error message while trying to add the SSL binding in IIS.</font>

<a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/7610.image_4A4B736B.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/7610.image_5F00_4A4B736B.png"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/0741.image_thumb_7AFE7B16.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/0741.image_5F00_thumb_5F00_7AFE7B16.png" width="498" height="248" /></a>

<font size="2" face="Segoe UI">Well, the error is definitely not descriptive enough, neither does it provide any vital information to troubleshoot the issue. However, if you look at the Event logs, you will find the clue and the reason why the error is seen.</font>

<table cellspacing="0" cellpadding="2" width="750" align="center" border="2">
  <tr>
    <td valign="top" width="746">
      <p>
        <font size="2" face="Courier New">Log Name:&#160;&#160;&#160;&#160;&#160; System <br />Source:&#160;&#160;&#160;&#160;&#160;&#160;&#160; Schannel <br />Date:&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; 07-10-2012 02:13:15 <br />Event ID:&#160;&#160;&#160;&#160;&#160; 36870 <br />Task Category: None <br />Level:&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; Error <br />Keywords:&#160;&#160;&#160;&#160;&#160; <br />User:&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; SYSTEM <br />Computer:&#160;&#160;&#160;&#160;&#160; xxxxxxxxx <br />Description: <br /><font style="background-color: rgb(255, 255, 0);" color="#ff0000"><strong>A fatal error occurred when attempting to access the SSL server credential private key</strong></font>. The error code returned from the cryptographic module is 0x8009030d. The internal error state is 10001.</font>
      </p>
    </td>
  </tr>
  
  <tr>
    <td width="746" align="center">
      <font size="2" face="Segoe UI"><strong>Event message logged in the system event logs on failure.</strong></font>
    </td>
  </tr>
</table>

<font size="2" face="Segoe UI">The event logs should give you some clue regarding the problem. The primary reason for the above error is the problem in accessing the “<strong>Private Key</strong>” of the certificate due to a broken keyset.</font>

<font size="2" face="Segoe UI">For those who may not be following, Public Key Cryptography deals with “<strong>Public Key</strong>” & “<strong>Private Key</strong>”. The Public key is distributed to the clients, while only the Server has access to the Private key as it is used for decrypting the SSL Request. So “<strong>Private Key</strong>” is of utmost importance here.</font>

<font size="2" face="Segoe UI">There are few scenarios where we could see a problem accessing the “<strong>Private Key</strong>” of the SSL Cert. I will discuss a few in this article:</font>

* * *

<h1 align="center">
  <font size="5" face="Segoe UI"><u>SCENARIO 1</u></font>
</h1>

<font size="2" face="Segoe UI">The most common scenario is when the users use the IIS MMC to import a certificate and they uncheck the option “<strong>Allow this certificate to be exported</strong>”. This results in a broken keyset and thus results in the problem.</font>

<a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/0601.image7_59F6CEA3.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/0601.image7_5F00_59F6CEA3.png"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/2742.image7_thumb_396F8EF1.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/2742.image7_5F00_thumb_5F00_396F8EF1.png" width="330" height="240" /></a>

<font size="2" face="Segoe UI"><strong><font size="3"><u>Solution</u></font></strong>:</font>

<font size="2" face="Segoe UI">There are 2 ways to fix this problem. Before we start off, delete/remove the existing certificate from the store.</font>

  1. <font size="2" face="Segoe UI">If using IIS MMC to import the certificate, then ensure that the “<strong>Allow this certificate to be exported</strong>” is checked.</font>
  2. <font size="2" face="Segoe UI">If making the private key exportable is not an option, then use the <strong>Certificates MMC</strong> to import the certificate. Please go through the following KB on how to import a certificate using the MMC: <a title="http://support.microsoft.com/kb/232137" href="http://support.microsoft.com/kb/232137">http://support.microsoft.com/kb/232137</a></font>

* * *

<p align="center">
  <font size="5" face="Segoe UI"><strong><u>SCENARIO 2</u></strong></font>
</p>

<font size="2" face="Segoe UI">Another reason which can result in a broken keyset is due to missing permissions on the <strong>MachineKeys </strong>folder. This is the location where all the private keys are stored. The folder path (<strong>IIS 7 & higher</strong>) is as shown below: </font><font size="2" face="Segoe UI"><u><strong>C:\ProgramData\Microsoft\Crypto\RSA\MachineKeys</strong></u></font>

<font size="2" face="Segoe UI">The default permissions on this folder are described in the following articles:</font>

[http://support.microsoft.com/kb/278381](http://support.microsoft.com/kb/278381 "http://support.microsoft.com/kb/278381")

[http://msdn.microsoft.com/en-us/library/ee248638(v=vs.100).aspx](http://msdn.microsoft.com/en-us/library/ee248638(v=vs.100).aspx "http://msdn.microsoft.com/en-us/library/ee248638(v=vs.100).aspx")

<font size="2" face="Segoe UI"><strong><font size="3"><u>Solution</u></font></strong>:</font>

<font size="2" face="Segoe UI">Firstly, delete/remove the broken certificate from the store. </font><font size="2" face="Segoe UI">Ensure the permissions are as per the articles mentioned above. So we need to permissions to the Administrators and Everyone account. Do remember to select the </font>

<a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/2047.image_12F25FE1.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/2047.image_5F00_12F25FE1.png"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/7318.image_thumb_7192BA44.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/7318.image_5F00_thumb_5F00_7192BA44.png" width="585" height="441" /></a>

&#160;

<table cellspacing="0" cellpadding="2" width="750" align="center" border="2">
  <tr>
    <td valign="top" width="746">
      <font size="2" face="Segoe UI"><strong>NOTE</strong>: There might be a possibility that the issue might be seen even after ensuring right permissions. In this case, use the <strong>procmon.exe</strong> tool and fix the access denied error on the specific file inside the machinekeys folder. <br />You may also try giving the <strong>System </strong>account <strong>Full Permissions </strong>on the <strong>MachineKeys </strong>folder.</font>
    </td>
  </tr>
</table>

<p align="left">
  <font size="2" face="Segoe UI">After giving the necessary permissions, re-import the certificate as described in <strong>SCENARIO 1</strong>.</font>
</p>

<p align="center">
  <strong><u><font size="1" face="Segoe UI"></font></u></strong>
</p>

* * *

<p align="center">
  <font size="5" face="Segoe UI"><strong><u>SCENARIO 3</u></strong></font>
</p>

<font size="2" face="Segoe UI">There is another possibility, that the issue might occur even after ensuring the both mentioned above. I have observed this behavior typically on <strong>Windows Server 2008</strong>. This depends on the <strong>KeySpec</strong> property of the certificate.</font>

<font size="2" face="Segoe UI">The KeySpec property specifies whether the private key can be used for encryption, or signing, or both.</font>

<font size="2" face="Segoe UI">The following MSDN article describes <strong>KeySpec</strong> property: <br /><a title="http://msdn.microsoft.com/en-us/library/windows/desktop/aa379020%28v=vs.85%29.aspx" href="http://msdn.microsoft.com/en-us/library/windows/desktop/aa379020%28v=vs.85%29.aspx">http://msdn.microsoft.com/en-us/library/windows/desktop/aa379020%28v=vs.85%29.aspx</a></font>

<font size="2" face="Segoe UI">In order to examine the <strong>KeySpec</strong> property of the certificate, use the following command:</font>

<table cellspacing="0" cellpadding="2" width="590" align="center" border="2">
  <tr>
    <td valign="top" width="586">
      <font size="3" face="Courier New"><strong>certutil –v –store my <thumbprint></strong></font>
    </td>
  </tr>
</table>

<font size="2" face="Segoe UI">NOTE: In the above command the thumbprint information can be found in the details tab of the certificate. The following are valid commands:</font>

<font style="background-color: rgb(0, 255, 0);" size="2" face="Courier New">certutil -v -store my "32 b5 39 8e d3 c9 c6 f1 a3 50 bc d4 b5 14 eb b5 a4 5d 1f c6"</font>

<font style="background-color: rgb(0, 255, 0);" face="Courier New">certutil -v -store my "32b5398ed3c9c6f1a350bcd4b514ebb5a45d1fc6"</font>

<font style="background-color: rgb(0, 255, 0);" face="Courier New">certutil -v -store my 32b5398ed3c9c6f1a350bcd4b514ebb5a45d1fc6</font>

<font size="2" face="Segoe UI">Get the output of the above command in a notepad and then search for <strong>KeySpec</strong>, which is part of the <strong>CERT_KEY_PROV_INFO_PROP_ID</strong> section. The <strong>KeySpec</strong> is represented as a hexadecimal value.</font>

<table cellspacing="0" cellpadding="2" width="750" align="center" border="2">
  <tr>
    <td valign="top" width="746">
      <p>
        <font style="background-color: rgb(0, 255, 0);" size="2" face="Courier New"><strong>certutil -v -store my 32b5398ed3c9c6f1a350bcd4b514ebb5a45d1fc6</strong></font>
      </p>
      
      <p>
        <font size="2" face="Courier New">&#8230;</font>
      </p>
      
      <p>
        <font size="2" face="Courier New">&#8230;</font>
      </p>
      
      <p>
        <font size="2" face="Courier New"><strong><font style="background-color: rgb(255, 255, 0);">CERT_KEY_PROV_INFO_PROP_ID(2)</font>:</strong> <br />&#160; Key Container = {00F81886-5F70-430A-939C-BB7DD58ECE2A} <br /> Unique container name: 99247943bd018ca78ef945b82652598d_3ade29bb-f050-41f3-b0db-f2b69957a1d7 <br />&#160; Provider = Microsoft Strong Cryptographic Provider <br />&#160; ProviderType = 1 <br />&#160; Flags = 20 <br /><font style="background-color: rgb(255, 255, 0);">&#160; <strong><font color="#ffffff"><font color="#ff0000">KeySpec = 2 &#8212; AT_SIGNATURE</font></font></strong></font></font>
      </p>
      
      <p>
        <strong><font size="2" face="Courier New">&#8230;</font></strong>
      </p>
    </td>
  </tr>
</table>

<font size="2" face="Segoe UI">As described above it can take three values:</font>

<table class="MsoNormalTable" style="width: 431.2pt; border-collapse: collapse; mso-yfti-tbllook: 1184; mso-padding-alt: 0cm 0cm 0cm 0cm;" cellspacing="0" cellpadding="0" width="618" border="0">
  <tr style="height: 46.35pt; mso-yfti-irow: 0; mso-yfti-firstrow: yes;">
    <td style="background: rgb(68, 114, 196); border-width: 2.25pt 1pt 2.25pt 2.25pt; border-style: solid; border-color: windowtext; padding: 0cm 5.4pt; width: 70.8pt; height: 46.35pt;" width="94">
      <p align="center">
        <b><span style="color: white; line-height: 106%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt;">Numerical <br />Value</span></b><span style="line-height: 106%; font-size: 12pt;"><o:p></o:p></span>
      </p>
    </td>
    
    <td style="background: rgb(68, 114, 196); border-width: 2.25pt 1pt 2.25pt medium; border-style: solid solid solid none; border-color: windowtext windowtext windowtext currentcolor; padding: 0cm 5.4pt; width: 120.3pt; height: 46.35pt;" width="147">
      <p align="center">
        <b><span style="color: white; line-height: 106%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt;"><font size="4">Value</font></span></b><span style="line-height: 106%; font-size: 12pt;"><o:p></o:p></span>
      </p>
    </td>
    
    <td style="background: rgb(68, 114, 196); border-width: 2.25pt 2.25pt 2.25pt medium; border-style: solid solid solid none; border-color: windowtext windowtext windowtext currentcolor; padding: 0cm 5.4pt; width: 240.1pt; height: 46.35pt;" width="375">
      <p align="center">
        <b><span style="color: white; line-height: 106%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt;"><font size="4">Description</font></span></b><span style="line-height: 106%; font-size: 12pt;"><o:p></o:p></span>
      </p>
    </td>
  </tr>
  
  <tr style="height: 63.55pt; mso-yfti-irow: 1;">
    <td style="background: rgb(68, 114, 196); border-width: medium 1pt medium 2.25pt; border-style: none solid; border-color: currentcolor windowtext; padding: 0cm 5.4pt; width: 70.8pt; height: 63.55pt;" width="94">
      <p align="center">
        <b><span style="color: white; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt;"></span></b><span style="font-size: 12pt;"><o:p></o:p></span>
      </p>
    </td>
    
    <td style="background: rgb(216, 216, 216); border-width: medium 1pt medium medium; border-style: none solid none none; border-color: currentcolor windowtext currentcolor currentcolor; padding: 0cm 5.4pt; width: 120.3pt; height: 63.55pt;" width="147">
      <p align="center">
        <b><span lang="EN-IN" style="line-height: 106%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-ansi-language: en-in;">AT_NONE</span></b><span style="line-height: 106%; font-size: 10pt;"><o:p></o:p></span>
      </p>
    </td>
    
    <td style="background: rgb(216, 216, 216); border-width: medium 2.25pt medium medium; border-style: none solid none none; border-color: currentcolor windowtext currentcolor currentcolor; padding: 0cm 5.4pt; width: 240.1pt; height: 63.55pt;" width="375">
      <p class="MsoNormal" style="text-align: center;" align="center">
        <span lang="EN-IN" style="line-height: 106%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-ansi-language: en-in;">The intended use is not identified. This value should be used if the provider is a Cryptography API: Next Generation (CNG) key storage provider (KSP).</span><span style="line-height: 106%; font-size: 10pt;"><o:p></o:p></span>
      </p>
    </td>
  </tr>
  
  <tr style="height: 27.5pt; mso-yfti-irow: 2;">
    <td style="background: rgb(68, 114, 196); border-width: medium 1pt medium 2.25pt; border-style: none solid; border-color: currentcolor windowtext; padding: 0cm 5.4pt; width: 70.8pt; height: 27.5pt;" width="94">
      <p align="center">
        <b><span style="color: white; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt;">1</span></b><span style="font-size: 12pt;"><o:p></o:p></span>
      </p>
    </td>
    
    <td style="border-width: medium 1pt medium medium; border-style: none solid none none; border-color: currentcolor windowtext currentcolor currentcolor; padding: 0cm 5.4pt; width: 120.3pt; height: 27.5pt;" width="147">
      <p align="center">
        <b><span lang="EN-IN" style="line-height: 106%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-ansi-language: en-in;">AT_KEYEXCHANGE</span></b><span style="line-height: 106%; font-size: 10pt;"><o:p></o:p></span>
      </p>
    </td>
    
    <td style="border-width: medium 2.25pt medium medium; border-style: none solid none none; border-color: currentcolor windowtext currentcolor currentcolor; padding: 0cm 5.4pt; width: 240.1pt; height: 27.5pt;" width="375">
      <p class="MsoNormal" style="text-align: center;" align="center">
        <span lang="EN-IN" style="line-height: 106%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-ansi-language: en-in;">The key can be used for encryption or key exchange.</span><span style="line-height: 106%; font-size: 10pt;"><o:p></o:p></span>
      </p>
    </td>
  </tr>
  
  <tr style="height: 27.5pt; mso-yfti-irow: 3; mso-yfti-lastrow: yes;">
    <td style="background: rgb(68, 114, 196); border-width: medium 1pt 2.25pt 2.25pt; border-style: none solid solid; border-color: currentcolor windowtext windowtext; padding: 0cm 5.4pt; width: 70.8pt; height: 27.5pt;" width="94">
      <p align="center">
        <b><span style="color: white; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt;">2</span></b><span style="font-size: 12pt;"><o:p></o:p></span>
      </p>
    </td>
    
    <td style="background: rgb(216, 216, 216); border-width: medium 1pt 2.25pt medium; border-style: none solid solid none; border-color: currentcolor windowtext windowtext currentcolor; padding: 0cm 5.4pt; width: 120.3pt; height: 27.5pt;" width="147">
      <p align="center">
        <b><span lang="EN-IN" style="line-height: 106%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-ansi-language: en-in;">AT_SIGNATURE</span></b><span style="line-height: 106%; font-size: 10pt;"><o:p></o:p></span>
      </p>
    </td>
    
    <td style="background: rgb(216, 216, 216); border-width: medium 2.25pt 2.25pt medium; border-style: none solid solid none; border-color: currentcolor windowtext windowtext currentcolor; padding: 0cm 5.4pt; width: 240.1pt; height: 27.5pt;" width="375">
      <p class="MsoNormal" style="text-align: center;" align="center">
        <span lang="EN-IN" style="line-height: 106%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 10pt; mso-ansi-language: en-in;">The key can be used for signing.</span><span style="line-height: 106%; font-size: 10pt;"><o:p></o:p></span>
      </p>
    </td>
  </tr>
</table>

<font size="2" face="Segoe UI">So the issue is seen if the <strong>KeySpec </strong>value is set to anything other than 1. The issue is more likely to be occur when the <strong>CSR </strong>is generated using a custom template and the <strong>KeySpec</strong> is not specified.</font>

<font size="2" face="Segoe UI"><font style="background-color: rgb(255, 255, 0);">Whenever the <strong>KeySpec </strong>attribute is not explicitly specified, <u>it takes the default value of 2</u> i.e., it can be used for signing purposes only</font>.</font>

<font size="2" face="Segoe UI"><strong><u><font size="3">Solution</font></u></strong>:</font>

<font size="2" face="Segoe UI">So one thing that you need to remember is that the KeySpec attribute has to be specified explicitly.</font>

  1. <font size="2" face="Segoe UI">If you are generating a certificate via the code, then ensure you are explicitly setting the <strong>KeySpec</strong> attribute to 1.</font>
  2. <font size="2" face="Segoe UI">If using <strong>certreq.exe</strong> utility along with an inf file to submit a request to SAN, ensure that you explicitly specify the KeySpec attribute to be 1.</font>
  * <font size="2" face="Segoe UI">Refer the following article for this: <a href="http://support.microsoft.com/kb/931351">http://support.microsoft.com/kb/931351</a></font>

  3. <font size="2" face="Segoe UI">Remember the <strong>KeySpec </strong>attribute is specified while creating the <strong>Certificate Signing Request</strong>. This cannot be modified once the certificate has been issued. So remember to set the value appropriately.</font>
  4. <font size="2" face="Segoe UI">Also compare the <strong>KeySpec</strong> with the <strong>Key Usage</strong> attribute and make sure that both match logically. <br />For example, for a certificate whose <strong>KeySpec</strong> equals to <strong>AT_KEYEXCHANGE, </strong>the <strong>Key Usage </strong>should be <br /><strong>XCN_NCRYPT_ALLOW_DECRYPT_FLAG | XCN_NCRYPT_ALLOW_KEY_AGREEMENT_FLAG.</strong></font>

**<font size="2" face="Segoe UI"></font>**

<font size="2" face="Segoe UI"></font><font size="2" face="Segoe UI"></font><font size="2" face="Segoe UI"></font><font size="2" face="Segoe UI"></font><font size="2" face="Segoe UI"></font><font size="2" face="Segoe UI"></font><font size="2" face="Segoe UI"></font><font size="2" face="Segoe UI"></font><font size="2" face="Segoe UI"></font> 

<table cellspacing="0" cellpadding="2" width="750" align="center" border="2">
  <tr>
    <td valign="top" width="746">
      <p>
        <strong><font size="3" face="Segoe UI">XCN_NCRYPT_ALLOW_USAGES_NONE</font></strong>
      </p>
      
      <dd>
        <p>
          <font size="2" face="Segoe UI">The permitted uses are not defined.</font>
        </p>
      </dd>
    </td>
  </tr>
  
  <tr>
    <td valign="top" width="746">
      <p>
        <strong><font size="3" face="Segoe UI">XCN_NCRYPT_ALLOW_DECRYPT_FLAG</font></strong>
      </p>
      
      <dd>
        <p>
          <font size="2" face="Segoe UI">The key can be used to decrypt content. This maps to the following </font><a href="http://msdn.microsoft.com/en-us/library/windows/desktop/aa379410(v=vs.85).aspx"><strong><font size="2" face="Segoe UI">X509KeyUsageFlags</font></strong></a><font size="2" face="Segoe UI"> values:</font>
        </p>
        
        <ul>
          <li>
            <font size="2" face="Courier New"><strong>XCN_CERT_DATA_ENCIPHERMENT_KEY_USAGE </strong></font>
          </li>
          <li>
            <font size="2" face="Courier New"><strong>XCN_CERT_DECIPHER_ONLY_KEY_USAGE </strong></font>
          </li>
          <li>
            <font size="2" face="Courier New"><strong>XCN_CERT_ENCIPHER_ONLY_KEY_USAGE </strong></font>
          </li>
          <li>
            <font size="2" face="Courier New"><strong>XCN_CERT_KEY_ENCIPHERMENT_KEY_USAGE</strong></font>
          </li>
        </ul>
        
        <p>
          <font size="2" face="Segoe UI"></font></dd> </td> </tr> 
          
          <tr>
            <td valign="top" width="746">
              <p>
                <strong><font size="3" face="Segoe UI">XCN_NCRYPT_ALLOW_SIGNING_FLAG</font></strong>
              </p>
              
              <dd>
                <p>
                  <font size="2" face="Segoe UI">The key can be used for signing. This maps to the following </font><a href="http://msdn.microsoft.com/en-us/library/windows/desktop/aa379410(v=vs.85).aspx"><strong><font size="2" face="Segoe UI">X509KeyUsageFlags</font></strong></a><font size="2" face="Segoe UI"> values:</font>
                </p>
                
                <ul>
                  <li>
                    <font size="2" face="Courier New"><strong>XCN_CERT_CRL_SIGN_KEY_USAGE </strong></font>
                  </li>
                  <li>
                    <font size="2" face="Courier New"><strong>XCN_CERT_DIGITAL_SIGNATURE_KEY_USAGE </strong></font>
                  </li>
                  <li>
                    <font size="2" face="Courier New"><strong>XCN_CERT_KEY_CERT_SIGN_KEY_USAGE</strong></font>
                  </li>
                </ul>
              </dd>
            </td>
          </tr>
          
          <tr>
            <td valign="top" width="746">
              <p>
                <strong><font size="3" face="Segoe UI">XCN_NCRYPT_ALLOW_KEY_AGREEMENT_FLAG</font></strong>
              </p>
              
              <dd>
                <p>
                  <font size="2" face="Segoe UI">The key can be used to establish key agreement between entities.</font>
                </p>
              </dd>
            </td>
          </tr>
          
          <tr>
            <td valign="top" width="746">
              <p>
                <strong><font size="3" face="Segoe UI">XCN_NCRYPT_ALLOW_ALL_USAGES</font></strong>
              </p>
              
              <dd>
                <p>
                  <font size="2" face="Segoe UI">All of the uses defined for this enumeration are permitted.</font>
                </p>
              </dd>
            </td>
          </tr></tbody> </table> 
          
          <p>
            &#160;&#160;&#160;&#160; <u><font face="Segoe UI"><font size="2"><strong> </p> 
            
            <hr />
            More Information</strong>:</font></font></u>&#160;
          </p>
          
          <p>
            <font size="2" face="Segoe UI">For further read on <strong>KeyUsage </strong>refer the below 2 links:</font>
          </p>
          
          <p>
            <a title="http://msdn.microsoft.com/en-us/library/windows/desktop/aa379021%28v=vs.85%29.aspx" href="http://msdn.microsoft.com/en-us/library/windows/desktop/aa379021%28v=vs.85%29.aspx"><font size="2" face="Segoe UI">http://msdn.microsoft.com/en-us/library/windows/desktop/aa379021%28v=vs.85%29.aspx</font></a> <br /><a title="http://msdn.microsoft.com/en-us/library/windows/desktop/aa379417%28v=vs.85%29.aspx" href="http://msdn.microsoft.com/en-us/library/windows/desktop/aa379417%28v=vs.85%29.aspx"><font size="2" face="Segoe UI">http://msdn.microsoft.com/en-us/library/windows/desktop/aa379417%28v=vs.85%29.aspx</font></a>
          </p>
          
          <p>
            <font face="Segoe UI"><font size="2"><strong>Configuring and Troubleshooting Certificate Services Client–Credential Roaming</strong>: </font></font><a title="http://technet.microsoft.com/en-us/library/dd277392.aspx" href="http://technet.microsoft.com/en-us/library/dd277392.aspx"><font size="2" face="Segoe UI">http://technet.microsoft.com/en-us/library/dd277392.aspx</font></a>
          </p>
          
          <p>
            <font size="2" face="Segoe UI"><strong>How to create a certificate request with CertEnroll (JavaScript): </strong></font><a title="http://blogs.msdn.com/b/alejacma/archive/2009/01/28/how-to-create-a-certificate-request-with-certenroll-javascript.aspx" href="http://blogs.msdn.com/b/alejacma/archive/2009/01/28/how-to-create-a-certificate-request-with-certenroll-javascript.aspx"><font size="2" face="Segoe UI"></font></a><font size="2" face="Segoe UI"><a href="http://blogs.msdn.com/b/alejacma/archive/2009/01/28/how-to-create-a-certificate-request-with-certenroll-javascript.aspx">http://blogs.msdn.com/b/alejacma/archive/2009/01/28/how-to-create-a-certificate-request-with-certenroll-javascript.aspx</a></font>
          </p>
          
          <p>
            <font face="Segoe UI"><strong><font size="2">Generating a certificate (self-signed) using PowerShell and CertEnroll interfaces: </font></strong><a></a><a title="http://blogs.technet.com/b/vishalagarwal/archive/2009/08/22/generating-a-certificate-self-signed-using-powershell-and-certenroll-interfaces.aspx" href="http://blogs.technet.com/b/vishalagarwal/archive/2009/08/22/generating-a-certificate-self-signed-using-powershell-and-certenroll-interfaces.aspx"><font size="2">http://blogs.technet.com/b/vishalagarwal/archive/2009/08/22/generating-a-certificate-self-signed-using-powershell-and-certenroll-interfaces.aspx</font></a></font>
          </p>
          
          <p>
            <font size="2" face="Segoe UI">Hope this helps. <img class="wlEmoticon wlEmoticon-smile" alt="Smile" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6811.wlEmoticon-smile_5679EB36.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/6811.wlEmoticon_2D00_smile_5F00_5679EB36.png" /></font>
          </p>