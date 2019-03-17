---
id: 411
title: 'AZURE REST API and PowerShell: Retrieve Cloud Service Configuration'
date: 2015-06-02T06:00:57+00:00
author: kaushal
layout: post
guid: https://blogs.msdn.microsoft.com/kaushal/2015/06/02/azure-rest-api-powershell-retrieve-cloud-service-configuration/
permalink: /2015/06/02/azure-rest-api-powershell-retrieve-cloud-service-configuration/
orig_url:
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2015/06/02/azure-rest-api-amp-powershell-retrieve-cloud-service-configuration.aspx
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2015/06/02/azure-rest-api-amp-powershell-retrieve-cloud-service-configuration.aspx
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2015/06/02/azure-rest-api-amp-powershell-retrieve-cloud-service-configuration.aspx
orig_site_id:
  - "13803"
  - "13803"
  - "13803"
orig_post_id:
  - "10618778"
  - "10618778"
  - "10618778"
orig_post_name:
  - azure rest api amp powershell retrieve cloud service configuration
  - azure rest api amp powershell retrieve cloud service configuration
  - azure rest api amp powershell retrieve cloud service configuration
orig_parent_id:
  - "10618778"
  - "10618778"
  - "10618778"
orig_thread_id:
  - "892544"
  - "892544"
  - "892544"
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
orig_post_author_email:
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
orig_post_author_created:
  - 2009-07-24 14:00:49.000
  - 2009-07-24 14:00:49.000
  - 2009-07-24 14:00:49.000
orig_is_approved:
  - "1"
  - "1"
  - "1"
orig_attachment_count:
  - "0"
  - "0"
  - "0"
total_views:
  - "697"
  - "697"
  - "697"
opengraph_tags:
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="AZURE REST API &amp; PowerShell: Retrieve Cloud Service Configuration" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2015/06/02/azure-rest-api-powershell-retrieve-cloud-service-configuration/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="Recently I was working on an issue where we had to retrieve PaaS instance configuration details like the RDP, OS Family, Reserved IP etc. Typically this is present in the .cscfg file of a Cloud Service. We had to retrieve these details via Azure Service Management REST API. Documentation on the Operations on Cloud Services..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/7444.060315_0550_AZURERESTAP1.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="AZURE REST API &amp; PowerShell: Retrieve Cloud Service Configuration" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2015/06/02/azure-rest-api-powershell-retrieve-cloud-service-configuration/" />
    <meta name="twitter:description" content="Recently I was working on an issue where we had to retrieve PaaS instance configuration details like the RDP, OS Family, Reserved IP etc. Typically this is present in the .cscfg file of a Cloud Service. We had to retrieve these details via Azure Service Management REST API. Documentation on the Operations on Cloud Services..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/7444.060315_0550_AZURERESTAP1.png" />

  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="AZURE REST API &amp; PowerShell: Retrieve Cloud Service Configuration" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2015/06/02/azure-rest-api-powershell-retrieve-cloud-service-configuration/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="Recently I was working on an issue where we had to retrieve PaaS instance configuration details like the RDP, OS Family, Reserved IP etc. Typically this is present in the .cscfg file of a Cloud Service. We had to retrieve these details via Azure Service Management REST API. Documentation on the Operations on Cloud Services..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/7444.060315_0550_AZURERESTAP1.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="AZURE REST API &amp; PowerShell: Retrieve Cloud Service Configuration" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2015/06/02/azure-rest-api-powershell-retrieve-cloud-service-configuration/" />
    <meta name="twitter:description" content="Recently I was working on an issue where we had to retrieve PaaS instance configuration details like the RDP, OS Family, Reserved IP etc. Typically this is present in the .cscfg file of a Cloud Service. We had to retrieve these details via Azure Service Management REST API. Documentation on the Operations on Cloud Services..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/7444.060315_0550_AZURERESTAP1.png" />

  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="AZURE REST API &amp; PowerShell: Retrieve Cloud Service Configuration" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2015/06/02/azure-rest-api-powershell-retrieve-cloud-service-configuration/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="Recently I was working on an issue where we had to retrieve PaaS instance configuration details like the RDP, OS Family, Reserved IP etc. Typically this is present in the .cscfg file of a Cloud Service. We had to retrieve these details via Azure Service Management REST API. Documentation on the Operations on Cloud Services..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/7444.060315_0550_AZURERESTAP1.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="AZURE REST API &amp; PowerShell: Retrieve Cloud Service Configuration" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2015/06/02/azure-rest-api-powershell-retrieve-cloud-service-configuration/" />
    <meta name="twitter:description" content="Recently I was working on an issue where we had to retrieve PaaS instance configuration details like the RDP, OS Family, Reserved IP etc. Typically this is present in the .cscfg file of a Cloud Service. We had to retrieve these details via Azure Service Management REST API. Documentation on the Operations on Cloud Services..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/7444.060315_0550_AZURERESTAP1.png" />

categories:
  - Uncategorized
---
<span style="font-family:Segoe UI; font-size:10pt">Recently I was working on an issue where we had to retrieve <strong>PaaS</strong> instance configuration details like the RDP, OS Family, Reserved IP etc. Typically this is present in the <strong>.cscfg</strong> file of a Cloud Service.<br /> </span>

<span style="font-family:Segoe UI; font-size:10pt">We had to retrieve these details via <strong>Azure Service Management REST API</strong>. Documentation on the <a href="https://msdn.microsoft.com/en-us/library/azure/ee460812.aspx">Operations on Cloud Services</a> can be found on MSDN.<br /> </span>

<span style="font-family:Segoe UI; font-size:10pt">The API of our interest is <strong>GET DEPLOYMENT</strong>. The documentation is available on MSDN: <a href="https://msdn.microsoft.com/en-us/library/azure/ee460804.aspx">https://msdn.microsoft.com/en-us/library/azure/ee460804.aspx</a><br /> </span>

<span style="font-family:Segoe UI; font-size:10pt">In this post I will be using PowerShell scripts to invoke the <strong>GET DEPLOYMENT API</strong>.<br /> </span>

<span style="font-family:Segoe UI; font-size:10pt">Below is a snippet from MSDN:<br /> </span>

<div style="margin-left: 34pt">
  <table style="border-collapse:collapse; background: #e7e6e6" border="0">
    <colgroup> <col style="width:643px"/></colgroup> <tr>
      <td style="padding-left: 7px; padding-right: 7px; border-top:  solid #00b0f0 2.25pt; border-left:  solid #00b0f0 2.25pt; border-bottom:  solid #00b0f0 2.25pt; border-right:  solid #00b0f0 2.25pt">
        <p>
          <span style="font-family:Segoe UI; font-size:10pt">The <strong>Get Deployment</strong> request can be used to retrieve deployment events for a single deployment slot (staging or production) or for a specific deployment name. If you want to retrieve information by deployment name, you must first get the unique name for the deployment. This unique name is part of the response when you make a request to get the deployment in a deployment slot.</span>
        </p>
      </td>
    </tr>
  </table>
</div>

<span style="font-family:Segoe UI; font-size:10pt">From MSDN documentation there are two ways to invoke the API.<br /> </span>

<div style="margin-left: 34pt">
  <table style="border-collapse:collapse" border="0">
    <colgroup> <col style="width:74px"/> <col style="width:568px"/></colgroup> <tr style="height: 25px; background: #0070c0">
      <td style="padding-left: 7px; padding-right: 7px; border-top:  solid 2.25pt; border-left:  solid 2.25pt; border-bottom:  solid 2.25pt; border-right:  solid 2.25pt">
        <p style="text-align: center">
          <span style="color:white; font-family:Segoe UI; font-size:12pt"><strong>Method</strong></span>
        </p>
      </td>

      <td style="padding-left: 7px; padding-right: 7px; border-top:  solid 2.25pt; border-left:  none; border-bottom:  solid 2.25pt; border-right:  solid 2.25pt">
        <p style="text-align: center">
          <span style="color:white; font-family:Segoe UI; font-size:12pt"><strong>Request URI</strong></span>
        </p>
      </td>
    </tr>

    <tr style="height: 41px">
      <td vAlign="middle" style="padding-left: 7px; padding-right: 7px; border-top:  none; border-left:  solid 2.25pt; border-bottom:  solid 1.0pt; border-right:  solid 1.0pt">
        <p style="text-align: center">
          <span style="font-family:Segoe UI; font-size:10pt">GET</span>
        </p>
      </td>

      <td vAlign="middle" style="padding-left: 7px; padding-right: 7px; border-top:  none; border-left:  none; border-bottom:  solid 1.0pt; border-right:  solid 2.25pt">
        <p>
          <a href="https://management.core.windows.net/<subscription-id>/services/hostedservices/<cloudservice-name>/deploymentslots/<deployment-slot"><span style="font-family:Segoe UI; font-size:10pt">https://management.core.windows.net/<subscription-id>/services/hostedservices/<cloudservice-name>/deploymentslots/<deployment-slot</span></a><span style="font-family:Segoe UI; font-size:10pt">> </span>
        </p>
      </td>
    </tr>

    <tr style="height: 41px">
      <td vAlign="middle" style="padding-left: 7px; padding-right: 7px; border-top:  none; border-left:  solid 2.25pt; border-bottom:  solid 2.25pt; border-right:  solid 1.0pt">
        <p style="text-align: center">
          <span style="font-family:Segoe UI; font-size:10pt">GET</span>
        </p>
      </td>

      <td vAlign="middle" style="padding-left: 7px; padding-right: 7px; border-top:  none; border-left:  none; border-bottom:  solid 2.25pt; border-right:  solid 2.25pt">
        <p>
          <a href="https://management.core.windows.net/<subscription-id>/services/hostedservices/<cloudservice-name>/deployments/<deployment-name"><span style="font-family:Segoe UI; font-size:10pt">https://management.core.windows.net/<subscription-id>/services/hostedservices/<cloudservice-name>/deployments/<deployment-name</span></a><span style="font-family:Segoe UI; font-size:10pt">> </span>
        </p>
      </td>
    </tr>
  </table>
</div>

<span style="font-family:Segoe UI; font-size:10pt">We already have a PowerShell commandlet for this functionality:<br /><strong>Get-AzureDeployment</strong>: <a href="https://msdn.microsoft.com/en-us/library/azure/dn495146.aspx">https://msdn.microsoft.com/en-us/library/azure/dn495146.aspx</a><br /> </span>

<div>
  <table style="border-collapse:collapse; background: #404040" border="0">
    <colgroup> <col style="width:756px"/></colgroup> <tr>
      <td vAlign="middle" style="padding-top: 1px; padding-left: 7px; padding-bottom: 1px; padding-right: 7px">
        <p>
          <span style="color:#00b0f0; font-family:Segoe UI; font-size:18pt">Requirements</span>
        </p>
      </td>
    </tr>
  </table>
</div>

<span style="font-family:Segoe UI; font-size:10pt">In order to make an AZURE REST API call, you have to:<br /> </span>

  1. <span style="font-family:Segoe UI; font-size:10pt">Authenticate the request to Management Service. Refer this link: <a href="https://msdn.microsoft.com/en-in/library/azure/ee460782.aspx">https://msdn.microsoft.com/en-in/library/azure/ee460782.aspx</a><br /> </span>
  2. <div>
      <span style="font-family:Segoe UI; font-size:10pt">Some <strong>Azure Service Management REST API</strong>&#8216;s require additional headers to be sent along with the request. Read the documentation for the API before proceeding further.<br /> </span>
    </div>

      1. <span style="font-family:Segoe UI; font-size:10pt">The <strong>Get Deployment</strong> API requires the <strong>x-ms-version</strong> header in HTTP Request. Below is the snippet of the documentation for this API from MSDN.<br /> </span>

<div style="margin-left: 34pt">
  <table style="border-collapse:collapse" border="0">
    <colgroup> <col style="width:143px"/> <col style="width:499px"/></colgroup> <tr style="height: 25px; background: #0070c0">
      <td style="padding-left: 7px; padding-right: 7px; border-top:  solid 2.25pt; border-left:  solid 2.25pt; border-bottom:  solid 2.25pt; border-right:  solid 2.25pt">
        <p style="text-align: center">
          <span style="color:white; font-family:Segoe UI; font-size:12pt"><strong>Request Header</strong></span>
        </p>
      </td>

      <td style="padding-left: 7px; padding-right: 7px; border-top:  solid 2.25pt; border-left:  none; border-bottom:  solid 2.25pt; border-right:  solid 2.25pt">
        <p style="text-align: center">
          <span style="color:white; font-family:Segoe UI; font-size:12pt"><strong>Description</strong></span>
        </p>
      </td>
    </tr>

    <tr style="height: 41px">
      <td vAlign="middle" style="padding-left: 7px; padding-right: 7px; border-top:  none; border-left:  solid 2.25pt; border-bottom:  solid 2.25pt; border-right:  solid 2.25pt">
        <p style="text-align: center">
          <span style="font-family:Segoe UI; font-size:10pt">x-ms-version</span>
        </p>
      </td>

      <td vAlign="middle" style="padding-left: 7px; padding-right: 7px; border-top:  none; border-left:  none; border-bottom:  solid 2.25pt; border-right:  solid 2.25pt">
        <p>
          <span style="font-family:Segoe UI; font-size:10pt">Required. Specifies the version of the operation to use for this request. This header should be set to <span style="background-color:yellow"><strong>2009-10-01</strong> or higher</span>. For more information about versioning headers, see <a href="https://msdn.microsoft.com/en-us/library/azure/gg592580.aspx">Service Management Versioning</a>.</span>
        </p>
      </td>
    </tr>
  </table>
</div>

 

<div>
  <table style="border-collapse:collapse; background: #404040" border="0">
    <colgroup> <col style="width:756px"/></colgroup> <tr>
      <td vAlign="middle" style="padding-top: 1px; padding-left: 7px; padding-bottom: 1px; padding-right: 7px">
        <p>
          <span style="color:#00b0f0; font-family:Segoe UI; font-size:18pt">Generating the certificate</span>
        </p>
      </td>
    </tr>
  </table>
</div>

<span style="font-family:Segoe UI; font-size:10pt">We will use <strong>MakeCert.exe</strong>. You may want to refer these articles:<br /> </span>

<span style="font-family:Segoe UI; font-size:10pt"><strong>Create & Upload a Management Certificate for Azure</strong>: <a href="https://msdn.microsoft.com/en-us/library/azure/gg551722.aspx">https://msdn.microsoft.com/en-us/library/azure/gg551722.aspx</a><br /> <br /><strong>Makecert.exe (Certificate Creation Tool)</strong>: <a href="https://msdn.microsoft.com/en-us/library/bfsktky3(v=vs.110).aspx">https://msdn.microsoft.com/en-us/library/bfsktky3(v=vs.110).aspx</a><br /> </span>

<span style="font-family:Segoe UI; font-size:10pt">Open a Visual studio command prompt and execute the following command:<br /> </span>

<div style="margin-left: 34pt">
  <table style="border-collapse:collapse; background: #e7e6e6" border="0">
    <colgroup> <col style="width:747px"/></colgroup> <tr>
      <td style="padding-left: 7px; padding-right: 7px; border-top:  solid #00b0f0 2.25pt; border-left:  solid #00b0f0 2.25pt; border-bottom:  solid #00b0f0 2.25pt; border-right:  solid #00b0f0 2.25pt">
        <p>
          <span style="color:black; font-family:Courier New; font-size:9pt"><span style="background-color:yellow">makecert -sky exchange -r -n &#8220;CN=</span><span style="background-color:lime"><CertificateName></span><span style="background-color:yellow">&#8221; -pe -a sha1 -len 2048 -ss My &#8220;</span><span style="background-color:lime"><CertificateName></span><span style="background-color:yellow">.cer&#8221;</span><span style="color:white"><br /> </span></span>
        </p>

        <p>
          <span style="font-family:Segoe UI; font-size:9pt">Replace the highlighted section (in green) in the above command with your inputs</span>
        </p>
      </td>
    </tr>
  </table>
</div>

  * <span style="font-family:Segoe UI; font-size:10pt">Browse to Visual Studio Tools folder.<br /> </span>
  * <span style="font-family:Segoe UI; font-size:10pt">Typically this is under: &#8220;<strong>C:\ProgramData\Microsoft\Windows\Start Menu\Programs\Microsoft Visual Studio 2012\Visual Studio Tools</strong>&#8221;<br /> </span>
  * <span style="font-family:Segoe UI; font-size:10pt">Double click and launch &#8220;<strong>VS2012 x86 Native Tools Command Prompt</strong>&#8221; in administrator mode<br /> </span>
  * <span style="font-family:Segoe UI; font-size:10pt">Execute the above command as shown below:<br /><img src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/7444.060315_0550_AZURERESTAP1.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/7444.060315_5F00_0550_5F00_AZURERESTAP1.png" alt="" /><br /> </span>
  * <span style="font-family:Segoe UI; font-size:10pt">Go to run and type &#8220;<strong>mmc</strong>&#8221; and then click on <strong>OK</strong>.<br /> </span>
  * <span style="font-size:10pt"><span style="font-family:Segoe UI">Select <strong>File</strong><br /> </span><span style="font-family:Wingdings">à</span><span style="font-family:Segoe UI"><br /> <strong>Add/Remove Snap-in…</strong><br /> </span></span>
  * <span style="font-family:Segoe UI; font-size:10pt">Select <strong>Certificates</strong> and click on <strong>Add > </strong>button<br /> </span>
  * <span style="font-family:Segoe UI; font-size:10pt">Under the <strong>Certificates snap-in</strong> select <strong>My user account</strong> and click on <strong>Finish</strong>.<br /> </span>
  * <span style="font-family:Segoe UI; font-size:10pt">Click on <strong>OK</strong>.<br /> </span>
  * <div>
      <span style="font-family:Segoe UI; font-size:10pt">This view is the <strong>current user certificate store</strong> as shown below<br /> </span>
    </div>

<img src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8877.060315_0550_AZURERESTAP2.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/8877.060315_5F00_0550_5F00_AZURERESTAP2.png" alt="" /> <span style="font-family:Segoe UI; font-size:10pt"><br /> </span>

  * <span style="font-family:Segoe UI; font-size:10pt">Export the certificate without the private key and store it on your hard drive.<br /> </span>
  * <span style="font-family:Segoe UI; font-size:10pt">Now go to the <a href="https://manage.windowsazure.com/">Azure Management Portal</a><br /> </span>
  * <div>
      <span style="font-family:Segoe UI; font-size:10pt">Scroll down to the <strong>SETTINGS</strong> section.<br /> </span>
    </div>

<img src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8484.060315_0550_AZURERESTAP3.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/8484.060315_5F00_0550_5F00_AZURERESTAP3.png" alt="" /> <span style="font-family:Segoe UI; font-size:10pt"><br /> </span>

  * <span style="font-family:Segoe UI; font-size:10pt">In the centre pane, click on <strong>MANAGEMENT CERTIFICATES</strong> & then click on <strong>UPLOAD</strong>.<br /> </span>
  * <span style="font-family:Segoe UI; font-size:10pt">Select the certificate we exported and upload it.<br /><img src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/0486.060315_0550_AZURERESTAP4.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/0486.060315_5F00_0550_5F00_AZURERESTAP4.png" alt="" /><br /> </span>
  * <div>
      <span style="font-family:Segoe UI; font-size:10pt">Make a note of the Certificate thumbprint.<br /> </span>
    </div>

     

<div>
  <table style="border-collapse:collapse; background: #404040" border="0">
    <colgroup> <col style="width:756px"/></colgroup> <tr>
      <td vAlign="middle" style="padding-top: 1px; padding-left: 7px; padding-bottom: 1px; padding-right: 7px">
        <p>
          <span style="color:#00b0f0; font-family:Segoe UI; font-size:18pt">Invoking the REST API</span>
        </p>
      </td>
    </tr>
  </table>
</div>

<span style="font-family:Segoe UI; font-size:10pt">Once the certificate has been generated and uploaded. We can write a PowerShell script to retrieve the same certificate from the store and pass it along with the REST API request.<br /> </span>

<span style="font-family:Segoe UI; font-size:10pt">We will be using <strong>PowerShell</strong> to invoke the API and retrieve the details.<br /> </span>

<span style="font-family:Segoe UI; font-size:10pt">Below is the <strong>PowerShell</strong> script to retrieve the certificate from the user store and pass it on to the <strong>Azure Service Management</strong> for authentication.<br /> </span>

<div>
  <table style="border-collapse:collapse" border="0">
    <colgroup> <col style="width:917px"/></colgroup> <tr>
      <td style="padding-left: 7px; padding-right: 7px; border-top:  solid #00b0f0 2.25pt; border-left:  solid #00b0f0 2.25pt; border-bottom:  solid #00b0f0 2.25pt; border-right:  solid #00b0f0 2.25pt">
        <p style="background: white">
          <span style="color:darkgreen; font-family:Courier New; font-size:9pt">#Request Headers required to invoke the GET DEPLOYMENT REST API<br /><span style="color:orangered">$method</span><br /> <span style="color:darkgray">=</span><br /> <span style="color:darkred">&#8220;GET&#8221;<br /><span style="color:orangered">$headerDate</span><br /> <span style="color:darkgray">=</span> &#8216;2009-10-01&#8217;<br /><span style="color:orangered">$headers</span><br /> <span style="color:darkgray">=</span> @{&#8220;x-ms-version&#8221;<span style="color:darkgray">=<span style="color:darkred">&#8220;<span style="color:orangered">$headerDate<span style="color:darkred">&#8220;</span>}</span><br /> </span></span></span></span>
        </p>

        <p style="background: white">
          <span style="font-family:Courier New; font-size:9pt"><span style="color:darkgreen">#Retrieving the subscription ID<br /><span style="color:orangered">$subID</span><br /> <span style="color:darkgray">=</span> (<span style="color:blue">Get-AzureSubscription</span><br /> <span style="color:navy">-Current</span>)<span style="color:darkgray">.</span>SubscriptionId </span><br /><span style="color:orangered">$URI</span><br /> <span style="color:darkgray">=</span><br /> <a href="https://management.core.windows.net/$subID/services/hostedservices/kaushalz/deployments/4f006bb7d2874dd4895f77a97b7938d0">https://management.core.windows.net/$subID/services/hostedservices/kaushalz/deployments/4f006bb7d2874dd4895f77a97b7938d0</a><span style="color:darkred"><br /> </span></span>
        </p>

        <p style="background: white">
          <span style="color:darkgreen; font-family:Courier New; font-size:9pt">#Retrieving the certificate from Local Store<br /><span style="color:orangered">$cert</span><br /> <span style="color:darkgray">=</span> (<span style="color:blue">Get-ChildItem</span><br /> <span style="color:blueviolet">Cert:\CurrentUser\My</span><br /> <span style="color:darkgray">|</span><br /> <span style="color:blue">?</span>{<span style="color:orangered">$_<span style="color:darkgray">.</span>Thumbprint <span style="color:darkgray">-eq</span><br /> <span style="color:darkred">&#8220;B4D460D985F1D07A6B9F8BFD67E36BC53A4490FC&#8221;</span>})<span style="color:darkgray">.</span>GetRawCertData()<span style="color:darkred"><br /> </span></span></span>
        </p>

        <p style="background: white">
          <span style="color:darkgreen; font-family:Courier New; font-size:9pt">#converting the raw cert data to BASE64<br /><span style="color:orangered">body</span><br /> <span style="color:darkgray">=</span><br /> <span style="color:darkred">&#8220;<Binary>&#8212;&#8211;BEGIN CERTIFICATE&#8212;&#8211;`n</span>$(<span style="color:darkgray">[<span style="color:teal">convert<span style="color:darkgray">]::</span>ToBase64String(<span style="color:orangered">$cert</span>))<span style="color:darkred">`n&#8212;&#8211;END CERTIFICATE&#8212;&#8211;</Binary>&#8221;<br /> </span></span></span></span>
        </p>

        <p style="background: white">
          <span style="font-family:Courier New; font-size:9pt"><span style="color:darkgreen">#Retrieving the certificate ThumbPrint<br /><span style="color:orangered">$mgmtCertThumb</span><br /> <span style="color:darkgray">=</span> (<span style="color:blue">Get-AzureSubscription</span><br /> <span style="color:navy">-Current</span>)<span style="color:darkgray">.</span>Certificate<span style="color:darkgray">.</span>Thumbprint</span><br /> </span>
        </p>

        <p style="background: white">
          <span style="color:darkgreen; font-family:Courier New; font-size:9pt">#Passing all the above parameters to Invoke-RestMethod cmdlet<br /><span style="color:blue">Invoke-RestMethod</span><br /> <span style="color:navy">-Uri</span><br /> <span style="color:orangered">$URI</span><br /> <span style="color:navy">-Method</span><br /> <span style="color:orangered">$method</span><br /> <span style="color:navy">-Headers</span><br /> <span style="color:orangered">$headers</span><br /> <span style="color:navy">-CertificateThumbprint</span><br /> <span style="color:darkred">&#8221; B4D460D985F1D07A6B9F8BFD67E36BC53A4490FC&#8221;</span><br /> <span style="color:navy">-ContentType</span><br /> <span style="color:orangered">$ContentType</span></span>
        </p>
      </td>
    </tr>
  </table>
</div>

  * <span style="font-family:Segoe UI; font-size:10pt">Launch <strong>Windows PowerShell ISE</strong> in administrator mode.<br /> </span>
  * <span style="font-family:Segoe UI; font-size:10pt">Copy the above sample script and paste it in the scripting window.<br /> </span>

<div style="margin-left: 34pt">
  <table style="border-collapse:collapse; background: #e7e6e6" border="0">
    <colgroup> <col style="width:643px"/></colgroup> <tr>
      <td style="padding-left: 7px; padding-right: 7px; border-top:  solid #00b0f0 2.25pt; border-left:  solid #00b0f0 2.25pt; border-bottom:  solid #00b0f0 2.25pt; border-right:  solid #00b0f0 2.25pt">
        <p>
          <span style="font-family:Segoe UI; font-size:10pt"><strong>NOTE</strong>: replace the <strong>thumbprint</strong> in the above script with the thumbprint of your certificate. You can retrieve this from the MMC windows we accessed earlier. I&#8217;m passing the <strong>Deployment Name</strong> (or <strong>Deployment ID</strong>) in the above URL.</span>
        </p>
      </td>
    </tr>
  </table>
</div>

  * <span style="font-family:Segoe UI; font-size:10pt">Run the script to get the output as shown below:<br /> </span>

<img src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3482.060315_0550_AZURERESTAP5.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/3482.060315_5F00_0550_5F00_AZURERESTAP5.png" alt="" /> <span style="font-family:Segoe UI; font-size:10pt"><br /> </span>

<span style="font-family:Segoe UI; font-size:10pt">If you read the documentation, the response body is in XML format and it is displaying only the parent node (DEPLOYMENT).<br /> </span>

<span style="font-family:Segoe UI; font-size:10pt">We can read the response into a XML object and then display it. Here is sample snippet:<br /> </span>

<div style="margin-left: 34pt">
  <table style="border-collapse:collapse" border="0">
    <colgroup> <col style="width:690px"/></colgroup> <tr>
      <td style="padding-left: 7px; padding-right: 7px; border-top:  solid #00b0f0 2.25pt; border-left:  solid #00b0f0 2.25pt; border-bottom:  solid #00b0f0 2.25pt; border-right:  solid #00b0f0 2.25pt">
        <p style="background: white">
          <span style="color:darkgreen; font-family:Courier New; font-size:9pt">#Getting the response from the REST API and saving it as a XML object<br /><span style="color:darkgray">[<span style="color:teal">xml<span style="color:darkgray">]<span style="color:orangered">$url</span> =</span><br /> <span style="color:blue">Invoke-RestMethod</span><br /> <span style="color:navy">-Uri</span><br /> <span style="color:orangered">$URI</span><br /> <span style="color:navy">-Method</span><br /> <span style="color:orangered">$method</span><br /> <span style="color:navy">-Headers</span><br /> <span style="color:orangered">$headers</span><br /> <span style="color:navy">-CertificateThumbprint</span><br /> <span style="color:darkred">&#8220;B4D460D985F1D07A6B9F8BFD67E36BC53A4490FC&#8221;</span><br /> <span style="color:navy">-ContentType</span><br /> <span style="color:orangered">$ContentType<span style="color:darkgreen"><br /> </span></span></span></span></span>
        </p>

        <p style="background: white">
          <span style="color:darkgreen; font-family:Courier New; font-size:9pt">#Printing the XML<br /><span style="color:blue">write</span><br /> <span style="color:orangered">$url<span style="color:darkgray">.</span>ChildNodes</span></span>
        </p>
      </td>
    </tr>
  </table>
</div>

<span style="font-family:Segoe UI; font-size:10pt">Below is a screenshot of the output after adding the above two lines in the earlier script:<br /> </span>

<img src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/1667.060315_0550_AZURERESTAP6.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/1667.060315_5F00_0550_5F00_AZURERESTAP6.png" alt="" /> <span style="font-family:Segoe UI; font-size:10pt"><br /> </span>

<div style="margin-left: 34pt">
  <table style="border-collapse:collapse; background: white" border="0">
    <colgroup> <col style="width:643px"/></colgroup> <tr>
      <td style="padding-left: 7px; padding-right: 7px; border-top:  solid #00b0f0 2.25pt; border-left:  solid #00b0f0 2.25pt; border-bottom:  solid #00b0f0 2.25pt; border-right:  solid #00b0f0 2.25pt">
        <p>
          <span style="font-family:Segoe UI; font-size:10pt"><strong>NOTE</strong>: The Configuration section in the above output is a Base-64 encoded string. You would have to add the following snippet to parse this further:<br /> </span>
        </p>

        <p style="background: white">
          <span style="font-family:Courier New; font-size:9pt"><span style="color:orangered">$base64encodedconfiguration</span><br /> <span style="color:darkgray">=</span><br /> <span style="color:orangered">$url<span style="color:darkgray">.</span>Deployment<span style="color:darkgray">.</span>Configuration</span><br /><span style="color:orangered">$d<span style="color:darkgray">=</span><br /> <span style="color:darkgray">[<span style="color:teal">System.Convert<span style="color:darkgray">]::</span>FromBase64String(<span style="color:orangered">$base64encodedconfiguration</span>)</span><br />[<span style="color:teal">xml<span style="color:darkgray">]<span style="color:orangered">$decodedxml</span> =</span><br /> <span style="color:darkgray">[<span style="color:teal">System.Text.Encoding<span style="color:darkgray">]::</span>UTF8<span style="color:darkgray">.</span>GetString(<span style="color:orangered">$d</span>)</span><br /><span style="color:blue">write</span><br /> <span style="color:orangered">$decodedxml<span style="color:darkgray">.</span>ChildNodes</span></span></span></span></span></span>
        </p>
      </td>
    </tr>
  </table>
</div>

<span style="font-family:Segoe UI; font-size:10pt">You can use the same approach to call any other Azure Service Management REST API. Ensure you read the documentation carefully and then proceed further.<br /> </span>

<span style="font-size:10pt"><span style="font-family:Segoe UI">HTH </span><span style="font-family:Wingdings">J</span></span>
