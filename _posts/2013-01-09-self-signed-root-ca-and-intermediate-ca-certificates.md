---
id: 162
title: Self-Signed, Root CA and Intermediate CA Certificates
date: 2013-01-09T13:58:57+00:00
author: kaushal
layout: post
guid: https://blogs.msdn.microsoft.com/kaushal/2013/01/09/self-signed-root-ca-and-intermediate-ca-certificates/
permalink: /2013/01/09/self-signed-root-ca-and-intermediate-ca-certificates/
orig_url:
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2013/01/10/self-signed-root-ca-and-intermediate-ca-certificates.aspx
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2013/01/10/self-signed-root-ca-and-intermediate-ca-certificates.aspx
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2013/01/10/self-signed-root-ca-and-intermediate-ca-certificates.aspx
orig_site_id:
  - "13803"
  - "13803"
  - "13803"
orig_post_id:
  - "10383618"
  - "10383618"
  - "10383618"
orig_parent_id:
  - "10383618"
  - "10383618"
  - "10383618"
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
  - http://blogs.msdn.com/b/kaushal/archive/2013/01/09/self-signed-root-ca-and-intermediate-ca-certificates.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2013/01/09/self-signed-root-ca-and-intermediate-ca-certificates.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2013/01/09/self-signed-root-ca-and-intermediate-ca-certificates.aspx
orig_post_name:
  - self signed root ca and intermediate ca certificates
  - self signed root ca and intermediate ca certificates
  - self signed root ca and intermediate ca certificates
orig_thread_id:
  - "831617"
  - "831617"
  - "831617"
orig_post_author_email:
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
orig_attachment_count:
  - "0"
  - "0"
  - "0"
total_views:
  - "16470"
  - "16470"
  - "16470"
opengraph_tags:
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Self-Signed, Root CA and Intermediate CA Certificates" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2013/01/09/self-signed-root-ca-and-intermediate-ca-certificates/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="In this article I will be discussing about the following: Self-Signed Certificate Root CA Certificate Intermediate CA Certificate At the end I would like everyone to be able to differentiate between these certificate types. Self Signed Certificate Self Signed Certificates are certs where both the Issued To and the Issued By field of the certificates..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6318.image_thumb_39624BFA.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Self-Signed, Root CA and Intermediate CA Certificates" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2013/01/09/self-signed-root-ca-and-intermediate-ca-certificates/" />
    <meta name="twitter:description" content="In this article I will be discussing about the following: Self-Signed Certificate Root CA Certificate Intermediate CA Certificate At the end I would like everyone to be able to differentiate between these certificate types. Self Signed Certificate Self Signed Certificates are certs where both the Issued To and the Issued By field of the certificates..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6318.image_thumb_39624BFA.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Self-Signed, Root CA and Intermediate CA Certificates" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2013/01/09/self-signed-root-ca-and-intermediate-ca-certificates/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="In this article I will be discussing about the following: Self-Signed Certificate Root CA Certificate Intermediate CA Certificate At the end I would like everyone to be able to differentiate between these certificate types. Self Signed Certificate Self Signed Certificates are certs where both the Issued To and the Issued By field of the certificates..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6318.image_thumb_39624BFA.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Self-Signed, Root CA and Intermediate CA Certificates" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2013/01/09/self-signed-root-ca-and-intermediate-ca-certificates/" />
    <meta name="twitter:description" content="In this article I will be discussing about the following: Self-Signed Certificate Root CA Certificate Intermediate CA Certificate At the end I would like everyone to be able to differentiate between these certificate types. Self Signed Certificate Self Signed Certificates are certs where both the Issued To and the Issued By field of the certificates..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6318.image_thumb_39624BFA.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Self-Signed, Root CA and Intermediate CA Certificates" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2013/01/09/self-signed-root-ca-and-intermediate-ca-certificates/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="In this article I will be discussing about the following: Self-Signed Certificate Root CA Certificate Intermediate CA Certificate At the end I would like everyone to be able to differentiate between these certificate types. Self Signed Certificate Self Signed Certificates are certs where both the Issued To and the Issued By field of the certificates..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6318.image_thumb_39624BFA.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Self-Signed, Root CA and Intermediate CA Certificates" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2013/01/09/self-signed-root-ca-and-intermediate-ca-certificates/" />
    <meta name="twitter:description" content="In this article I will be discussing about the following: Self-Signed Certificate Root CA Certificate Intermediate CA Certificate At the end I would like everyone to be able to differentiate between these certificate types. Self Signed Certificate Self Signed Certificates are certs where both the Issued To and the Issued By field of the certificates..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6318.image_thumb_39624BFA.png" />
    
categories:
  - Uncategorized
---
<font size="2" face="Segoe UI">In this article I will be discussing about the following:</font>

  * <font size="2" face="Segoe UI">Self-Signed Certificate</font>
  * <font size="2" face="Segoe UI">Root CA Certificate</font>
  * <font size="2" face="Segoe UI">Intermediate CA Certificate</font>

At the end I would like everyone to be able to differentiate between these certificate types.

<font size="5" face="Segoe UI"><strong><u>Self Signed Certificate</u></strong></font>

<font size="2" face="Segoe UI">Self Signed Certificates are certs where both the <strong>Issued To </strong>and the <strong>Issued By </strong>field of the certificates are same. In simple words it is a certificate where one issues a certificate to itself and hence the name <strong>Self Signed Certificate</strong>. Here is one example:</font>

<a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/1145.image_6FB37409.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/1145.image_5F00_6FB37409.png"><img title="image" style="border-top: 0px; border-right: 0px; background-image: none; border-bottom: 0px; float: none; padding-top: 0px; padding-left: 0px; margin-left: auto; border-left: 0px; display: block; padding-right: 0px; margin-right: auto" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6318.image_thumb_39624BFA.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/6318.image_5F00_thumb_5F00_39624BFA.png" width="398" height="494" /></a>

<font size="2" face="Segoe UI">As seen in the above image the <strong>Issued to</strong> and <strong>Issued by </strong>are same. You may also observe the warning indicating that the certificate is not trusted. Of course it is not as it is self-signed, none of the Known Public CA’s have issued this, so it wont be trusted. </font>

   <font size="2" face="Segoe UI"></p> 

<table cellspacing="0" cellpadding="2" width="420" align="center" bgcolor="#778899" border="2">
  <tr>
    <td valign="top" width="416">
      <p>
        <font size="2" face="Segoe UI"><strong>NOTE</strong>: To get past the above error put the cert in the Root CA store.</font>&#160;
      </p>
    </td>
  </tr>
</table>

<p>
  These certs come in handy as they can be created easily using several tools. Obtaining a certificate from a noted Certification Authority has a cost associated with it and may not be feasible at all times. Developers typically test their applications using a self signed certificates most of the times.
</p>

<p>
  <strong><u><font size="5">Root CA Certificate</font></u></strong>
</p>

<p>
  <strong>Root CA </strong>Certificate is a <strong>CA </strong>Certificate which is simply a <strong>Self-signed Certificate</strong>. This certificate represents a entity which issues certificate and is known as <strong>Certificate Authority </strong>or the <strong>CA</strong>. The usage of the certificate distinguishes it with other normal certificates. Now a CA can be classified as either <strong>Root CA’s</strong> or <strong>Intermediate CA’s</strong>. On a <strong>Windows OS</strong>, if you are looking at the certificate store, you would see all the Root CA certificates in the <strong>Trusted Root Certification Authorities</strong>. This by default includes the list of public root CA’s which are installed with Windows and are updated periodically through Windows Updates. The number of the certificates would be lesser.
</p>

<p>
  <font size="2" face="Segoe UI"> </p> 
  
  <table cellspacing="0" cellpadding="2" width="420" align="center" bgcolor="#778899" border="2">
    <tr>
      <td valign="top" width="416">
        <p>
          <font size="2" face="Segoe UI"><strong>NOTE</strong>: <font style="background-color: #ffff00">Don’t add Intermediate CA certificates to the Trusted Root Certification Authorities store.</font></font>
        </p>
      </td>
    </tr>
  </table>
  
  <p>
    </font>
  </p>
  
  <p>
    <strong><u>Identification of a Root CA:</u></strong>
  </p>
  
  <p>
    Now how do we differentiate the CA certificates as <strong>Root CA</strong> or <strong>Intermediate CA</strong>. There is so much fuss around this. Its actually easy, look at the CA cert. If the <strong>Issued to</strong> and <strong>Issued by </strong>are same then it is a <strong>Root CA </strong>or else it is a <strong>Intermediate CA</strong>. Another identification would be to look at the <strong>Certification Path</strong>. The Cert which appears at the top of the list is the <strong>Root CA</strong>. Below is one example of one of the public root CA’s:
  </p>
  
  <p>
    <a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/5736.image_5E7F9666.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/5736.image_5F00_5E7F9666.png"><img title="image" style="border-top: 0px; border-right: 0px; background-image: none; border-bottom: 0px; float: none; padding-top: 0px; padding-left: 0px; margin-left: auto; border-left: 0px; display: block; padding-right: 0px; margin-right: auto" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/0640.image_thumb_4EFC8497.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/0640.image_5F00_thumb_5F00_4EFC8497.png" width="716" height="447" /></a>
  </p>
  
  <p>
    If you think logically this makes sense. CA’s are supposed to issue certificates. Now if I start the process from the beginning, then someone has to issue a certificate to himself and then start the process of issuing the certs down the line.
  </p>
  
  <p>
    I’m not going to discuss the purpose of the CA certificate as that would lead to a whole new discussion altogether.
  </p>
  
  <p>
    <strong><u><font size="5">Intermediate CA Certificate</font></u></strong>
  </p>
  
  <p>
    <strong>Intermediate CA </strong>Certificate is a CA certificate which is not a <strong>Self-signed Certificate</strong>. The purpose of this certificate may be same as the Root CA or different. Now one may think why to have a intermediate CA at all. Well here is what I think:
  </p>
  
  <p>
    Initially it may not require to have a Intermediate CA, as the Root CA’s will serve the purpose. However as the requirement for PKI increases so would the number of CA’s. Understanding that CA at the end of the day is a Server Machine performing this computational task, it is required to have multiple machines. So they have to be replicated. Now it is again not viable to have many Root CA’s in the case of a Internet Scenario as this could lead to fraud and other management issues. So the concept of Intermediate CA was introduced. The Root CA’s delegated their tasks to the corresponding Intermediate CA’s for this. This way they can have one or more Intermediate CA’s.
  </p>
  
  <p>
    On <strong>Windows OS</strong>, these certificates can be found in the <strong>Intermediate Certification Authorities </strong>Store. Comparatively the number of certificates in this store would be more compared to <strong>Trusted Root Certification Authorities </strong>store.
  </p>
  
  <p>
    Below is a image of a certificate store of <strong>MY </strong>or <strong>Local Computer</strong> account. It contains many certificate stores, but I have only highlighted the ones relevant to this article.
  </p>
  
  <p>
    <a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/2781.image_61D10841.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/2781.image_5F00_61D10841.png"><img title="image" style="border-top: 0px; border-right: 0px; background-image: none; border-bottom: 0px; float: none; padding-top: 0px; padding-left: 0px; margin-left: auto; border-left: 0px; display: block; padding-right: 0px; margin-right: auto" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8154.image_thumb_003B492B.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/8154.image_5F00_thumb_5F00_003B492B.png" width="501" height="419" /></a>
  </p>
  
  <p>
    </font>
  </p>
  
  <p>
    <font size="2" face="Segoe UI">Hope this article will clear some confusion at least.</font>
  </p>
  
  <p>
    <font size="2" face="Segoe UI">Until then CIAO <img class="wlEmoticon wlEmoticon-smile" style="border-top-style: none; border-left-style: none; border-bottom-style: none; border-right-style: none" alt="Smile" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/5367.wlEmoticon-smile_38920E0E.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/5367.wlEmoticon_2D00_smile_5F00_38920E0E.png" /></font>
  </p>