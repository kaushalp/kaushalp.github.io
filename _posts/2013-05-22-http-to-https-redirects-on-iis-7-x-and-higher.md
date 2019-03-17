---
id: 222
title: HTTP to HTTPS redirects on IIS 7.x and higher
date: 2013-05-22T19:47:24+00:00
author: kaushal
layout: post
guid: https://blogs.msdn.microsoft.com/kaushal/2013/05/22/http-to-https-redirects-on-iis-7-x-and-higher/
permalink: /2013/05/22/http-to-https-redirects-on-iis-7-x-and-higher/
orig_url:
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2013/05/23/http-to-https-redirects-on-iis-7-x-and-higher.aspx
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2013/05/23/http-to-https-redirects-on-iis-7-x-and-higher.aspx
orig_site_id:
  - "13803"
  - "13803"
orig_post_id:
  - "10420774"
  - "10420774"
orig_parent_id:
  - "10420774"
  - "10420774"
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
  - http://blogs.msdn.com/b/kaushal/archive/2013/05/22/http-to-https-redirects-on-iis-7-x-and-higher.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2013/05/22/http-to-https-redirects-on-iis-7-x-and-higher.aspx
orig_post_name:
  - http to https redirects on iis 7 x and higher
  - http to https redirects on iis 7 x and higher
orig_thread_id:
  - "844411"
  - "844411"
orig_post_author_email:
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
orig_attachment_count:
  - "0"
  - "0"
total_views:
  - "271278"
  - "271278"
opengraph_tags:
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="HTTP to HTTPS redirects on IIS 7.x and higher" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2013/05/22/http-to-https-redirects-on-iis-7-x-and-higher/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="This is the most common requirement on most of the Exchange servers hosted on IIS. The server admins configure an http to https redirect. Today I will be discussing few ways of doing this. I will keep updating this document as I find more ways to do so. I am considering OWA as a sub..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8130.052313_0300_HTTPtoHTTPS1.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="HTTP to HTTPS redirects on IIS 7.x and higher" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2013/05/22/http-to-https-redirects-on-iis-7-x-and-higher/" />
    <meta name="twitter:description" content="This is the most common requirement on most of the Exchange servers hosted on IIS. The server admins configure an http to https redirect. Today I will be discussing few ways of doing this. I will keep updating this document as I find more ways to do so. I am considering OWA as a sub..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8130.052313_0300_HTTPtoHTTPS1.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="HTTP to HTTPS redirects on IIS 7.x and higher" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2013/05/22/http-to-https-redirects-on-iis-7-x-and-higher/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="This is the most common requirement on most of the Exchange servers hosted on IIS. The server admins configure an http to https redirect. Today I will be discussing few ways of doing this. I will keep updating this document as I find more ways to do so. I am considering OWA as a sub..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8130.052313_0300_HTTPtoHTTPS1.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="HTTP to HTTPS redirects on IIS 7.x and higher" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2013/05/22/http-to-https-redirects-on-iis-7-x-and-higher/" />
    <meta name="twitter:description" content="This is the most common requirement on most of the Exchange servers hosted on IIS. The server admins configure an http to https redirect. Today I will be discussing few ways of doing this. I will keep updating this document as I find more ways to do so. I am considering OWA as a sub..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8130.052313_0300_HTTPtoHTTPS1.png" />
    
categories:
  - IIS
  - redirect
  - URL Rewrite
  - Web App
---
<span style="font-size: 12pt;font-family: segoe ui"><strong><font style="background-color: #ffff00">***Updated post on 8th May 2017***</font></strong></span>

<span style="font-size: 12pt;font-family: segoe ui"><font size="2">This is the most common requirement on most of the Exchange servers hosted on IIS. The server admins configure an http to https redirect. </font></span>

<span style="font-size: 12pt;font-family: segoe ui"><font size="2">Today I will be discussing few ways of doing this. I will keep updating this document as I find more ways to do so. I am considering OWA as a sub application under IIS for all the below examples. Here is the structuring of the Web Site: </font></span>

<p style="margin-left: 81pt">
  <font size="2"><img alt="" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8130.052313_0300_HTTPtoHTTPS1.png" /><span style="font-family: segoe ui"> </span></font>
</p>

<span style="font-size: 12pt;font-family: segoe ui"><font size="2">In this case, we want all the requests (both <strong>HTTP</strong> & <strong>HTTPS</strong>) to be redirected on <strong>HTTPS</strong> to the application called &#8220;<strong>OWA</strong>&#8221; under the <strong>Default Web Site</strong>. </font></span>

# <span style="text-decoration: underline;font-family: segoe ui">Method 1: Using IIS URL Rewrite Module </span>

<span style="font-size: 12pt;font-family: segoe ui"><font size="2">For this you will have to install the <strong>URL Rewrite</strong> module. (<span style="background-color: yellow">FYI, this is available for IIS 7 and higher only</span>.) </font></span>

<span style="font-size: 12pt;font-family: segoe ui"><font size="2"><strong>Download from here</strong>: </font><a href="http://www.iis.net/downloads/microsoft/url-rewrite"><font size="2">http://www.iis.net/downloads/microsoft/url-rewrite</font></a><font size="2"> </font></span>

<span style="font-size: 12pt;font-family: segoe ui"><font size="2">Once installed, the <strong>URL Rewrite</strong> module would be listed under IIS section. There are few articles out there on this. Here are few to list: </font></span>

  1. [<span style="font-size: 12pt;font-family: segoe ui"><font size="2">http://www.sslshopper.com/iis7-redirect-http-to-https.html</font></span>](http://www.sslshopper.com/iis7-redirect-http-to-https.html)<span style="font-size: 12pt;font-family: segoe ui"><font size="2"> </font></span> 
      * [<span style="font-size: 12pt;font-family: segoe ui"><font size="2">http://www.jppinto.com/2010/03/automatically-redirect-http-requests-to-https-on-iis7-using-url-rewrite-2-0/</font></span>](http://www.jppinto.com/2010/03/automatically-redirect-http-requests-to-https-on-iis7-using-url-rewrite-2-0/)<span style="font-size: 12pt;font-family: segoe ui"><font size="2"> </font></span></ol> 
    <span style="font-size: 12pt;font-family: segoe ui"><font size="2">These articles are definitely a great repository, however I observed that they have not addressed an important factor. </font></span>
    
    <span style="font-size: 12pt;font-family: segoe ui"><font size="2">As specified in the above links add the below section in the web.config at the root of the site:</font></span>
    
    
    
    <div style="margin-left: 39pt">
      <font size="2"></font>
    </div>
    
    <span style="font-size: 12pt;font-family: segoe ui"><font size="2">In the above rule I&#8217;m checking whether the server variable &#8220;<strong>SERVER_PORT_SECURE</strong>&#8221; is set to <strong>1</strong> or <strong></strong>. (I&#8217;m doing a permanent redirect in the above URL, it can be changed accordingly as per the requirement)</font></span>
    
    <span style="font-size: 12pt;font-family: segoe ui"><font size="2">If you want to include the query string in the re-written url, then you can add <span style="color: #000000">appendQueryString=&#8221;true&#8221;</span> under the action section.</font></span>
    
    <span style="font-size: 12pt;font-family: segoe ui"><font size="2">You can find the complete list of IIS Server variables here: </font><a href="http://msdn.microsoft.com/en-us/library/ms524602(v=vs.90).aspx"><font size="2">http://msdn.microsoft.com/en-us/library/ms524602(v=vs.90).aspx</font></a><font size="2"> </font></span>
    
    > <table cellspacing="0" cellpadding="2" width="670" border="3">
    >   <tr>
    >     <td valign="top" width="149">
    >       <span style="font-size: 12pt;font-family: segoe ui;color: white"><strong><font color="#000000" size="2">SERVER_PORT_SECURE</font></strong></span>
    >     </td>
    >     
    >     <td valign="top" width="521">
    >       <span style="font-size: 12pt;font-family: segoe ui;color: white"><font size="2"><font color="#000000">A string that contains either 0 or 1. If the request is being handled on the secure port, then this is 1. Otherwise, it is 0.</font></font></span>
    >     </td>
    >   </tr>
    > </table>
    
    <span style="font-size: 12pt;font-family: segoe ui"><font size="2">Alternatively, instead of the above server variable the following server variable &#8220;<strong>HTTPS</strong>&#8221; and &#8220;<strong>SERVER_PORT</strong>&#8221; can also be used correspondingly. </font></span>
    
    <div style="margin-left: 39pt">
      <table style="background: #bfbfbf;border-collapse: collapse" border="0">
        <colgroup><font size="2"> </p> <col style="width: 750px"></font></colgroup> <tr style="height: 36px">
          <td style="padding-left: 9px;padding-right: 9px" valign="middle">
            <span style="font-family: segoe ui"><font size="2"><strong>NOTE</strong>: Ensure the rewrite rule is disabled at each of the virtual directories/applications under the Default Web Site. Due to inheritance, the rule will cause the requests to end up in infinite loop calling itself repeatedly.</font></span>
          </td>
        </tr>
      </table>
    </div>
    
![](https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/2671.052313_0300_HTTPtoHTTPS2.png)  <span style="font-family: segoe ui"></span>
    
    # <span style="text-decoration: underline;font-family: segoe ui">Method 2: Using IIS Default Document (a default.asp page) </span>
    
    <span style="font-size: 12pt;font-family: segoe ui">In this method we will introduce a sample asp page at the root of the website and then add the following piece of code: </span>
    
    
    
    <span style="font-size: 12pt;font-family: segoe ui"></span>&nbsp;
    
    <span style="font-family: segoe ui"></span>
    
    <span style="font-size: 12pt">Alternatively you could use the port numbers in the above code to achieve the same (<span style="background-color: yellow">ensure to change the port numbers as per the website configuration</span>).</span>
    
![](https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/7077.052313_0300_HTTPtoHTTPS3.png)  <span style="font-family: segoe ui"></span>
    
    # <span style="text-decoration: underline;font-family: segoe ui">Method 3: Using IIS HTTP Redirect Module </span>
    
    <span style="font-size: 12pt;font-family: segoe ui"><font size="2">This is one of the simplest methods, <span style="background-color: yellow">but has a lot of limitations and ideally not used</span>. Here is how we do it: </font></span>
    
    <span style="font-size: 12pt;font-family: segoe ui"><font size="2"><strong>PRE-REQUISITES: HTTP Redirect</strong> module is installed and the website has a valid <strong>HTTPS</strong> binding in place. </font></span>
    
      * <span style="font-size: 12pt;font-family: segoe ui"><font size="2">Launch the IIS Manager. </font></span> 
          * <span style="font-size: 12pt;font-family: segoe ui"><font size="2">Go to the <strong>HTTP Redirect</strong> module. </font></span> 
              * <div>
                  <span style="font-size: 12pt;font-family: segoe ui"><font size="2">Fill the details as per the requirement as shown below: </font></span>
                </div>
                
                <p style="margin-left: 4pt">
                  <font size="2"><img alt="" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/7455.052313_0300_HTTPtoHTTPS4.png" /><span style="font-size: 12pt;font-family: segoe ui"> </span></font>
                </p></ul> 
            
            <span style="font-size: 12pt;font-family: segoe ui"><font size="2">This may not be ideal for all the scenarios as the user is redirected to a specified URL. </font></span>
            
            <div style="margin-left: 44pt">
              <table style="background: #bfbfbf;border-collapse: collapse" border="0">
                <colgroup><font size="2"> </p> <col style="width: 822px"></font></colgroup> <tr style="height: 152px">
                  <td style="padding-left: 9px;padding-right: 9px" valign="middle">
                    <font size="2"><span style="font-family: segoe ui"><strong>NOTE</strong>: Ensure the enforced redirection is removed from each of the virtual directories/applications under the Default Web Site. Due to inheritance, the requests will end up in an endless loop, redirecting to itself repeatedly.</span> </font> </p> 
                    
                    <p>
                      <span style="font-family: segoe ui"><font size="2">Also ensure <strong>Require SSL</strong> is not checked at the Root of the website under <strong>SSL Settings</strong>, this may cause to throw an error page to the users when the browse the site over HTTP. It can be enforced at the application level.</font></span>
                    </p>
                  </td>
                </tr>
              </table>
            </div>
            
            <font size="2"><img alt="" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/5633.052313_0300_HTTPtoHTTPS5.png" /><span style="font-size: 12pt;font-family: segoe ui"> </span></font>
            
            <span style="font-size: 12pt;font-family: segoe ui"><font size="2">There is another way using custom error pages which has been documented here: </font></span>
            
              * [<span style="font-size: 12pt;font-family: segoe ui"><font size="2">http://www.sslshopper.com/iis7-redirect-http-to-https.html</font></span>](http://www.sslshopper.com/iis7-redirect-http-to-https.html)<span style="font-size: 12pt;font-family: segoe ui"><font size="2"> </font></span> 
                  * [<span style="font-size: 12pt;font-family: segoe ui"><font size="2">http://www.jppinto.com/2009/04/automatically-redirect-http-requests-to-https-iis-7/</font></span>](http://www.jppinto.com/2009/04/automatically-redirect-http-requests-to-https-iis-7/)<span style="font-size: 12pt;font-family: segoe ui"><font size="2"> </font></span></ul> 
                <span style="font-size: 12pt;font-family: segoe ui"><font size="2">The author in the 2<sup>nd</sup> link claims that it doesn&#8217;t work on IIS 7.5 and higher versions due to updates in the configuration security. </font></span>
                
                <span style="font-size: 12pt;font-family: segoe ui"><font size="2">I haven&#8217;t found the time to test and write it up and neither am I sure if the above actually works. Once I have tested I will add it up here.</font></span>