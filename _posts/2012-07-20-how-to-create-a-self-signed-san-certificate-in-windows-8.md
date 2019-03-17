---
id: 87
title: How to create a Self-Signed SAN Certificate in Windows 8
date: 2012-07-20T01:36:00+00:00
author: kaushal
layout: post
guid: https://blogs.msdn.microsoft.com/kaushal/2012/07/20/how-to-create-a-self-signed-san-certificate-in-windows-8/
permalink: /2012/07/20/how-to-create-a-self-signed-san-certificate-in-windows-8/
orig_url:
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2012/07/20/how-to-create-a-self-signed-san-certificate-in-windows-8.aspx
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2012/07/20/how-to-create-a-self-signed-san-certificate-in-windows-8.aspx
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2012/07/20/how-to-create-a-self-signed-san-certificate-in-windows-8.aspx
orig_site_id:
  - "13803"
  - "13803"
  - "13803"
orig_post_id:
  - "10331892"
  - "10331892"
  - "10331892"
orig_parent_id:
  - "10331892"
  - "10331892"
  - "10331892"
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
  - http://blogs.msdn.com/b/kaushal/archive/2012/07/20/how-to-create-a-self-signed-san-certificate-in-windows-8.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2012/07/20/how-to-create-a-self-signed-san-certificate-in-windows-8.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2012/07/20/how-to-create-a-self-signed-san-certificate-in-windows-8.aspx
orig_post_name:
  - how to create a self signed san certificate in windows 8
  - how to create a self signed san certificate in windows 8
  - how to create a self signed san certificate in windows 8
orig_thread_id:
  - "815266"
  - "815266"
  - "815266"
orig_post_author_email:
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
orig_attachment_count:
  - "0"
  - "0"
  - "0"
total_views:
  - "20978"
  - "20978"
  - "20978"
opengraph_tags:
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="How to create a Self-Signed SAN Certificate in Windows 8" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/07/20/how-to-create-a-self-signed-san-certificate-in-windows-8/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="One of the cool features of Windows 8 is the improved set of PowerShell commandlets that have been shipped with it. There are several of them which could have made the task a lot easier for the server admins. In here I will be discussing about one of the commandlets using which we can create..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3582.image_thumb_6E0BE240.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="How to create a Self-Signed SAN Certificate in Windows 8" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/07/20/how-to-create-a-self-signed-san-certificate-in-windows-8/" />
    <meta name="twitter:description" content="One of the cool features of Windows 8 is the improved set of PowerShell commandlets that have been shipped with it. There are several of them which could have made the task a lot easier for the server admins. In here I will be discussing about one of the commandlets using which we can create..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3582.image_thumb_6E0BE240.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="How to create a Self-Signed SAN Certificate in Windows 8" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/07/20/how-to-create-a-self-signed-san-certificate-in-windows-8/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="One of the cool features of Windows 8 is the improved set of PowerShell commandlets that have been shipped with it. There are several of them which could have made the task a lot easier for the server admins. In here I will be discussing about one of the commandlets using which we can create..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3582.image_thumb_6E0BE240.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="How to create a Self-Signed SAN Certificate in Windows 8" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/07/20/how-to-create-a-self-signed-san-certificate-in-windows-8/" />
    <meta name="twitter:description" content="One of the cool features of Windows 8 is the improved set of PowerShell commandlets that have been shipped with it. There are several of them which could have made the task a lot easier for the server admins. In here I will be discussing about one of the commandlets using which we can create..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3582.image_thumb_6E0BE240.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="How to create a Self-Signed SAN Certificate in Windows 8" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/07/20/how-to-create-a-self-signed-san-certificate-in-windows-8/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="One of the cool features of Windows 8 is the improved set of PowerShell commandlets that have been shipped with it. There are several of them which could have made the task a lot easier for the server admins. In here I will be discussing about one of the commandlets using which we can create..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3582.image_thumb_6E0BE240.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="How to create a Self-Signed SAN Certificate in Windows 8" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/07/20/how-to-create-a-self-signed-san-certificate-in-windows-8/" />
    <meta name="twitter:description" content="One of the cool features of Windows 8 is the improved set of PowerShell commandlets that have been shipped with it. There are several of them which could have made the task a lot easier for the server admins. In here I will be discussing about one of the commandlets using which we can create..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3582.image_thumb_6E0BE240.png" />
    
categories:
  - Uncategorized
tags:
  - New-SelfSignedCertificate
  - PowerShell
  - SAN
  - SAN Certificate
  - Self-Signed
  - Windows 8
---
<span style="font-family: segoe ui; font-size: x-small;"><font size="2">One of the cool features of Windows 8 is the improved set of PowerShell commandlets that have been shipped with it. There are several of them which could have made the task a lot easier for the server admins.</font></span>

<font size="2"></font> 

<span style="font-family: segoe ui; font-size: x-small;"><font size="2">In here I will be discussing about one of the commandlets using which we can create a self-signed SSL Certificate. Yes, I mean self-signed and a SAN Certificate.</font></span>

<font size="2"></font> 

<span style="font-family: segoe ui; font-size: x-small;"><font size="2">What you also need to know is that there are no lengthy procedures, it is a simple command with few parameters which adds to the simplicity.</font></span>

<font size="2"></font> 

<span style="font-family: segoe ui; font-size: x-small;"><font size="2">So here are few pre-requisites that I could think of,</font></span>

<font size="2"></font> 

<font size="2"></font> </p> 

  * <span style="font-family: segoe ui; font-size: x-small;"><font size="2">Windows PowerShell and PowerShell ISE needs to be installed.</font></span>
<font size="2"></font> 

  * <span style="font-family: segoe ui; font-size: x-small;"><font size="2">OS is either Windows Server 2012 or Windows 8. (I’m not aware if this cmdlet has been back-ported to previous OS versions, I hope they do)</font></span>
<font size="2"></font> 

  * <span style="font-family: segoe ui; font-size: x-small;"><font size="2">The Windows PowerShell help menu is updated (Well this is not a necessity, but it will help if this is done.)</font></span>
<font size="2"></font></ul> 

<font size="2"></font> 

<span style="font-family: segoe ui;"><span style="font-size: x-small;"><font size="2"><strong>Commandlet Name</strong>: <span style="background-color: rgb(255, 255, 0);">New-SelfSignedCertificate</span></font></span></span>

<font size="2"></font> 

<span style="font-family: segoe ui;"><span style="font-size: x-small;"><font size="2"><strong><span style="text-decoration: underline;">Syntax</span></strong>:</font></span></span>

<font size="2"></font> 

<span style="font-family: courier new; font-size: x-small; background-color: rgb(255, 255, 0);"><strong><font size="2" face="Segoe UI">New-SelfSignedCertificate [-CertStoreLocation <String>] [-CloneCert <Certificate>] [-DnsName <String>] [-Confirm <SwitchParameter>] [-WhatIf <SwitchParameter>] [<CommonParameters>]</font></strong></span>

<p align="center">
  <strong><span style="font-family: segoe ui; font-size: large;"><font size="5">Scenario</font></span></strong>
</p>

<span style="font-family: segoe ui; font-size: x-small;"><font size="2">Consider you need to create a self-signed SAN certificate for the following hostnames:</font></span>

<font size="2"></font> 

<font size="2"></font> </p> 

  * [<span style="font-family: segoe ui; font-size: x-small;"><font size="2">www.test.com</font></span>](http://www.test.com)
<font size="2"></font> 

  * [<span style="font-family: segoe ui; font-size: x-small;"><font size="2">www.test.edu</font></span>](http://www.test.edu)
<font size="2"></font> 

  * [<span style="font-family: segoe ui; font-size: x-small;"><font size="2">www.test.testing.com</font></span>](http://www.test.testing.com)
<font size="2"></font></ul> 

<font size="2"></font> 

<span style="font-family: segoe ui; font-size: x-small;"><font size="2">Using the above commandlet the cert can be issued and automatically placed in the personal store of My Computer Account.</font></span>

<font size="2"></font> 

<span style="font-family: segoe ui; font-size: x-small;"><font size="2">Here is the command that we need to execute to generate the cert.</font></span>

<table style="margin-right: auto; margin-left: auto;" cellspacing="0" cellpadding="0" width="750" border="2">
  <tr>
    <td bgcolor="#003399" valign="top" width="746">
      <p>
        <span style="font-family: courier new;"><span style="color: rgb(255, 255, 255);"><font size="3">PS C:\><font style="background-color: rgb(255, 255, 0);" color="#000000"> New-SelfSignedCertificate -DnsName www.test.com, www.test.edu, www.test.testing.com -CertStoreLocation cert:\LocalMachine\My</font></font></span></span>
      </p>
      
      <p>
        <font size="3" face="Courier New"></font>
      </p>
      
      <p>
        <span style="color: rgb(255, 255, 255); font-family: courier new;"><font size="3">Directory: Microsoft.PowerShell.Security\Certificate::LocalMachine\My</font></span>
      </p>
      
      <p>
        <font size="3" face="Courier New"></font>
      </p>
      
      <p>
        &#160;
      </p>
      
      <p>
        <font size="3" face="Courier New"></font>
      </p>
      
      <p>
        <span style="color: rgb(255, 255, 255); font-family: courier new;"><font size="3">Thumbprint&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; Subject </font></span>
      </p>
      
      <p>
        <font size="3" face="Courier New"></font>
      </p>
      
      <p>
        <span style="color: rgb(255, 255, 255); font-family: courier new;"><font size="3">&#8212;&#8212;&#8212;-&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; &#8212;&#8212;- </font></span>
      </p>
      
      <p>
        <font size="3" face="Courier New"></font>
      </p>
      
      <p>
        <span style="font-family: segoe ui;"><span style="color: rgb(255, 255, 255); font-family: courier new;"><font size="3">7020CC054B5818262ECF6C7D9BB2E2546D2B4FD8 CN=www.test.com</font></span> </span>
      </p>
    </td>
  </tr>
</table>

<span style="font-family: segoe ui; font-size: x-small;"><font size="2">This will install the self-signed cert in the Personal store of machine account.</font></span>

<font size="2"></font> 

<span style="font-family: segoe ui; font-size: x-small;"><span style="background-color: rgb(255, 255, 0);"><font size="2"><strong>Note</strong>: Certificate wouldn’t be trusted. Place the certificate in the Trusted Root CA store and the error will go away.</font></span></span>

<font size="2"></font> 

<span style="font-family: segoe ui; font-size: x-small;"><font size="2">So this is what the certificate looks like:</font></span>

<p style="text-align: center;">
  <a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4667.image_3B1C51D9.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/4667.image_5F00_3B1C51D9.png"><img title="image" style="display: inline;" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3582.image_thumb_6E0BE240.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/3582.image_5F00_thumb_5F00_6E0BE240.png" width="295" height="370" /></a>&#160;<a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/7801.image_56FD6104.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/7801.image_5F00_56FD6104.png"><img title="image" style="display: inline;" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3000.image_thumb_09ECF16C.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/3000.image_5F00_thumb_5F00_09ECF16C.png" width="297" height="370" /></a>
</p>

<span style="font-family: segoe ui; font-size: x-small;"><font size="2">It can’t get easier than this. </font></span>

<font size="2"></font> 

<span style="font-family: segoe ui; font-size: x-small;"><font size="2">Another thing worthwhile mentioning is the help menu, which is <strong><em>very</em></strong> descriptive. I have pasted the entire help menu content for the above commandlet below</font></span>

<font size="2"></font> 

<span style="font-family: segoe ui; font-size: x-small;"><font size="2">The good thing is that it also provides descriptive examples.</font></span>

<table style="margin-right: auto; margin-left: auto;" cellspacing="0" cellpadding="0" border="1">
  <tr>
    <td valign="top" width="765">
      <p align="center">
        <span style="font-family: segoe ui; font-size: medium;"><strong><font size="4">New-SelfSignedCertificate Help</font></strong></span>
      </p>
    </td>
  </tr>
  
  <tr>
    <td valign="top" width="765">
      <p>
        <span style="font-family: segoe ui;"><span style="font-size: x-small;"><strong><span style="text-decoration: underline;"><font size="2">Description</font></span></strong></span></span>
      </p>
      
      <p>
        <font size="2"></font>
      </p>
      
      <p>
        <span style="font-family: segoe ui; font-size: x-small;"><font size="2">&#160;&#160;&#160;&#160;&#160;&#160;&#160; The New-SelfSignedCertificate cmdlet creates a self-signed certificate for testing purposes. Using the <strong>CloneCert</strong> parameter, a test certificate can be created based on an existing certificate with all settings copied from the original certificate except for the public key. A new key of the same algorithm and length will be created.</font></span>
      </p>
      
      <p>
        <font size="2"></font>
      </p>
      
      <p>
        <span style="font-family: segoe ui; font-size: x-small;"><font size="2">&#160;&#160;&#160;&#160;&#160;&#160;&#160; If an existing certificate is not being cloned, then an SSL server certificate with the following default settings is created:</font></span>
      </p>
      
      <p>
        <font size="2"></font>
      </p>
      
      <ul>
        <font size="2"></font> </p> 
        
        <li>
          <span style="font-family: segoe ui; font-size: x-small;"><font size="2"><strong>Subject</strong>:&#160;&#160; Empty</font></span>
        </li>
        <p>
          <font size="2"></font>
        </p>
        
        <li>
          <span style="font-family: segoe ui; font-size: x-small;"><font size="2"><strong>Key</strong>:&#160;&#160; RSA 2048</font></span>
        </li>
        <p>
          <font size="2"></font>
        </p>
        
        <li>
          <span style="font-family: segoe ui; font-size: x-small;"><font size="2"><strong>EKUs</strong>:&#160;&#160; Client Authentication and Server Authentication</font></span>
        </li>
        <p>
          <font size="2"></font>
        </p>
        
        <li>
          <span style="font-family: segoe ui; font-size: x-small;"><font size="2"><strong>Key Usage</strong>:&#160;&#160; Digital Signature, Key Encipherment (a0)</font></span>
        </li>
        <p>
          <font size="2"></font>
        </p>
        
        <li>
          <span style="font-family: segoe ui; font-size: x-small;"><font size="2"><strong>Validity</strong> <strong>Period</strong>:&#160;&#160; One year</font></span>
        </li>
        <p>
          <font size="2"></font></ul> 
          
          <p>
            <font size="2"></font>
          </p>
          
          <p>
            <span style="font-family: segoe ui; font-size: x-small;"><font size="2">Delegation may be required when using this cmdlet with Windows PowerShell® remoting and changing user configuration.</font></span>
          </p>
          
          <p>
            <font size="2"></font>
          </p>
          
          <p>
            <span style="font-family: segoe ui;"><span style="font-size: x-small;"><strong><span style="text-decoration: underline;"><font size="2">Parameters</font></span></strong></span></span>
          </p>
          
          <p>
            <font size="2"></font>
          </p>
          
          <p>
            <span style="font-family: segoe ui; font-size: x-small;"><font size="2">&#8211;<strong>CertStoreLocation</strong> <String></font></span>
          </p>
          
          <p>
            <font size="2"></font>
          </p>
          
          <p>
            <span style="font-family: segoe ui; font-size: x-small;"><font size="2">&#160;&#160;&#160;&#160;&#160;&#160;&#160; Specifies the certificate store in which a new certificate will be stored. The current path is the default value.</font></span>
          </p>
          
          <p>
            <font size="2"></font>
          </p>
          
          <ul>
            <font size="2"></font> </p> 
            
            <li>
              <span style="font-family: segoe ui; font-size: x-small;"><font size="2">Required? False</font></span>
            </li>
            <p>
              <font size="2"></font>
            </p>
            
            <li>
              <span style="font-family: segoe ui; font-size: x-small;"><font size="2">Position? Named</font></span>
            </li>
            <p>
              <font size="2"></font>
            </p>
            
            <li>
              <span style="font-family: segoe ui; font-size: x-small;"><font size="2">Default value <strong>. </strong></font></span>
            </li>
            <p>
              <font size="2"></font>
            </p>
            
            <li>
              <span style="font-family: segoe ui; font-size: x-small;"><font size="2">Accept pipeline input? False</font></span>
            </li>
            <p>
              <font size="2"></font>
            </p>
            
            <li>
              <span style="font-family: segoe ui; font-size: x-small;"><font size="2">Accept wildcard characters? False</font></span>
            </li>
            <p>
              <font size="2"></font></ul> 
              
              <p>
                <font size="2"></font>
              </p>
              
              <p>
                <span style="font-family: segoe ui; font-size: x-small;"><font size="2">&#8211;<strong>CloneCert</strong> <Certificate></font></span>
              </p>
              
              <p>
                <font size="2">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; I<span style="font-family: segoe ui; font-size: x-small;">dentifies the certificate to copy when creating a new certificate. The certificate being cloned can be identified by an X509 certificate or the file path in the certificate provider. When this parameter is used, all fields and extensions of the certificate will be inherited except the public key (a new key of the same algorithm and length will be created) and the <strong>NotAfter</strong> and <strong>NotBefore</strong> fields (the validity period for the <strong>NotBefore</strong> field is set to ten minutes in the past).</span> </font>
              </p>
              
              <ul>
                <font size="2"></font> </p> 
                
                <li>
                  <span style="font-family: segoe ui; font-size: x-small;"><font size="2">Required? False</font></span>
                </li>
                <p>
                  <font size="2"></font>
                </p>
                
                <li>
                  <span style="font-family: segoe ui; font-size: x-small;"><font size="2">Position? Named</font></span>
                </li>
                <p>
                  <font size="2"></font>
                </p>
                
                <li>
                  <span style="font-family: segoe ui; font-size: x-small;"><font size="2">Default value </font></span>
                </li>
                <p>
                  <font size="2"></font>
                </p>
                
                <li>
                  <span style="font-family: segoe ui; font-size: x-small;"><font size="2">Accept pipeline input? true (ByValue)</font></span>
                </li>
                <p>
                  <font size="2"></font>
                </p>
                
                <li>
                  <span style="font-family: segoe ui; font-size: x-small;"><font size="2">Accept wildcard characters? False</font></span>
                </li>
                <p>
                  <font size="2"></font></ul> 
                  
                  <p>
                    <font size="2"></font>
                  </p>
                  
                  <p>
                    <span style="font-family: segoe ui;"><span style="font-size: x-small;"><font size="2"><strong>-DnsName</strong> <String></font></span></span>
                  </p>
                  
                  <p>
                    <font size="2"></font>
                  </p>
                  
                  <p>
                    <font size="2">&#160;&#160;&#160;&#160;&#160;&#160;&#160; <span style="font-family: segoe ui; font-size: x-small;">Specifies one or more DNS names to put into the Subject Alternative Name extension of the certificate when a certificate to be copied is not specified via the CloneCert parameter. The first DNS name is also saved as Subject Name and Issuer Name.</span></font>
                  </p>
                  
                  <p>
                    <font size="2"></font>
                  </p>
                  
                  <ul>
                    <font size="2"></font> </p> 
                    
                    <li>
                      <span style="font-family: courier new; font-size: x-small;"><font size="2" face="Segoe UI">Required? False</font></span>
                    </li>
                    <p>
                      <font size="2"></font>
                    </p>
                    
                    <li>
                      <span style="font-family: courier new; font-size: x-small;"><font size="2" face="Segoe UI">Position? Named</font></span>
                    </li>
                    <p>
                      <font size="2"></font>
                    </p>
                    
                    <li>
                      <span style="font-family: courier new; font-size: x-small;"><font size="2" face="Segoe UI">Default value </font></span>
                    </li>
                    <p>
                      <font size="2"></font>
                    </p>
                    
                    <li>
                      <span style="font-family: courier new; font-size: x-small;"><font size="2" face="Segoe UI">Accept pipeline input? False</font></span>
                    </li>
                    <p>
                      <font size="2"></font>
                    </p>
                    
                    <li>
                      <span style="font-family: courier new; font-size: x-small;"><font size="2" face="Segoe UI">Accept wildcard characters? False</font></span>
                    </li>
                    <p>
                      <font size="2"></font></ul> 
                      
                      <p>
                        <font size="2"></font>
                      </p>
                      
                      <p>
                        <span style="font-family: segoe ui; font-size: x-small;"><font size="2">&#8211;<strong>Confirm</strong> <SwitchParameter></font></span>
                      </p>
                      
                      <p>
                        <font size="2"></font>
                      </p>
                      
                      <p>
                        <font size="2">&#160;&#160;&#160;&#160;&#160;&#160;&#160; <span style="font-family: segoe ui; font-size: x-small;">Prompts you for confirmation before running the cmdlet. </span></font>
                      </p>
                      
                      <p>
                        <font size="2"></font>
                      </p>
                      
                      <ul>
                        <font size="2"></font> </p> 
                        
                        <li>
                          <span style="font-family: segoe ui; font-size: x-small;"><font size="2">Required? False</font></span>
                        </li>
                        <p>
                          <font size="2"></font>
                        </p>
                        
                        <li>
                          <span style="font-family: segoe ui; font-size: x-small;"><font size="2">Position? Named</font></span>
                        </li>
                        <p>
                          <font size="2"></font>
                        </p>
                        
                        <li>
                          <span style="font-family: segoe ui; font-size: x-small;"><font size="2">Default value </font></span>
                        </li>
                        <p>
                          <font size="2"></font>
                        </p>
                        
                        <li>
                          <span style="font-family: segoe ui; font-size: x-small;"><font size="2">Accept pipeline input? False</font></span>
                        </li>
                        <p>
                          <font size="2"></font>
                        </p>
                        
                        <li>
                          <span style="font-family: segoe ui; font-size: x-small;"><font size="2">Accept wildcard characters? False</font></span>
                        </li>
                        <p>
                          <font size="2"></font></ul> 
                          
                          <p>
                            <font size="2"></font>
                          </p>
                          
                          <p>
                            <span style="font-family: segoe ui; font-size: x-small;"><font size="2">&#8211;<strong>WhatIf</strong> <SwitchParameter></font></span>
                          </p>
                          
                          <p>
                            <font size="2"></font>
                          </p>
                          
                          <p>
                            <font size="2">&#160;&#160;&#160;&#160;&#160;&#160;&#160; <span style="font-family: segoe ui; font-size: x-small;">Shows what would happen if the cmdlet runs. The cmdlet is not run.</span></font>
                          </p>
                          
                          <p>
                            <font size="2"></font>
                          </p>
                          
                          <ul>
                            <font size="2"></font> </p> 
                            
                            <li>
                              <span style="font-family: segoe ui; font-size: x-small;"><font size="2">Required? False</font></span>
                            </li>
                            <p>
                              <font size="2"></font>
                            </p>
                            
                            <li>
                              <span style="font-family: segoe ui; font-size: x-small;"><font size="2">Position? Named</font></span>
                            </li>
                            <p>
                              <font size="2"></font>
                            </p>
                            
                            <li>
                              <span style="font-family: segoe ui; font-size: x-small;"><font size="2">Default value </font></span>
                            </li>
                            <p>
                              <font size="2"></font>
                            </p>
                            
                            <li>
                              <span style="font-family: segoe ui; font-size: x-small;"><font size="2">Accept pipeline input? False</font></span>
                            </li>
                            <p>
                              <font size="2"></font>
                            </p>
                            
                            <li>
                              <span style="font-family: segoe ui; font-size: x-small;"><font size="2">Accept wildcard characters? False</font></span>
                            </li>
                            <p>
                              <font size="2"></font></ul> 
                              
                              <p>
                                <font size="2"><strong><span style="font-family: segoe ui; font-size: x-small;">Inputs</span></strong> </font>
                              </p>
                              
                              <p>
                                <span style="font-family: courier new; font-size: x-small;"><font size="2" face="Segoe UI"> Microsoft.CertificateServices.Commands.Certificate</font></span>
                              </p>
                              
                              <p>
                                <font size="2"></font>
                              </p>
                              
                              <p>
                                <span style="font-family: segoe ui; font-size: x-small;"><font size="2"> The Certificate object can either be provided as a Path object to a certificate or an X509Certificate2 object.</font></span>
                              </p>
                              
                              <p>
                                <font size="2"></font>
                              </p>
                              
                              <p>
                                <strong><span style="font-family: segoe ui; font-size: x-small;"><font size="2">Outputs</font></span></strong>
                              </p>
                              
                              <p>
                                <font size="2"></font>
                              </p>
                              
                              <p>
                                <span style="font-family: courier new; font-size: x-small;"><font size="2" face="Segoe UI"> System.Security.Cryptography.X509Certificates.X509Certificate2</font></span>
                              </p>
                              
                              <p>
                                <font size="2"></font>
                              </p>
                              
                              <p>
                                <span style="font-family: segoe ui; font-size: x-small;"><font size="2"> An X509Certificate2 object for the certificate that has been created</font>.</span>
                              </p></td> </tr> </tbody> </table>