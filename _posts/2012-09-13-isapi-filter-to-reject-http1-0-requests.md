---
id: 121
title: ISAPI Filter to reject HTTP/1.0 requests
date: 2012-09-13T13:58:18+00:00
author: kaushal
layout: post
guid: https://blogs.msdn.microsoft.com/kaushal/2012/09/13/isapi-filter-to-reject-http1-0-requests/
permalink: /2012/09/13/isapi-filter-to-reject-http1-0-requests/
orig_url:
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2012/09/14/isapi-filter-to-reject-http-1-0-requests.aspx
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2012/09/14/isapi-filter-to-reject-http-1-0-requests.aspx
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2012/09/14/isapi-filter-to-reject-http-1-0-requests.aspx
orig_site_id:
  - "13803"
  - "13803"
  - "13803"
orig_post_id:
  - "10349233"
  - "10349233"
  - "10349233"
orig_parent_id:
  - "10349233"
  - "10349233"
  - "10349233"
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
  - http://blogs.msdn.com/b/kaushal/archive/2012/09/13/isapi-filter-to-reject-http1-0-requests.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2012/09/13/isapi-filter-to-reject-http1-0-requests.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2012/09/13/isapi-filter-to-reject-http1-0-requests.aspx
orig_post_name:
  - isapi filter to reject http 1 0 requests
  - isapi filter to reject http 1 0 requests
  - isapi filter to reject http 1 0 requests
orig_thread_id:
  - "820493"
  - "820493"
  - "820493"
orig_post_author_email:
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
orig_attachment_count:
  - "0"
  - "0"
  - "0"
total_views:
  - "7898"
  - "7898"
  - "7898"
opengraph_tags:
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="ISAPI Filter to reject HTTP/1.0 requests" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/09/13/isapi-filter-to-reject-http1-0-requests/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="There is a known problem on IIS where the IP Address is leaked in the content-location header of the HTTP response. There is a fix for this and its documented here: http://support.microsoft.com/kb/834141 The above KB also mentions that the issue might still occur even after using the above fix. It is discussed in detail in..." />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="ISAPI Filter to reject HTTP/1.0 requests" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/09/13/isapi-filter-to-reject-http1-0-requests/" />
    <meta name="twitter:description" content="There is a known problem on IIS where the IP Address is leaked in the content-location header of the HTTP response. There is a fix for this and its documented here: http://support.microsoft.com/kb/834141 The above KB also mentions that the issue might still occur even after using the above fix. It is discussed in detail in..." />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="ISAPI Filter to reject HTTP/1.0 requests" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/09/13/isapi-filter-to-reject-http1-0-requests/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="There is a known problem on IIS where the IP Address is leaked in the content-location header of the HTTP response. There is a fix for this and its documented here: http://support.microsoft.com/kb/834141 The above KB also mentions that the issue might still occur even after using the above fix. It is discussed in detail in..." />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="ISAPI Filter to reject HTTP/1.0 requests" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/09/13/isapi-filter-to-reject-http1-0-requests/" />
    <meta name="twitter:description" content="There is a known problem on IIS where the IP Address is leaked in the content-location header of the HTTP response. There is a fix for this and its documented here: http://support.microsoft.com/kb/834141 The above KB also mentions that the issue might still occur even after using the above fix. It is discussed in detail in..." />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="ISAPI Filter to reject HTTP/1.0 requests" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/09/13/isapi-filter-to-reject-http1-0-requests/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="There is a known problem on IIS where the IP Address is leaked in the content-location header of the HTTP response. There is a fix for this and its documented here: http://support.microsoft.com/kb/834141 The above KB also mentions that the issue might still occur even after using the above fix. It is discussed in detail in..." />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="ISAPI Filter to reject HTTP/1.0 requests" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/09/13/isapi-filter-to-reject-http1-0-requests/" />
    <meta name="twitter:description" content="There is a known problem on IIS where the IP Address is leaked in the content-location header of the HTTP response. There is a fix for this and its documented here: http://support.microsoft.com/kb/834141 The above KB also mentions that the issue might still occur even after using the above fix. It is discussed in detail in..." />
    
categories:
  - Uncategorized
---
<font size="2" face="Segoe UI">There is a known problem on IIS where the IP Address is leaked in the <strong>content-location</strong> header of the HTTP response. There is a fix for this and its documented here:</font>

<font size="2"></font> 

[<font size="2" face="Segoe UI">http://support.microsoft.com/kb/834141</font>](http://support.microsoft.com/kb/834141 "http://support.microsoft.com/kb/834141")

<font size="2"></font> 

<font size="2" face="Segoe UI">The above KB also mentions that the issue might still occur even after using the above fix. It is discussed in detail in the “<strong>Mitigating Factors</strong>” section. Below is a snippet from the above article:</font>

<font size="2" face="Segoe UI"></font><font size="2" face="Segoe UI"></font><font size="2" face="Segoe UI"></font> 

<table cellspacing="0" cellpadding="2" width="583" border="3">
  <tr>
    <td valign="top" width="581">
      <font size="4" face="Segoe UI"><strong>Mitigating Factors</strong></font> </p> 
      
      <p>
        <font face="Segoe UI"><font size="2"><font style="background-color: rgb(255, 255, 0);">After you set the <strong>UseHostName</strong> or <strong>SetHostName </strong>properties in IIS 6.0, it is still possible to see the server’s IP address in an HTTP response</font>. By default, this does not occur. It results from how the response is generated and sent. For example, if you configure an HTTP redirect that results in an HTTP 302 response being sent, and your redirect code uses the server’s IP address, the IP address may appear in the Content-Location or Location header of the response. To work around this issue, do not use the server’s IP address in the redirect logic. Instead, use its host name or fully qualified machine name.</font></font>
      </p>
      
      <p>
        <font face="Segoe UI"><font size="2"> A similar type of behavior can occur if you configure custom error pages to perform a REDIRECT operation and you use IIS Manager to set the redirect target as a URL instead of a file. In this scenario, specify the file instead of the URL to keep the IP address hidden. <br /> The server&#8217;s IP address can also be sent in an HTTP response if the following conditions are true: </font></font>
      </p>
      
      <ul>
        <li>
          <font face="Segoe UI"><font style="background-color: rgb(255, 255, 0);" color="#ff0000" size="2">The corresponding <strong>HTTP</strong> request did not include an <strong>HTTP</strong>:Host header value.</font></font>
        </li>
        <li>
          <font face="Segoe UI"><font style="background-color: rgb(255, 255, 0);" size="2"><font color="#ff0000">An ISAPI filter that makes a call to <strong>GetServerVariables</strong>(servername) during the <strong>SF_NOTIFY_PREPROC_HEADERS </strong>event is configured in IIS</font>.</font></font>
        </li>
      </ul>
      
      <p>
        <font face="Segoe UI"><font size="2"> </p> 
        
        <p>
          This is because <strong>PREPROC_HEADERS</strong> is called before IIS has read the configuration data; in this case, either UseHostName or SetHostName. Therefore, there is no other option but to return the IP address. If the request contains a Host value and the GetServerVariables(servername) call is made in PREPROC_HEADERS, SERVER_NAME will contain the value of the client&#8217;s Host header. HTTP/1.1 Web browsers must include a Host header in their requests. <font style="background-color: rgb(255, 255, 0);">Therefore, this scenario is much more likely to occur when the HTTP request is generated and sent by something other than a Web browser or when a Web browser uses HTTP/1.0.</font>
        </p>
        
        <p>
          </font></font></td> </tr> </tbody> </table> 
          
          <p>
            <font size="2" face="Segoe UI"></font>
          </p>
          
          <p>
            &#160;
          </p>
          
          <p>
            <font size="2" face="Segoe UI">So in real world the admins run a PCI scan on the server and it reports the server is vulnerable as it is leaking IP Address and suggests to follow the above support article.</font>
          </p>
          
          <p>
            <font size="2"></font>
          </p>
          
          <p>
            <font size="2" face="Segoe UI">However, even after applying the above fix, the issue is still seen as the scanners use a custom client which issue HTTP Requests over HTTP/1.0 protocol. <font style="background-color: rgb(255, 255, 0);">The problem is here with the protocol and not with the product</font>.</font>
          </p>
          
          <p>
            <font size="2"></font>
          </p>
          
          <p>
            <font size="2" face="Segoe UI">In the Mitigating factors section discussed above, it states 2 reasons why the issue is seen even after applying the fix. The first reason comes into picture for <strong>HTTP/1.0 </strong>protocol. There was a limitation in this protocol which assumed the client would send the <strong>hostname </strong>as a part of the <strong>HTTP Request</strong>, but never enforced it. This is the problem, since it assumes, if the incoming request doesn’t contain a hostname it would send back the response containing the <strong><font color="#ff0000">IP Address</font></strong> of the server in the <strong>content-location </strong>header. This issue shouldn’t be seen in<strong> HTTP/1.1 </strong>as it mandates that the client should send the hostname as part of the <strong>HTTP Request</strong>.</font>
          </p>
          
          <p>
            <font size="2"></font>
          </p>
          
          <p>
            <font size="2" face="Segoe UI">Now, the questions is what is the fix?</font>
          </p>
          
          <p>
            <font size="3" face="Segoe UI"><strong><font color="#008000" size="4">ANSWER</font></strong>: <font size="2">Reject all HTTP/1.0 requests. This is the ideal solution as HTTP/1.0 protocol is obsolete and none of the current day browsers use this version.</font></font>
          </p>
          
          <p>
            <font size="2" face="Segoe UI">Next questions is, how do we implement this on IIS?</font>
          </p>
          
          <p>
            <font size="3" face="Segoe UI"><strong><font color="#008000" size="4">ANSWER</font></strong>: <font size="2">Firstly, this issue is seen on all versions of IIS. As every server will support the protocol. So you will have to disable it. Going by the IIS versions,</font></font>
          </p>
          
          <p>
            <font size="3" face="Segoe UI"><strong><font size="4"><u>For IIS 7.0 and higher</u></font></strong>:</font>
          </p>
          
          <p>
            <font size="2" face="Segoe UI">Please refer the following blog on how to fix this issue on IIS 7.0 & higher:</font>
          </p>
          
          <p>
            <font size="2"></font>
          </p>
          
          <p>
            <a title="http://www.asprangers.com/post/2012/02/09/IIS-7-IP-Address-revealed-on-redirection-requests-on-HTTP10-protocol.aspx" href="http://www.asprangers.com/post/2012/02/09/IIS-7-IP-Address-revealed-on-redirection-requests-on-HTTP10-protocol.aspx"><font size="2" face="Segoe UI">http://www.asprangers.com/post/2012/02/09/IIS-7-IP-Address-revealed-on-redirection-requests-on-HTTP10-protocol.aspx</font></a>
          </p>
          
          <p>
            <font size="2"></font>
          </p>
          
          <p>
            <font size="2" face="Segoe UI">In the above article, they have used the <strong>URL Rewrite </strong>Module reject <strong>HTTP/1.0</strong> requests.</font>
          </p>
          
          <p>
            <font size="2"></font>
          </p>
          
          <p>
            <font size="2" face="Segoe UI">For IIS 6:</font>
          </p>
          
          <p>
            <font size="2"></font>
          </p>
          
          <p>
            <font size="2" face="Segoe UI">There is no simple solution available on IIS 6. One way is to write a isapi filter which would reject all incoming requests. Below is a sample code to do the same.</font>
          </p>
          
          <p>
            <font size="2"></font>
          </p>
          
          <ul>
            <font size="2"></font> </p> 
            
            <li>
              <font size="2" face="Segoe UI">Create a Empty C++ Project in Visual Studio 2005.</font>
            </li>
            <p>
              <font size="2"></font>
            </p>
            
            <li>
              <font size="2" face="Segoe UI">Add a .cpp file to the project and name it HttpVersionBlocker.cpp (or a name of your choice)</font>
            </li>
            <p>
              <font size="2"></font>
            </p>
            
            <li>
              <font size="2" face="Segoe UI">As we know, we need to define 2 important functions, GetFilterVersion and HttpFilterProc.</font>
            </li>
            <p>
              <font size="2"></font>
            </p>
            
            <li>
              <font size="2" face="Segoe UI">Below is the code snippet. Copy this to the above .cpp file</font>
            </li>
          </ul>
          
          <div id="codeSnippetWrapper" style="margin: 20px 0px 10px; padding: 4px; border: 1px solid silver; width: 97.16%; height: 600px; text-align: left; line-height: 12pt; overflow: auto; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; cursor: text; direction: ltr; max-height: 600px; background-color: rgb(244, 244, 244);">
            <div id="codeSnippet" style="padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: rgb(244, 244, 244);">
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: white;"><span style="color: rgb(204, 102, 51);">#include</span> &lt;afxcoll.h&gt;</pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: rgb(244, 244, 244);">#include&lt;stdio.h&gt;</pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: white;">#include&lt;afxisapi.h&gt;</pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: rgb(244, 244, 244);">#include&lt;afx.h&gt;</pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: white;">#include&lt;stdlib.h&gt;</pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: rgb(244, 244, 244);">&#160;</pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: white;"><span style="color: rgb(0, 128, 0);">//-------------------------------------------------------</span></pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: rgb(244, 244, 244);"><span style="color: rgb(0, 128, 0);">// This function is the entry point to the ISAPI Filter </span></pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: white;"><span style="color: rgb(0, 128, 0);">//-------------------------------------------------------</span></pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: rgb(244, 244, 244);">&#160;</pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: white;">BOOL WINAPI _stdcall GetFilterVersion(HTTP_FILTER_VERSION *pVer)</pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: rgb(244, 244, 244);">{</pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: white;">        pVer-&gt;dwFlags = (SF_NOTIFY_PREPROC_HEADERS ); </pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: rgb(244, 244, 244);">        pVer-&gt;dwFilterVersion = HTTP_FILTER_REVISION; </pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: white;">        strcpy_s(pVer-&gt;lpszFilterDesc, <span style="color: rgb(0, 96, 128);">"HTTP/1.0 Blocker"</span>); </pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: rgb(244, 244, 244);">        <span style="color: rgb(0, 0, 255);">return</span> <span style="color: rgb(0, 0, 255);">TRUE</span>; </pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: white;">}</pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: rgb(244, 244, 244);">&#160;</pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: white;"><span style="color: rgb(0, 128, 0);">//-------------------------------------------------------</span></pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: rgb(244, 244, 244);"><span style="color: rgb(0, 128, 0);">// This function will be invoked on every request </span></pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: white;"><span style="color: rgb(0, 128, 0);">//-------------------------------------------------------</span></pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: rgb(244, 244, 244);">&#160;</pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: white;">DWORD WINAPI __stdcall HttpFilterProc(HTTP_FILTER_CONTEXT *pfc, DWORD NotificationType, VOID *pvData) </pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: rgb(244, 244, 244);">{ </pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: white;">    <span style="color: rgb(0, 0, 255);">char</span> buffer[256];</pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: rgb(244, 244, 244);">    DWORD buffSize = <span style="color: rgb(0, 0, 255);">sizeof</span>(buffer);</pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: white;">    HTTP_FILTER_PREPROC_HEADERS *p;</pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: rgb(244, 244, 244);">&#160;</pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: white;">    <span style="color: rgb(0, 0, 255);">switch</span> (NotificationType)  </pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: rgb(244, 244, 244);">    {</pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: white;">      <span style="color: rgb(0, 0, 255);">case</span> SF_NOTIFY_PREPROC_HEADERS :</pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: rgb(244, 244, 244);">      p = (HTTP_FILTER_PREPROC_HEADERS *)pvData;</pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: white;">      BOOL bHeader = p-&gt;GetHeader(pfc,<span style="color: rgb(0, 96, 128);">"version"</span>,buffer,&buffSize); </pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: rgb(244, 244, 244);">      CString Version(buffer);</pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: white;">&#160;</pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: rgb(244, 244, 244);">      <span style="color: rgb(0, 0, 255);">if</span>(Version.Find(<span style="color: rgb(0, 96, 128);">"HTTP/1.0"</span>) != -1) </pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: white;">      {</pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: rgb(244, 244, 244);">            <span style="color: rgb(0, 128, 0);">// If HTTP/1.0 then Request, then change the URL</span></pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: white;">            p-&gt;SetHeader(pfc, <span style="color: rgb(0, 96, 128);">"url"</span>, <span style="color: rgb(0, 96, 128);">"/Rejected:HTTP/1.0_is_not_supported"</span>);</pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: rgb(244, 244, 244);">      }</pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: white;">      <span style="color: rgb(0, 0, 255);">return</span> SF_STATUS_REQ_HANDLED_NOTIFICATION; </pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: rgb(244, 244, 244);">    }</pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: white;">    <span style="color: rgb(0, 0, 255);">return</span> SF_STATUS_REQ_NEXT_NOTIFICATION; </pre>
              
              <p>
                <!--CRLF-->
              </p>
              
              <pre style="margin: 0em; padding: 0px; width: 100%; text-align: left; color: black; line-height: 12pt; overflow: visible; font-family: &quot;Courier New&quot;, courier, monospace; font-size: 8pt; direction: ltr; background-color: rgb(244, 244, 244);">}</pre>
              
              <p>
                <!--CRLF--></div> </div> 
                
                <ul>
                  <li>
                    <font size="2" face="Segoe UI">Go to Project properties and change the configuration type to Dynamic Library (.dll).</font>
                  </li>
                  <p>
                    <font size="2"></font>
                  </p>
                  
                  <li>
                    <font size="2" face="Segoe UI">Add a new file and call it HttpversionBlocker.def. copy paste the below section into it:</font>
                  </li>
                </ul>
                
                <table cellspacing="0" cellpadding="2" width="400" border="3">
                  <tr>
                    <td valign="top" width="400">
                      <p>
                        <font size="2" face="Courier New"><strong>LIBRARY "test"</strong></font>
                      </p>
                      
                      <p>
                        <font size="2"></font>
                      </p>
                      
                      <p>
                        <font size="2" face="Courier New"><strong>EXPORTS</strong></font>
                      </p>
                      
                      <p>
                        <font size="2"></font>
                      </p>
                      
                      <p>
                        <font size="2" face="Courier New"><strong>HttpFilterProc</strong></font>
                      </p>
                      
                      <p>
                        <font size="2"></font>
                      </p>
                      
                      <p>
                        <font size="2" face="Courier New"><strong>GetFilterVersion</strong></font>
                      </p>
                    </td>
                  </tr>
                </table>
                
                <ul>
                  <li>
                    <font size="2" face="Segoe UI">Build the project. </font>
                  </li>
                  <p>
                    <font size="2"></font>
                  </p>
                  
                  <li>
                    <font size="2" face="Segoe UI">This will generate the HttpVersionBlocker.dll </font>
                  </li>
                  <p>
                    <font size="2"></font>
                  </p>
                  
                  <li>
                    <font face="Segoe UI"><font size="2">Configure this as an Isapi filter in IIS. You can refer the below link to do this: </font><a href="http://www.microsoft.com/technet/prodtechnol/WindowsServer2003/Library/IIS/54c41c83-3723-4695-9bf1-9f7b1f674be0.mspx?mfr=true"><font size="2">Installing ISAPI Filters (IIS 6.0)</font></a></font>
                  </li>
                  <p>
                    <font size="2"></font></ul> 
                    
                    <p>
                      <font size="2"></font>
                    </p>
                    
                    <p>
                      <font face="Segoe UI"><font size="2">Alternatively, if one is not comfortable with coding there is another option. There is a 3rd party product that I’ve used in the past to achieve the same result. It is called WebKnight. Here is the link: </font><a title="http://www.aqtronix.com/?PageID=136" href="http://www.aqtronix.com/?PageID=136"><font size="2">http://www.aqtronix.com/?PageID=136</font></a><font size="2">.</font></font>
                    </p>
                    
                    <p>
                      <font size="2"></font>
                    </p>
                    
                    <p>
                      <font size="2" face="Segoe UI">This product is kind of a <strong>Application Firewall </strong>and can be used to block incoming requests on IIS.</font>
                    </p>
                    
                    <p>
                      <font size="2"></font>
                    </p>
                    
                    <p>
                      <font size="2" face="Segoe UI">The product can be downloaded freely, while they charge for the support.</font>
                    </p>
                    
                    <p>
                      <font size="2"></font>
                    </p>
                    
                    <p>
                      <font size="2" face="Segoe UI">You can try it at your own risk.</font>
                    </p>
                    
                    <p>
                      <font size="2"></font>
                    </p>
                    
                    <p>
                      <font size="2" face="Segoe UI">I don’t have much understanding of the product and neither do we support it so I’ll best leave it here.</font>
                    </p>
                    
                    <p>
                      <font size="2"></font>
                    </p>
                    
                    <p>
                      <font face="Segoe UI"></font>
                    </p>
                    
                    <p>
                      <font size="2"></font>
                    </p>
                    
                    <p>
                      <font style="background-color: rgb(165, 165, 165);" size="2" face="Segoe UI"><strong>NOTE: Neither of the solutions for IIS 6 is supported by Microsoft, as this is a problem with the protocol and not IIS.</strong></font>
                    </p>