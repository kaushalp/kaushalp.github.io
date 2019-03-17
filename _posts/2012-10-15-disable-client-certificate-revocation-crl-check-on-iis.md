---
id: 154
title: Disable Client Certificate Revocation (CRL) Check on IIS
date: 2012-10-15T00:04:40+00:00
author: kaushal
layout: post
guid: https://blogs.msdn.microsoft.com/kaushal/2012/10/15/disable-client-certificate-revocation-crl-check-on-iis/
permalink: /2012/10/15/disable-client-certificate-revocation-crl-check-on-iis/
orig_url:
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2012/10/15/disable-client-certificate-revocation-check-on-iis.aspx
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2012/10/15/disable-client-certificate-revocation-check-on-iis.aspx
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2012/10/15/disable-client-certificate-revocation-check-on-iis.aspx
orig_site_id:
  - "13803"
  - "13803"
  - "13803"
orig_post_id:
  - "10359592"
  - "10359592"
  - "10359592"
orig_parent_id:
  - "10359592"
  - "10359592"
  - "10359592"
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
  - http://blogs.msdn.com/b/kaushal/archive/2012/10/15/disable-client-certificate-revocation-crl-check-on-iis.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2012/10/15/disable-client-certificate-revocation-crl-check-on-iis.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2012/10/15/disable-client-certificate-revocation-crl-check-on-iis.aspx
orig_post_name:
  - disable client certificate revocation check on iis
  - disable client certificate revocation check on iis
  - disable client certificate revocation check on iis
orig_thread_id:
  - "823757"
  - "823757"
  - "823757"
orig_post_author_email:
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
orig_attachment_count:
  - "0"
  - "0"
  - "0"
total_views:
  - "47302"
  - "47302"
  - "47302"
opengraph_tags:
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Disable Client Certificate Revocation (CRL) Check on IIS" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/10/15/disable-client-certificate-revocation-crl-check-on-iis/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="I have been asked this question on several occasions on how to disable revocation check in IIS 7.  It was pretty easy for IIS 6, on IIS 7 there is no documentation on how to do so. This post will describe on how to achieve this task. Firstly, list out all the existing IIS bindings..." />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Disable Client Certificate Revocation (CRL) Check on IIS" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/10/15/disable-client-certificate-revocation-crl-check-on-iis/" />
    <meta name="twitter:description" content="I have been asked this question on several occasions on how to disable revocation check in IIS 7.  It was pretty easy for IIS 6, on IIS 7 there is no documentation on how to do so. This post will describe on how to achieve this task. Firstly, list out all the existing IIS bindings..." />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Disable Client Certificate Revocation (CRL) Check on IIS" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/10/15/disable-client-certificate-revocation-crl-check-on-iis/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="I have been asked this question on several occasions on how to disable revocation check in IIS 7.  It was pretty easy for IIS 6, on IIS 7 there is no documentation on how to do so. This post will describe on how to achieve this task. Firstly, list out all the existing IIS bindings..." />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Disable Client Certificate Revocation (CRL) Check on IIS" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/10/15/disable-client-certificate-revocation-crl-check-on-iis/" />
    <meta name="twitter:description" content="I have been asked this question on several occasions on how to disable revocation check in IIS 7.  It was pretty easy for IIS 6, on IIS 7 there is no documentation on how to do so. This post will describe on how to achieve this task. Firstly, list out all the existing IIS bindings..." />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Disable Client Certificate Revocation (CRL) Check on IIS" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/10/15/disable-client-certificate-revocation-crl-check-on-iis/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="I have been asked this question on several occasions on how to disable revocation check in IIS 7.  It was pretty easy for IIS 6, on IIS 7 there is no documentation on how to do so. This post will describe on how to achieve this task. Firstly, list out all the existing IIS bindings..." />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Disable Client Certificate Revocation (CRL) Check on IIS" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/10/15/disable-client-certificate-revocation-crl-check-on-iis/" />
    <meta name="twitter:description" content="I have been asked this question on several occasions on how to disable revocation check in IIS 7.  It was pretty easy for IIS 6, on IIS 7 there is no documentation on how to do so. This post will describe on how to achieve this task. Firstly, list out all the existing IIS bindings..." />
    
categories:
  - Uncategorized
tags:
  - .crl
  - CCS
  - Certificate Revocatio
  - CRL
  - netsh
  - SNI
  - SSL
  - verifyclientcertrevocation
---
<span style="font-family: Segoe UI;font-size: small">I have been asked this question on several occasions on how to disable revocation check in IIS 7.  It was pretty easy for IIS 6, on IIS 7 there is no documentation on how to do so. This post will describe on how to achieve this task.</span>

<span style="font-size: small"><span style="font-family: Segoe UI">Firstly, list out all the existing IIS bindings via command line as shown below:</span></span>

<table border="3" width="600" cellspacing="0" cellpadding="2" align="center" bgcolor="#000000">
  <tr bgcolor="#000000">
    <td valign="top" width="594" bgcolor="#000000">
      <p align="center">
        <span style="color: #ffffff;font-family: Courier New;font-size: medium"><strong>netsh http show sslcert</strong></span>
      </p>
    </td>
  </tr>
  
  <tr bgcolor="#000000">
    <td valign="top" width="594">
      <p align="left">
        <span style="color: #ffffff;font-family: Segoe UI;font-size: medium"><strong><u>Default SSL Binding when added via IIS Manager</u></strong></span>
      </p>
      
      <p align="left">
        <span style="color: #ffffff;font-family: Courier New;font-size: small">IP:port                      : 0.0.0.0:443<br /> Certificate Hash             : 40db5bb1bf5659a155258d1d007c530fcb8996c2<br /> Application ID               : {4dc3e181-e14b-4a21-b022-59fc669b0914}<br /> Certificate Store Name       : My<br /> <span style="background-color: #ff0000"><strong>Verify Client Certificate Revocation    : Enabled</strong></span><br /> Verify Revocation Using Cached Client Certificate Only    : Disabled<br /> Usage Check                  : Enabled<br /> Revocation Freshness Time    : 0<br /> URL Retrieval Timeout        : 0<br /> Ctl Identifier               : (null)<br /> Ctl Store Name               : (null)<br /> DS Mapper Usage              : Disabled<br /> Negotiate Client Certificate : Disabled</span>
      </p>
    </td>
  </tr>
</table>

<span style="font-family: Segoe UI;font-size: medium"><strong>NOTE:</strong></span>

<table border="2" width="584" cellspacing="0" cellpadding="2" align="center" bgcolor="#778899">
  <tr>
    <td valign="top" width="580">
      <ol>
        <li>
          <span style="font-family: Segoe UI;font-size: small"><strong>Client Certificate Revocation</strong> is always enabled by default.</span>
        </li>
        <li>
          <span style="font-family: Segoe UI;font-size: small">Application ID of “</span><span style="background-color: #ffff00;font-family: Courier New;font-size: small"><strong>{4dc3e181-e14b-4a21-b022-59fc669b0914}</strong></span><span style="font-family: Segoe UI;font-size: small">” corresponds to <strong>IIS</strong>.</span>
        </li>
      </ol>
    </td>
  </tr>
</table>

<span style="font-family: Segoe UI;font-size: small"><br /> In order to disable the revocation check, we need to delete the existing binding first. <span style="background-color: #a5a5a5"><strong>Before you do that, make a note of the above details, especially the certificate hash.</strong></span></span>

<table border="2" width="600" cellspacing="0" cellpadding="2" align="center">
  <tr>
    <td align="center" width="596">
      <p align="left">
        <span style="font-family: Segoe UI;font-size: medium"><strong><u>NETSH command to delete existing SSL binding:</u></strong></span>
      </p>
      
      <p align="center">
        <span style="font-size: small"><span style="font-family: Courier New;font-size: medium"><strong>netsh http delete sslcert ipport=0.0.0.0:443</strong></span></span>
      </p>
    </td>
  </tr>
</table>

<span style="font-family: Segoe UI;font-size: small">Now add the binding again using netsh as shown below:</span>

<table border="2" width="600" cellspacing="0" cellpadding="2" align="center">
  <tr>
    <td valign="top" width="596">
      <p align="left">
        <span style="font-family: Segoe UI;font-size: medium"><strong><u>NETSH command to add an SSL binding to disable CRL Check:</u></strong></span>
      </p>
      
      <p align="left">
        <span style="font-family: Courier New;font-size: medium"><strong>netsh</strong> http add sslcert <strong>ipport</strong>=0.0.0.0:443 <strong>certhash</strong>=40db5bb1bf5659a155258d1d007c530fcb8996c2<br /> <strong>appid</strong>={4dc3e181-e14b-4a21-b022-59fc669b0914}<br /> <strong>certstorename</strong>=My <span style="background-color: #ffff00"><strong>verifyclientcertrevocation</strong>=disable</span></span>
      </p>
    </td>
  </tr>
</table>

&nbsp;

<span style="font-family: Segoe UI;font-size: small">Highlighted portion of the above command depicts that we are disabling the client certificate revocation. This adds a DWORD at the following location in registry:</span>

<table border="2" width="600" cellspacing="0" cellpadding="2" align="center">
  <tr>
    <td valign="top" width="596">
      <span style="font-size: small"><span style="font-family: Segoe UI"><strong>REGISTRY  </strong>: HKLM\SYSTEM\CurrentControlSet\Services\HTTP\Parameters\SslBindingInfo<br /> <strong>DWORD    </strong>: DefaultSslCertCheckMode<br /> <strong>Value         </strong>: 1</span></span>
    </td>
  </tr>
</table>

<span style="font-family: Segoe UI;font-size: small"><span style="font-size: small"><span style="font-family: Segoe UI"><strong>DefaultSslCertCheckMode</strong> </span></span>can take the following values. <a href="http://msdn.microsoft.com/en-us/library/aa364647.aspx" target="_blank" rel="noopener noreferrer">Click here</a> for more info.</span>

<table class="MsoTableMediumShading2Accent5" style="border: currentcolor;border-collapse: collapse" border="1" width="460" cellspacing="0" cellpadding="0" align="center">
  <tr style="height: 27.55pt">
    <td style="background: #4472c4;padding: 0cm 5.4pt;border: 2.25pt solid windowtext;width: 63.8pt;height: 27.55pt" width="85">
      <p align="center">
        <b><span lang="EN-IN" style="color: white;font-family: 'Segoe UI','sans-serif';font-size: 14pt"><span style="font-size: medium">VALUE</span></span></b>
      </p>
    </td>
    
    <td style="background: #4472c4;border-width: 2.25pt 2.25pt 2.25pt medium;border-style: solid solid solid none;border-color: windowtext windowtext windowtext currentcolor;padding: 0cm 5.4pt;width: 331.95pt;height: 27.55pt" width="373">
      <p align="center">
        <b><span lang="EN-IN" style="color: white;font-family: 'Segoe UI','sans-serif';font-size: 14pt"><span style="font-size: medium">MEANING</span></span></b>
      </p>
    </td>
  </tr>
  
  <tr style="height: 27.55pt">
    <td style="background: #4472c4;border-width: medium 2.25pt 2.25pt;border-style: none solid solid;border-color: currentcolor windowtext windowtext;padding: 0cm 5.4pt;width: 63.8pt;height: 27.55pt" align="center" width="85">
      <b><span lang="EN-IN" style="color: white;font-family: 'Segoe UI','sans-serif';font-size: 12pt"></span></b>
    </td>
    
    <td style="background: #d8d8d8;border-width: medium 2.25pt medium medium;border-style: none solid none none;border-color: currentcolor windowtext currentcolor currentcolor;padding: 0cm 5.4pt;width: 331.95pt;height: 27.55pt" align="center" width="373">
      <span lang="EN-IN" style="font-family: 'Segoe UI','sans-serif';font-size: 12pt"><span style="font-size: small">Enables the client certificate revocation check</span></span>
    </td>
  </tr>
  
  <tr style="height: 27.55pt">
    <td style="background: #4472c4;border-width: medium 2.25pt 2.25pt;border-style: none solid solid;border-color: currentcolor windowtext windowtext;padding: 0cm 5.4pt;width: 63.8pt;height: 27.55pt" align="center" width="85">
      <b><span lang="EN-IN" style="color: white;font-family: 'Segoe UI','sans-serif';font-size: 12pt">1</span></b>
    </td>
    
    <td style="border-width: medium 2.25pt medium medium;border-style: none solid none none;border-color: currentcolor windowtext currentcolor currentcolor;padding: 0cm 5.4pt;width: 331.95pt;height: 27.55pt" align="center" width="373">
      <span lang="EN-IN" style="font-family: 'Segoe UI','sans-serif';font-size: 12pt"><span style="font-size: small">Client certificate is not to be verified for revocation.</span></span>
    </td>
  </tr>
  
  <tr style="height: 27.55pt">
    <td style="background: #4472c4;border-width: medium 2.25pt 2.25pt;border-style: none solid solid;border-color: currentcolor windowtext windowtext;padding: 0cm 5.4pt;width: 63.8pt;height: 27.55pt" align="center" width="85">
      <b><span lang="EN-IN" style="color: white;font-family: 'Segoe UI','sans-serif';font-size: 12pt">2</span></b>
    </td>
    
    <td style="background: #d8d8d8;border-width: medium 2.25pt medium medium;border-style: none solid none none;border-color: currentcolor windowtext currentcolor currentcolor;padding: 0cm 5.4pt;width: 331.95pt;height: 27.55pt" align="center" width="373">
      <span lang="EN-IN" style="font-family: 'Segoe UI','sans-serif';font-size: 12pt"><span style="font-size: small">Only cached certificate revocation is to be used</span></span>
    </td>
  </tr>
  
  <tr style="height: 27.55pt">
    <td style="background: #4472c4;border-width: medium 2.25pt 2.25pt;border-style: none solid solid;border-color: currentcolor windowtext windowtext;padding: 0cm 5.4pt;width: 63.8pt;height: 27.55pt" align="center" width="85">
      <b><span lang="EN-IN" style="color: white;font-family: 'Segoe UI','sans-serif';font-size: 12pt">4</span></b>
    </td>
    
    <td style="border-width: medium 2.25pt medium medium;border-style: none solid none none;border-color: currentcolor windowtext currentcolor currentcolor;padding: 0cm 5.4pt;width: 331.95pt;height: 27.55pt" align="center" width="373">
      <span lang="EN-IN" style="font-family: 'Segoe UI','sans-serif';font-size: 12pt"><span style="font-size: small">The <b>DefaultRevocationFreshnessTime</b> setting is enabled</span></span>
    </td>
  </tr>
  
  <tr style="height: 27.55pt">
    <td style="background: #4472c4;border-width: medium 2.25pt 2.25pt;border-style: none solid solid;border-color: currentcolor windowtext windowtext;padding: 0cm 5.4pt;width: 63.8pt;height: 27.55pt" align="center" width="85">
      <b><span lang="EN-IN" style="color: white;font-family: 'Segoe UI','sans-serif';font-size: 12pt">0x10000</span></b>
    </td>
    
    <td style="background: #d8d8d8;border-width: medium 2.25pt 2.25pt medium;border-style: none solid solid none;border-color: currentcolor windowtext windowtext currentcolor;padding: 0cm 5.4pt;width: 331.95pt;height: 27.55pt" align="center" width="373">
      <span lang="EN-IN" style="font-family: 'Segoe UI','sans-serif';font-size: 12pt"><span style="font-size: small">No usage check is to be performed</span></span>
    </td>
  </tr>
</table>

&nbsp;

<span style="font-family: Segoe UI;font-size: small">Review the SSL bindings after executing the above command. The <strong>CRL</strong> check would be disabled.</span>

<table border="3" width="600" cellspacing="0" cellpadding="2" align="center" bgcolor="#000000">
  <tr bgcolor="#000000">
    <td valign="top" width="594">
      <p align="center">
        <span style="color: #ffffff;font-family: Courier New;font-size: medium"><strong>netsh http show sslcert</strong></span>
      </p>
    </td>
  </tr>
  
  <tr bgcolor="#000000">
    <td valign="top" width="594">
      <p align="left">
        <span style="color: #ffffff;font-family: Segoe UI;font-size: medium"><strong><u>SSL Binding added via NETSH to disable CRL:</u></strong></span>
      </p>
      
      <p align="left">
        <span style="color: #ffffff"><span style="font-family: Courier New;font-size: small">IP:port                      : 0.0.0.0:443<br /> Certificate Hash             : 40db5bb1bf5659a155258d1d007c530fcb8996c2<br /> Application ID               : {4dc3e181-e14b-4a21-b022-59fc669b0914}<br /> Certificate Store Name       : My<br /> <span style="background-color: #00ff00;color: #000000"><strong>Verify Client Certificate Revocation    : Disabled</strong></span><br /> Verify Revocation Using Cached Client Certificate Only    : Disabled<br /> Usage Check                  : Enabled<br /> Revocation Freshness Time    : 0<br /> URL Retrieval Timeout        : 0<br /> Ctl Identifier               : (null)<br /> Ctl Store Name               : (null)<br /> DS Mapper Usage              : Disabled<br /> Negotiate Client Certificate : Disabled</span> </span>
      </p>
    </td>
  </tr>
</table>

<span style="font-family: Segoe UI;font-size: small"><span style="background-color: #a5a5a5"><strong>NOTE</strong>: Client Certificate Revocation is always enabled by default.</span></span>

<span style="font-family: Segoe UI;font-size: small">More details on the <strong>netsh </strong>commands for <strong>HTTP </strong>can be found here: <a title="http://technet.microsoft.com/en-us/library/cc725882(v=ws.10).aspx#BKMK_2" href="http://technet.microsoft.com/en-us/library/cc725882(v=ws.10).aspx#BKMK_2">http://technet.microsoft.com/en-us/library/cc725882(v=ws.10).aspx#BKMK_2</a></span>

<p align="center">
  <span style="font-family: Segoe UI;font-size: large"><strong><u>MORE INFORMATION</u></strong></span>
</p>

<span style="font-family: Segoe UI;font-size: medium"><strong>NETSH Commands for HTTP in IIS 8:</strong></span>

<span style="font-family: Segoe UI;font-size: small">With IIS there are <strong>2</strong> new SSL bindings viz. <strong>SNI Bindings</strong> and <strong>CCS Bindings</strong>. So the above commands would have to be modified slightly to incorporate these changes. So we have 2 additional parameters than what are listed in the above <strong><a href="http://technet.microsoft.com/en-us/library/cc725882(v=ws.10).aspx#BKMK_2" target="_blank" rel="noopener noreferrer">TechNet article</a></strong>. They are:</span>

<table class="MsoTableMediumShading2Accent1" style="border: currentcolor;border-collapse: collapse" border="1" width="481" cellspacing="0" cellpadding="0" align="center">
  <tr style="height: 25.55pt">
    <td style="background: #4f81bd;padding: 0cm 5.4pt;border: 2.25pt solid windowtext;width: 103.85pt;height: 25.55pt" width="138">
      <p class="MsoNormal" style="text-align: center" align="center">
        <span class="MsoHyperlink"><b><span style="color: black;line-height: 105%;font-family: 'Segoe UI','sans-serif';font-size: 14pt;text-decoration: none">Tag</span></b></span>
      </p>
    </td>
    
    <td style="background: #4f81bd;border-width: 2.25pt 2.25pt 2.25pt medium;border-style: solid solid solid none;border-color: windowtext windowtext windowtext currentcolor;padding: 0cm 5.4pt;width: 299.3pt;height: 25.55pt" width="341">
      <p class="MsoNormal" style="text-align: center" align="center">
        <span class="MsoHyperlink"><b><span style="color: black;line-height: 105%;font-family: 'Segoe UI','sans-serif';font-size: 14pt;text-decoration: none">Value</span></b></span>
      </p>
    </td>
  </tr>
  
  <tr style="height: 25.55pt">
    <td style="background: #4f81bd;border-width: medium 2.25pt 2.25pt;border-style: none solid solid;border-color: currentcolor windowtext windowtext;padding: 0cm 5.4pt;width: 103.85pt;height: 25.55pt" align="center" width="138">
      <strong><span class="MsoHyperlink"><span style="color: black;line-height: 105%;font-family: 'Segoe UI','sans-serif';font-size: 12pt;text-decoration: none">hostnameport</span></span> </strong>
    </td>
    
    <td style="background: #d8d8d8;border-width: medium 2.25pt 2.25pt medium;border-style: none solid solid none;border-color: currentcolor windowtext windowtext currentcolor;padding: 0cm 5.4pt;width: 299.3pt;height: 25.55pt" align="center" width="341">
      <span style="font-size: medium"><span class="MsoHyperlink"><span style="color: black;font-family: 'Segoe UI','sans-serif';text-decoration: none">Unicode hostname and port for binding.</span></span> </span>
    </td>
  </tr>
  
  <tr style="height: 25.55pt">
    <td style="background: #4f81bd;border-width: medium 2.25pt 2.25pt;border-style: none solid solid;border-color: currentcolor windowtext windowtext;padding: 0cm 5.4pt;width: 103.85pt;height: 25.55pt" align="center" width="138">
      <span style="font-family: Segoe UI;font-size: medium"><strong>CCS</strong></span>
    </td>
    
    <td style="border-width: medium 2.25pt 2.25pt medium;border-style: none solid solid none;border-color: currentcolor windowtext windowtext currentcolor;padding: 0cm 5.4pt;width: 299.3pt;height: 25.55pt" align="center" width="341">
      <span class="MsoHyperlink"><span style="color: black;font-family: 'Segoe UI','sans-serif';text-decoration: none"><span style="font-size: medium">Central Certificate Store binding.</span></span></span>
    </td>
  </tr>
</table>

<span style="font-family: Segoe UI;font-size: small"><strong>hostnameport</strong> is very similar to the ipport. The only difference is that it takes a <strong>Unicode</strong> string as an input along with the port number. </span>

<span style="font-family: Segoe UI;font-size: small">Below are the modified commands for the corresponding bindings in <strong>IIS 8</strong>:</span>

<table class="MsoTableGrid" style="border: currentcolor;margin-right: 6.75pt;margin-left: 6.75pt;border-collapse: collapse" border="1" cellspacing="0" cellpadding="0" align="center" bgcolor="#708090">
  <tr style="height: 36.25pt">
    <td style="padding: 0cm 5.4pt;border: 2.25pt solid windowtext;width: 445.4pt;height: 36.25pt" width="594">
      <p class="MsoNormal">
        <strong><u><span style="font-family: 'Segoe UI','sans-serif'"><span style="font-size: medium">To delete a SNI Binding</span></span></u></strong>
      </p>
      
      <p class="MsoNormal" style="margin-bottom: 0pt" align="left">
        <span style="font-size: small"><span class="SpellE"><strong><span style="font-family: 'Courier New'">netsh</span></strong></span><strong><span style="font-family: 'Courier New'"> http delete <span class="SpellE">sslcert</span> <span style="background: yellow">hostnameport=www.sni.com:443</span></span></strong></span>
      </p>
      
      <p class="MsoNormal" style="margin-bottom: 0pt" align="left">
        <p class="MsoNormal" style="margin-bottom: 0pt" align="left">
          </td> </tr> 
          
          <tr style="height: 36.25pt">
            <td style="border-width: medium 2.25pt 2.25pt;border-style: none solid solid;border-color: currentcolor windowtext windowtext;padding: 0cm 5.4pt;width: 445.4pt;height: 36.25pt" width="594">
              <p class="MsoNormal">
                <strong><u><span style="font-family: 'Segoe UI','sans-serif'"><span style="font-size: medium">To delete a CCS Binding</span></span></u></strong>
              </p>
              
              <p class="MsoNormal" style="margin-bottom: 0pt">
                <span style="font-size: small"><span class="SpellE"><strong><span style="font-family: 'Courier New'">netsh</span></strong></span><strong><span style="font-family: 'Courier New'"> http delete <span class="SpellE">sslcert</span> <span style="background: yellow">ccs=443</span></span></strong></span>
              </p>
              
              <p class="MsoNormal" style="margin-bottom: 0pt">
                <p class="MsoNormal" style="margin-bottom: 0pt">
                  </td> </tr> 
                  
                  <tr style="height: 36.25pt">
                    <td style="border-width: medium 2.25pt 2.25pt;border-style: none solid solid;border-color: currentcolor windowtext windowtext;padding: 0cm 5.4pt;width: 445.4pt;height: 36.25pt" width="594">
                      <p class="MsoNormal">
                        <strong><u><span style="font-family: 'Segoe UI','sans-serif'"><span style="font-size: medium">To add a SNI Binding</span></span></u></strong>
                      </p>
                      
                      <p class="MsoNormal" style="margin-bottom: 0pt">
                        <span style="font-size: small"><span class="SpellE"><strong><span style="font-family: 'Courier New'">netsh</span></strong></span><span style="font-family: 'Courier New'"> http add <span class="SpellE">sslcert</span> <b><span style="background: yellow">hostnameport=www.sni.com:443</span></b> <span class="SpellE">certhash</span>=40db5bb1bf5659a155258d1d007c530fcb8996c2 <span class="SpellE">appid</span>={4dc3e181-e14b-4a21-b022-59fc669b0914} certstorename=My <span class="SpellE"><b><span style="background: yellow">verifyclientcertrevocation</span></b></span><b><span style="background: yellow">=disable</span></b></span></span>
                      </p>
                      
                      <p class="MsoNormal" style="margin-bottom: 0pt">
                        <p class="MsoNormal" style="margin-bottom: 0pt">
                          </td> </tr> 
                          
                          <tr style="height: 36.25pt">
                            <td style="border-width: medium 2.25pt 2.25pt;border-style: none solid solid;border-color: currentcolor windowtext windowtext;padding: 0cm 5.4pt;width: 445.4pt;height: 36.25pt" width="594">
                              <p class="MsoNormal">
                                <strong><u><span style="font-family: 'Segoe UI','sans-serif'"><span style="font-size: medium">To add a CCS Binding</span></span></u></strong>
                              </p>
                              
                              <p class="MsoNormal" style="margin-bottom: 0pt">
                                <span style="font-size: small"><span class="SpellE"><strong><span style="font-family: 'Courier New'">netsh</span></strong></span><span style="font-family: 'Courier New'"> http add <span class="SpellE">sslcert</span> <b><span style="background: yellow">ccs=443</span></b> <span class="SpellE">appid</span>={4dc3e181-e14b-4a21-b022-59fc669b0914} <span class="SpellE"><b><span style="background: yellow">verifyclientcertrevocation</span></b></span><b><span style="background: yellow">=disable</span></b></span></span>
                              </p>
                              
                              <p class="MsoNormal" style="margin-bottom: 0pt">
                                <p class="MsoNormal" style="margin-bottom: 0pt">
                                  <p class="MsoNormal" style="margin-bottom: 0pt">
                                    </td> </tr> </tbody> </table> 
                                    
                                    <p>
                                      &nbsp;
                                    </p>