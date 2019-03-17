---
id: 403
title: Client Certificate Authentication (Part 1)
date: 2015-05-27T00:04:00+00:00
author: kaushal
layout: post
guid: https://blogs.msdn.microsoft.com/kaushal/2015/05/27/client-certificate-authentication/
permalink: /2015/05/27/client-certificate-authentication-part-1/
orig_url:
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2015/05/27/client-certificate-authentication.aspx
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2015/05/27/client-certificate-authentication.aspx
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2015/05/27/client-certificate-authentication.aspx
orig_site_id:
  - "13803"
  - "13803"
  - "13803"
orig_post_id:
  - "10617445"
  - "10617445"
  - "10617445"
orig_parent_id:
  - "10617445"
  - "10617445"
  - "10617445"
orig_thread_id:
  - "892211"
  - "892211"
  - "892211"
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
orig_attachment_count:
  - "0"
  - "0"
  - "0"
orig_url_title:
  - http://blogs.msdn.com/b/kaushal/archive/2015/05/27/client-certificate-authentication.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2015/05/27/client-certificate-authentication.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2015/05/27/client-certificate-authentication.aspx
orig_post_name:
  - client certificate authentication
  - client certificate authentication
  - client certificate authentication
orig_post_author_email:
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
total_views:
  - "937"
  - "937"
  - "937"
opengraph_tags:
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Client Certificate Authentication" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2015/05/27/client-certificate-authentication/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="SSL/TLS certificates are commonly used for both encryption and identification of the parties. In this blog post, I&#8217;ll be describing Client Certificate Authentication in brief. Client Certificate Authentication is a mutual certificate based authentication, where the client provides its Client Certificate to the Server to prove its identity. This happens as a part of the..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3173.060215_0710_ClientCerti1.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Client Certificate Authentication" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2015/05/27/client-certificate-authentication/" />
    <meta name="twitter:description" content="SSL/TLS certificates are commonly used for both encryption and identification of the parties. In this blog post, I&#8217;ll be describing Client Certificate Authentication in brief. Client Certificate Authentication is a mutual certificate based authentication, where the client provides its Client Certificate to the Server to prove its identity. This happens as a part of the..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3173.060215_0710_ClientCerti1.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Client Certificate Authentication" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2015/05/27/client-certificate-authentication/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="SSL/TLS certificates are commonly used for both encryption and identification of the parties. In this blog post, I&#8217;ll be describing Client Certificate Authentication in brief. Client Certificate Authentication is a mutual certificate based authentication, where the client provides its Client Certificate to the Server to prove its identity. This happens as a part of the..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3173.060215_0710_ClientCerti1.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Client Certificate Authentication" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2015/05/27/client-certificate-authentication/" />
    <meta name="twitter:description" content="SSL/TLS certificates are commonly used for both encryption and identification of the parties. In this blog post, I&#8217;ll be describing Client Certificate Authentication in brief. Client Certificate Authentication is a mutual certificate based authentication, where the client provides its Client Certificate to the Server to prove its identity. This happens as a part of the..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3173.060215_0710_ClientCerti1.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Client Certificate Authentication" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2015/05/27/client-certificate-authentication/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="SSL/TLS certificates are commonly used for both encryption and identification of the parties. In this blog post, I&#8217;ll be describing Client Certificate Authentication in brief. Client Certificate Authentication is a mutual certificate based authentication, where the client provides its Client Certificate to the Server to prove its identity. This happens as a part of the..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3173.060215_0710_ClientCerti1.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Client Certificate Authentication" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2015/05/27/client-certificate-authentication/" />
    <meta name="twitter:description" content="SSL/TLS certificates are commonly used for both encryption and identification of the parties. In this blog post, I&#8217;ll be describing Client Certificate Authentication in brief. Client Certificate Authentication is a mutual certificate based authentication, where the client provides its Client Certificate to the Server to prove its identity. This happens as a part of the..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3173.060215_0710_ClientCerti1.png" />
    
categories:
  - Uncategorized
---
<span style="font-family: Segoe UI;font-size: 10pt"><strong>SSL/TLS</strong> certificates are commonly used for both encryption and identification of the parties. In this blog post, I&#8217;ll be describing <strong>Client Certificate Authentication</strong> in brief.<br /> </span>

<span style="font-family: Segoe UI;font-size: 10pt"><strong>Client Certificate Authentication</strong> is a mutual certificate based authentication, where the client provides its Client Certificate to the Server to prove its identity. This happens as a part of the SSL Handshake (it is <span style="background-color: yellow"><strong>optional</strong></span>).<br /> </span>

<span style="font-family: Segoe UI;font-size: 10pt">Before we proceed further, we need to understand<br /> </span>

  * <span style="font-family: Segoe UI;font-size: 10pt">What is a client certificate?<br /> </span>
  * <span style="font-family: Segoe UI;font-size: 10pt">What is authentication & why do we need it?<br /> </span>

<div>
  <table style="border-collapse: collapse;background: #3b3838" border="0">
    <colgroup> <col style="width: 756px" /></colgroup> <tr>
      <td valign="middle" style="padding: 1px 7px 1px 7px">
        <span style="color: #00b0f0;font-family: Segoe UI;font-size: 18pt"><strong>Client Certificates</strong></span>
      </td>
    </tr>
  </table>
</div>

<span style="font-family: Segoe UI;font-size: 10pt"><strong> Client Certificate</strong> is a <em>digital certificate</em> which confirms to the <a href="http://en.wikipedia.org/wiki/X.509">X.509</a> system. It is used by client systems to prove their identity to the remote server. Here is a simple way to identify where a certificate is a client certificate or not:<br /> </span>

  * <span style="font-family: Segoe UI;font-size: 10pt">In the Details tab, the certificates intended purpose has the following text:<br /> &#8220;<strong>Proves your identity to a remote computer</strong>&#8221;<br /> </span>
  * <span style="font-family: Segoe UI;font-size: 10pt">Verify that the <strong>Enhanced Key Usage</strong> field of the certificate has the OID set to <strong>(1.3.6.1.5.5.7.3.2)</strong>.<br /> </span>

<span style="font-family: Segoe UI;font-size: 10pt">Below is a screenshot of a sample Client Certificate:<br /> </span>

<p style="text-align: center">
  <img src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3173.060215_0710_ClientCerti1.png" alt="" /><span style="font-family: Segoe UI;font-size: 10pt"><br /> </span>
</p>

<span style="font-family: Segoe UI;font-size: 10pt">Refer <a href="https://tools.ietf.org/html/rfc5246">RFC 5246</a><br /> </span>

<div>
  <table style="border-collapse: collapse;background: #3b3838" border="0">
    <colgroup> <col style="width: 756px" /></colgroup> <tr>
      <td valign="middle" style="padding: 1px 7px 1px 7px">
        <span style="color: #00b0f0;font-family: Segoe UI;font-size: 18pt"><strong>Authentication & Authorization </strong></span>
      </td>
    </tr>
  </table>
</div>

<span style="font-family: Segoe UI;font-size: 10pt">In Computer Science, <strong>Authentication</strong> is a mechanism used to prove the identity of the parties involved in a communication. It verifies that &#8220;<strong><em>you are who you say you are</em></strong>&#8220;. Not to be confused with <strong>Authorization</strong>, which is to verify that &#8220;<strong><em>you are permitted to do what you are trying to do</em></strong>&#8220;.<br /> </span>

<span style="font-family: Segoe UI;font-size: 10pt">There are several types of authentication. Here is a list of authentication widely used on <strong>IIS</strong> (<em>in no specific order</em>):<br /> </span>

  * <span style="font-family: Segoe UI;font-size: 10pt">Anonymous Authentication (No Authentication)<br /> </span>
  * <span style="font-family: Segoe UI;font-size: 10pt">Basic Authentication<br /> </span>
  * <span style="font-family: Segoe UI;font-size: 10pt">Client Certificate Authentication<br /> </span>
  * <span style="font-family: Segoe UI;font-size: 10pt">Digest Authentication<br /> </span>
  * <span style="font-family: Segoe UI;font-size: 10pt">Forms Authentication<br /> </span>
  * <span style="font-family: Segoe UI;font-size: 10pt">NTLM<br /> </span>
  * <span style="font-family: Segoe UI;font-size: 10pt">Kerberos<br /> </span>
  * <span style="font-family: Segoe UI;font-size: 10pt">Smart Card Authentication<br /> </span>

<div style="margin-left: 41pt">
  <table style="border-collapse: collapse;background: #e7e6e6" border="0">
    <colgroup> <col style="width: 568px" /></colgroup> <tr>
      <td valign="middle" style="border: solid #00b0f0 2.25pt;padding: 4px">
        <span style="font-family: Segoe UI;font-size: 10pt"><strong>NOTE</strong>: As the SSL Handshake happens before HTTP communication, <strong>Client Certificate Authentication </strong>takes the highest precedence over any other type of authentication that takes place over <strong>HTTP </strong>protocol.</span>
      </td>
    </tr>
  </table>
</div>

<span style="font-family: Segoe UI;font-size: 10pt"><strong>Kerberos</strong>, <strong>Client Certificate Authentication</strong> and <strong>Smart Card Authentication</strong> are examples for mutual authentication mechanisms. <strong>Authentication</strong> is typically used for access control, where you want to restrict the access to known users. <strong>Authorization</strong> on the other hand is used to determine the access level/privileges granted to the users.<br /> </span>

<span style="font-family: Segoe UI;font-size: 10pt">On <strong>Windows, </strong>a thread is the basic unit of execution. Any task performed by the user is executed by the thread under the context of a specific account/identity. <strong>Authentication</strong> is one of the ways used to determine the <strong>thread identity</strong>, whose privileges will be used by the thread for execution.<br /> </span>

<div>
  <table style="border-collapse: collapse;background: #3b3838" border="0">
    <colgroup> <col style="width: 756px" /></colgroup> <tr>
      <td valign="middle" style="padding: 1px 7px 1px 7px">
        <span style="color: #00b0f0;font-family: Segoe UI;font-size: 18pt"><strong>Client Certificate Authentication in SSL/TLS Handshake </strong></span>
      </td>
    </tr>
  </table>
</div>

<span style="font-family: Segoe UI;font-size: 10pt">I have already discussed SSL Handshake in one of my blog posts. Browse to:<br /> <a href="http://blogs.msdn.com/b/kaushal/archive/2013/08/03/ssl-handshake-and-https-bindings-on-iis.aspx">http://blogs.msdn.com/b/kaushal/archive/2013/08/03/ssl-handshake-and-https-bindings-on-iis.aspx</a><br /> </span>

<span style="font-family: Segoe UI;font-size: 10pt">Here is a screenshot describing the <strong>SSL/TLS Handshake</strong>:<br /> </span>

<p style="text-align: center">
  <img src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6574.060215_0710_ClientCerti2.png" alt="" /><span style="font-family: Segoe UI;font-size: 10pt"><br /> </span>
</p>

  * <span style="font-family: Segoe UI;font-size: 10pt">Client sends <strong>CLIENT HELLO</strong> as described in the above image<br /> </span>
  * <span style="font-family: Segoe UI;font-size: 10pt">Upon receiving the <strong>CLIENT HELLO</strong>, if the server is configured for <span style="background-color: yellow"><strong>Client Certificate Authentication</strong></span>, it will send a list of <span style="background-color: yellow"><strong>Distinguished CA names</strong></span> & <span style="background-color: yellow"><strong>Client Certificate Request</strong></span> to the client as a part of the <strong>SERVER HELLO </strong>apart from other details depicted above.<br /> </span>
  * <div>
      <span style="font-family: Segoe UI;font-size: 10pt">Upon receiving the Server Hello containing the <strong>Client Certificate request</strong> & list of <strong>Distinguished CA names</strong>, the client will perform the following steps:<br /> </span>
    </div>
    
    <ul style="margin-left: 72pt">
      <li>
        <span style="font-family: Segoe UI;font-size: 10pt">The client uses the CA list available in the <strong>SERVER HELLO</strong> to determine the mutually trusted CA certificates.<br /> </span>
      </li>
      <li>
        <span style="font-family: Segoe UI;font-size: 10pt">The<strong><br /> </strong>client will then determine the Client Certificates that have been issued by the mutually trusted <strong>Certification Authorities</strong>.<br /> </span>
      </li>
      <li>
        <span style="font-family: Segoe UI;font-size: 10pt">The client will then present the client certificate list to the user so that they can select a certificate to be sent to the user.<br /> </span>
      </li>
    </ul>

<div style="margin-left: 105pt">
  <table style="border-collapse: collapse;background: #e7e6e6" border="0">
    <colgroup> <col style="width: 510px" /></colgroup> <tr>
      <td style="padding-left: 7px;padding-right: 7px;border: solid #00b0f0 2.25pt">
        <span style="font-family: Segoe UI;font-size: 10pt"><strong>NOTE</strong>:<br /> </span></p> 
        
        <ul>
          <li>
            <span style="font-family: Segoe UI;font-size: 10pt">On the Client the Client Certificates must have a Private Key. If absent, then the certificate is ignored.<br /> </span>
          </li>
          <li>
            <span style="font-family: Segoe UI;font-size: 10pt">If the server doesn&#8217;t provide the list of <strong>Distinguished CA Names </strong>in the<strong> SERVER HELLO</strong>, then the client will present the user with all the client certificates that it has access to.</span>
          </li>
        </ul>
      </td>
    </tr>
  </table>
</div>

  * <div>
      <span style="font-family: Segoe UI;font-size: 10pt">Upon selection, the client responds with a<br /> </span>
    </div>
    
      * <span style="font-family: Segoe UI;font-size: 10pt"><strong>ClientKeyExchange</strong> message which contains the <strong>Pre-master secret</strong><br /> </span>
      * <span style="font-family: Segoe UI;font-size: 10pt"><span style="background-color: yellow"><strong>Certificate</strong></span> message which contains the <strong><span style="background-color: yellow">Client certificate</span><br /> </strong>(<em>Doesn&#8217;t contain the private key</em>).<br /> </span>
      * <span style="font-family: Segoe UI;font-size: 10pt"><strong><span style="background-color: yellow">CertificateVerify</span><br /> </strong>message, which is used to provide explicit verification of a client certificate. This message is sent only if the Client Certificate message was sent. The client is authenticated by using its private key to sign a hash of all the messages up to this point. The recipient verifies the signature using the public key of the signer, thus ensuring it was signed with the client&#8217;s private key. Refer <a href="https://tools.ietf.org/html/rfc5246">RFC 5246</a> for more details.<br /> </span>
  * <span style="font-family: Segoe UI;font-size: 10pt">Post this Client & Server use the random numbers and the <strong>Pre-Master</strong> secret to generate symmetric (or Master) keys which will used for encrypting & decrypting messages for further communication.<br /> </span>
  * <span style="font-family: Segoe UI;font-size: 10pt">Both respond with <strong>ChangeCipherSpec</strong> indicating that they have finished the process.<br /> </span>
  * <span style="font-family: Segoe UI;font-size: 10pt">SSL Handshake stands completed now and both the parties own a copy of the master key which can be used for encryption and decryption.<br /> </span>

<div>
  <table style="border-collapse: collapse;background: #3b3838" border="0">
    <colgroup> <col style="width: 756px" /></colgroup> <tr>
      <td valign="middle" style="padding: 1px 7px 1px 7px">
        <span style="color: #00b0f0;font-family: Segoe UI;font-size: 18pt"><strong>Design Problems</strong></span>
      </td>
    </tr>
  </table>
</div>

<span style="font-family: Segoe UI;font-size: 10pt">We know that the server sends the list of <strong>Distinguished CA names </strong>as a part of<strong> SERVER HELLO.</strong> The <strong>RFC</strong> never mandates the list of Distinguished CA Names should contain <strong>Root CA</strong> or <strong>Intermediate CA certificates</strong>. Here is a snippet of this section defined in the <strong>RFC5246</strong>:<br /> </span>

<div style="margin-left: 105pt">
  <table style="border-collapse: collapse;background: #e7e6e6" border="0">
    <colgroup> <col style="width: 548px" /></colgroup> <tr>
      <td style="padding-left: 7px;padding-right: 7px;border: solid #00b0f0 2.25pt">
        <span style="font-family: Courier New;font-size: 10pt"><strong>certificate_authorities<br /> </strong></span></p> 
        
        <p>
          <span style="font-family: Courier New;font-size: 10pt">A list of the distinguished names [<a href="https://tools.ietf.org/html/rfc5246">X501</a>] of acceptable<br /> certificate_authorities, represented in DER-encoded format. These<br /> distinguished names may specify a desired distinguished name for a<br /> root CA or for a subordinate CA; thus, this message can be used to<br /> describe known roots as well as a desired authorization space. If<br /> the certificate_authorities list is empty, then the client MAY<br /> send any certificate of the appropriate ClientCertificateType,<br /> unless there is some external arrangement to the contrary</span></td> </tr> </tbody> </table> </div> 
          
          <p>
            <span style="font-family: Segoe UI;font-size: 10pt">Refer the below blog post for information on Root & Intermediate CA certificates:<br /> <a href="http://blogs.msdn.com/b/kaushal/archive/2013/01/10/self-signed-root-ca-and-intermediate-ca-certificates.aspx">http://blogs.msdn.com/b/kaushal/archive/2013/01/10/self-signed-root-ca-and-intermediate-ca-certificates.aspx</a><br /> </span>
          </p>
          
          <p>
            <span style="font-family: Segoe UI;font-size: 10pt">This can lead to a problem where few systems require <strong>Root CA</strong>&#8216;s while few require <strong>Intermediate CA</strong>&#8216;s to be present in the list sent in the <strong>SERVER HELLO</strong>. This makes the communicating parties incompatible on certain occasions.<br /> </span>
          </p>
          
          <p>
            <span style="font-family: Segoe UI;font-size: 10pt">Both the implementations are debatable. On one hand the list sent by the server cannot exceed a certain limit (<em>on windows the size is 12,228 bytes</em>). If exceeded, the auth will fail. The list of Intermediate CA&#8217;s always exceeds the list of Root CA by 2-3 folds or even higher. This is one of the reasons why some systems send the ROOT CA&#8217;s in the list of <strong>Distinguished CA Names</strong>. On the other hand, the <strong>Intermediate CA</strong> names are readily available in the client certificate provided by the user, so it makes it easier during the certificate chain validation, therefore some systems prefer this over the previous one. Both have their own merits.<br /> </span>
          </p>
          
          <p>
            <span style="font-family: Segoe UI;font-size: 10pt">One example I have personally encountered is <strong>Apple</strong>&#8216;s <strong>Safari</strong> browser communicating to a site hosted on <strong>IIS 7 or higher</strong> which requires <strong>Client Certificate</strong> for authentication. <strong>Safari</strong> expects a list of <strong>Intermediate CA</strong>&#8216;s in the <strong>SERVER HELLO</strong>. On the other hand, IIS sends only <strong>Root CA</strong>&#8216;s in that list. As a result the authentication fails as the client is unable to provide a client certificate to the server.<br /> </span>
          </p>
          
          <p>
            <span style="font-family: Segoe UI;font-size: 10pt">A solution to the above problem is to configure IIS to not send any the CA list in the <strong>SERVER HELLO</strong>. To achieve this follow the Method 3 described in the support article below:<br /> <a href="https://support.microsoft.com/en-us/kb/933430/">https://support.microsoft.com/en-us/kb/933430/</a><br /> </span>
          </p>
          
          <p>
            <span style="font-family: Segoe UI;font-size: 10pt">The above article requires you to add a registry key, <strong>SendTrustedIssuerList</strong>, which is set to 0.<br /> </span>
          </p>
          
          <p>
            <span style="font-family: Segoe UI;font-size: 10pt">As a result the server doesn&#8217;t send any list to the client, but requires it to pass a client certificate. The client will present the complete list of client certificates to choose from and it will proceed further as expected.<br /> </span>
          </p>
          
          <div style="margin-left: 105pt">
            <table style="border-collapse: collapse;background: #e7e6e6" border="0">
              <colgroup> <col style="width: 548px" /></colgroup> <tr>
                <td style="padding-left: 7px;padding-right: 7px;border: solid #00b0f0 2.25pt">
                  <span style="font-family: Segoe UI;font-size: 10pt"><strong>NOTE</strong>: In Windows Server 2012 and Windows 8, changes were made to the underlying authentication process so that:<br /> </span></p> 
                  
                  <ul>
                    <li>
                      <span style="font-family: Segoe UI;font-size: 10pt">CTL-based trusted issuer list management is no longer supported.<br /> </span>
                    </li>
                    <li>
                      <span style="font-family: Segoe UI;font-size: 10pt">The behavior to send the Trusted Issuer List by default is off: Default value of the <strong>SendTrustedIssuerList</strong> registry key is now 0 (off by default) instead of 1.<br /> </span>
                    </li>
                    <li>
                      <span style="font-family: Segoe UI;font-size: 10pt">Compatibility to previous versions of Windows operating systems is preserved.<br /> </span>
                    </li>
                  </ul>
                  
                  <p>
                    <span style="font-family: Segoe UI;font-size: 10pt"><strong>Further read</strong>: https://technet.microsoft.com/en-in/library/hh831771.aspx</span></td> </tr> </tbody> </table> </div>