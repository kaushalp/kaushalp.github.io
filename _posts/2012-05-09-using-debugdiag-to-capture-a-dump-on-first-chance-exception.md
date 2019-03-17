---
id: 82
title: Using DebugDiag to capture a dump on First Chance Exception
date: 2012-05-09T00:35:52+00:00
author: kaushal
layout: post
guid: https://blogs.msdn.microsoft.com/kaushal/2012/05/09/using-debugdiag-to-capture-a-dump-on-first-chance-exception/
permalink: /2012/05/09/using-debugdiag-to-capture-a-dump-on-first-chance-exception/
orig_url:
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2012/05/09/using-debugdiag-to-capture-a-dump-on-first-chance-exception.aspx
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2012/05/09/using-debugdiag-to-capture-a-dump-on-first-chance-exception.aspx
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2012/05/09/using-debugdiag-to-capture-a-dump-on-first-chance-exception.aspx
orig_site_id:
  - "13803"
  - "13803"
  - "13803"
orig_post_id:
  - "10302908"
  - "10302908"
  - "10302908"
orig_parent_id:
  - "10302908"
  - "10302908"
  - "10302908"
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
  - http://blogs.msdn.com/b/kaushal/archive/2012/05/09/using-debugdiag-to-capture-a-dump-on-first-chance-exception.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2012/05/09/using-debugdiag-to-capture-a-dump-on-first-chance-exception.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2012/05/09/using-debugdiag-to-capture-a-dump-on-first-chance-exception.aspx
orig_post_name:
  - using debugdiag to capture a dump on first chance exception
  - using debugdiag to capture a dump on first chance exception
  - using debugdiag to capture a dump on first chance exception
orig_thread_id:
  - "807439"
  - "807439"
  - "807439"
orig_post_author_email:
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
orig_attachment_count:
  - "0"
  - "0"
  - "0"
total_views:
  - "23040"
  - "23040"
  - "23040"
opengraph_tags:
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Using DebugDiag to capture a dump on First Chance Exception" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/05/09/using-debugdiag-to-capture-a-dump-on-first-chance-exception/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="Capturing memory dumps is a most common ask while troubleshooting performance related issues with web applications. We generally use DebugDiag to do so. Not many are familiar with the tool and hence find it difficult to use it to capture the data. This time I’ll discuss how to use DebugDiag to generate memory dumps on..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4527.image_thumb_0AEBAF2D.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Using DebugDiag to capture a dump on First Chance Exception" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/05/09/using-debugdiag-to-capture-a-dump-on-first-chance-exception/" />
    <meta name="twitter:description" content="Capturing memory dumps is a most common ask while troubleshooting performance related issues with web applications. We generally use DebugDiag to do so. Not many are familiar with the tool and hence find it difficult to use it to capture the data. This time I’ll discuss how to use DebugDiag to generate memory dumps on..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4527.image_thumb_0AEBAF2D.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Using DebugDiag to capture a dump on First Chance Exception" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/05/09/using-debugdiag-to-capture-a-dump-on-first-chance-exception/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="Capturing memory dumps is a most common ask while troubleshooting performance related issues with web applications. We generally use DebugDiag to do so. Not many are familiar with the tool and hence find it difficult to use it to capture the data. This time I’ll discuss how to use DebugDiag to generate memory dumps on..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4527.image_thumb_0AEBAF2D.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Using DebugDiag to capture a dump on First Chance Exception" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/05/09/using-debugdiag-to-capture-a-dump-on-first-chance-exception/" />
    <meta name="twitter:description" content="Capturing memory dumps is a most common ask while troubleshooting performance related issues with web applications. We generally use DebugDiag to do so. Not many are familiar with the tool and hence find it difficult to use it to capture the data. This time I’ll discuss how to use DebugDiag to generate memory dumps on..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4527.image_thumb_0AEBAF2D.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Using DebugDiag to capture a dump on First Chance Exception" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/05/09/using-debugdiag-to-capture-a-dump-on-first-chance-exception/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="Capturing memory dumps is a most common ask while troubleshooting performance related issues with web applications. We generally use DebugDiag to do so. Not many are familiar with the tool and hence find it difficult to use it to capture the data. This time I’ll discuss how to use DebugDiag to generate memory dumps on..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4527.image_thumb_0AEBAF2D.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Using DebugDiag to capture a dump on First Chance Exception" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/05/09/using-debugdiag-to-capture-a-dump-on-first-chance-exception/" />
    <meta name="twitter:description" content="Capturing memory dumps is a most common ask while troubleshooting performance related issues with web applications. We generally use DebugDiag to do so. Not many are familiar with the tool and hence find it difficult to use it to capture the data. This time I’ll discuss how to use DebugDiag to generate memory dumps on..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4527.image_thumb_0AEBAF2D.png" />
    
categories:
  - Uncategorized
---
<font size="3" face="Segoe UI">Capturing memory dumps is a most common ask while troubleshooting performance related issues with web applications. We generally use <strong>DebugDiag </strong>to do so. Not many are familiar with the tool and hence find it difficult to use it to capture the data.</font>

<font face="Segoe UI"></font> 

<font size="3" face="Segoe UI">This time I’ll discuss how to use DebugDiag to generate memory dumps on First Chance Exceptions. Please go through the following blog if you want to know what a first chance exception is:</font>

<font face="Segoe UI"></font> 

[<font color="#0000ff" size="3" face="Segoe UI"><u>http://blogs.msdn.com/b/davidklinems/archive/2005/07/12/438061.aspx</u></font>](http://blogs.msdn.com/b/davidklinems/archive/2005/07/12/438061.aspx "http://blogs.msdn.com/b/davidklinems/archive/2005/07/12/438061.aspx")

<font face="Segoe UI"></font> 

<font size="3" face="Segoe UI"></font>

<font size="3" face="Segoe UI">I’ll be using <strong>DebugDiag v1.2, </strong>below is the download link:</font>

<font face="Segoe UI"></font> 

[<font color="#0000ff" size="3" face="Segoe UI"><u>http://www.microsoft.com/en-us/download/details.aspx?id=26798</u></font>](http://www.microsoft.com/en-us/download/details.aspx?id=26798 "http://www.microsoft.com/en-us/download/details.aspx?id=26798")

<font face="Segoe UI"></font> 

<font face="Segoe UI"><font size="3"></font></font>

<font face="Segoe UI"><font size="3">Download and install the tool corresponding to the bitness of the server and not the process i.e., </font><font size="3">for 32 bit machines download <strong>x86</strong> and for <strong>64</strong> bit download x64. </font></font>

<font face="Segoe UI"></font> 

<font size="3" face="Segoe UI">The default installation folder is “<strong><u><font color="#0000ff">C:\Program Files\DebugDiag</font></u></strong>”</font>

<font size="3" face="Segoe UI"></font>

<font face="Segoe UI"></font><font face="Segoe UI"></font><font face="Segoe UI"></font><font face="Segoe UI"></font><font face="Segoe UI"></font> 

<table style="background: rgb(192, 192, 192);" cellspacing="0" cellpadding="2" width="558" align="center" border="1">
  <tr>
    <td valign="top" width="556">
      <font face="Segoe UI"></font> </p> 
      
      <p align="justify">
        <font size="3"><font face="Segoe UI"><strong>NOTE</strong>: Please ensure you have sufficient disk space when using <strong>DebugDiag </strong>to capture memory dump. The dump files are as big as the process. So if you have a process consuming 600 MB, the dump file would around ~600 MB. If there are many files created then you are running at the risk of crashing the server due to insufficient disk space.</font></font>
      </p>
      
      <p>
        <font face="Segoe UI"></font></td> </tr> </tbody> </table> 
        
        <p>
          <font face="Segoe UI"></font>
        </p>
        
        <p>
          <font size="3" face="Segoe UI">There are 2 ways to capture <strong>FIRST CHANCE EXCEPTION </strong>dumps of a process.</font>
        </p>
        
        <p>
          <font face="Segoe UI"></font>
        </p>
        
        <ul>
          <font face="Segoe UI"></font> </p> 
          
          <li>
            <font size="3"><font face="Segoe UI"><strong>Method 1</strong>: Generate a dump for all First Chance Exception or</font></font>
          </li>
        </ul>
        
        <p>
          <font size="3" face="Segoe UI"></font>
        </p>
        
        <ul>
          <font face="Segoe UI"></font> </p> 
          
          <li>
            <font size="3"><font face="Segoe UI"><strong>Method 2</strong>: Target a specific First chance exception (<strong>Recommended</strong>)</font></font>
          </li>
          <p>
            <font face="Segoe UI"></font></ul> 
            
            <p>
              <font face="Segoe UI"></font>
            </p>
            
            <p>
              <font size="5" face="Segoe UI"><strong></strong></font>
            </p>
            
            <p>
              <font size="5" face="Segoe UI"><strong>Method 1: Generate a dump for all First Chance Exception</strong></font>
            </p>
            
            <p>
              <font face="Segoe UI"></font>
            </p>
            
            <p>
              <font size="2"><font size="3" face="Segoe UI">This is the easiest way to capture a dump for any exception that is raised within the process, However this captures unnecessary data and a lot of junk data is generated and hence is never recommended. Below are the steps to configure the same:</font></font>
            </p>
            
            <p>
              <font face="Segoe UI"></font>
            </p>
            
            <ol>
              <font face="Segoe UI"></font> </p> 
              
              <li>
                <font size="3" face="Segoe UI">Launch DebugDiag <br /></font>
              </li>
              <p>
                <font face="Segoe UI"></font>
              </p>
              
              <li>
                <font size="3" face="Segoe UI">In the <strong>Rules</strong> tab select <strong>Crash</strong> and click on <strong>Next</strong></font>.<a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3022.image_34FBD322.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/3022.image_5F00_34FBD322.png"><font face="Segoe UI"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4527.image_thumb_0AEBAF2D.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/4527.image_5F00_thumb_5F00_0AEBAF2D.png" width="426" height="375" /></font></a>
              </li>
              <p>
                <font face="Segoe UI">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </font>
              </p>
              
              <li>
                <font face="Segoe UI"><font size="3">In “<strong>Select Target Type</strong>” </font><font size="3">select “<strong>A specific process</strong>” and click on <strong>Next</strong>.</font></font><a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3750.image_684770B1.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/3750.image_5F00_684770B1.png"><font face="Segoe UI"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/4034.image_thumb_11DB3BE5.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/4034.image_5F00_thumb_5F00_11DB3BE5.png" width="432" height="379" /></font></a>
              </li>
              <p>
                <font face="Segoe UI"></font>
              </p>
              
              <p>
                <font size="3"><font style="background-color: rgb(255, 255, 0);"><font face="Segoe UI"><strong>Note</strong>: I<font size="3">f the target is a web application hosted on IIS then, choose either “<strong>A</strong></font><font size="3"><strong>ll IIS/COM+ related processes</strong>” or “</font><font size="3"><strong>A specific IIS web application pool</strong>”. </font></font></font></font>
              </p>
              
              <p>
                <font face="Segoe UI"></font>
              </p>
              
              <li>
                <font size="3"><font face="Segoe UI">In “<strong>Select Target</strong>” select the target process and click on <strong>Next</strong>.&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; <br />&#160;&#160;&#160;&#160;&#160;&#160;&#160; </font><a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/8712.image_089F00A4.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/8712.image_5F00_089F00A4.png"><font face="Segoe UI"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/2451.image_thumb_4DD757CD.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/2451.image_5F00_thumb_5F00_4DD757CD.png" width="436" height="382" /></font></a><font face="Segoe UI">&#160;&#160;&#160;&#160;&#160; </font></font>
              </li>
              <li>
                <font size="3" face="Segoe UI">In “<strong>Advanced Configuration (Optional)</strong>” under “<strong>Unconfigured First Chance Exceptions</strong>” set the following: <br /></font>
              </li>
              <p>
                <font face="Segoe UI"></font>
              </p>
              
              <ol>
                <font face="Segoe UI"></font> </p> 
                
                <li>
                  <font size="3"><font face="Segoe UI"><strong>Action type for unconfigured first chance exceptions</strong>: <font style="background-color: rgb(255, 255, 0);">Full Userdump</font></font></font>
                </li>
                <p>
                  <font face="Segoe UI"></font>
                </p>
                
                <li>
                  <font size="3"><font face="Segoe UI"><strong>Action Limit for unconfigured first chance exceptions</strong>: </font><font style="background-color: rgb(255, 255, 0);"><font face="Segoe UI">10<font style="background-color: rgb(255, 255, 0);"> </font> 
                  
                  <p>
                    </font><font style="background-color: rgb(255, 255, 255);"><a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3835.image_4B4E260F.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/3835.image_5F00_4B4E260F.png"><font face="Segoe UI"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/1781.image_thumb_29824D7E.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/1781.image_5F00_thumb_5F00_29824D7E.png" width="455" height="401" /></font></a>&#160;<font color="#ff0000" face="Segoe UI"></font></font></font></font></li> 
                    
                    <p>
                      <font face="Segoe UI"></font></ol> 
                      
                      <p>
                        <font face="Segoe UI"></font>
                      </p>
                      
                      <li>
                        <font size="3" face="Segoe UI">Click on <strong>Next </strong>twice and then click on <strong>Finish </strong>to activate the rule.</font>
                      </li>
                      <p>
                        <font face="Segoe UI"></font></ol> 
                        
                        <p>
                          <font face="Segoe UI"></font>
                        </p>
                        
                        <p>
                          <font size="3" face="Segoe UI">This will generate a dump for any unconfigured exception that may occur inside the target process. The file name will be in the following format:</font>
                        </p>
                        
                        <p>
                          <font face="Segoe UI"></font>
                        </p>
                        
                        <p>
                          <font style="background-color: rgb(204, 204, 204);"><font face="Segoe UI"><strong><ProcessName></strong>__<strong><ApplicationPool></strong>__PID__<strong><PIDValue></strong>__Date__<strong><DateValue></strong>__Time_<strong><TimeValue></strong>__First chance exception <strong><Exception_Code></strong>.dmp</font></font>
                        </p>
                        
                        <p>
                          <font face="Segoe UI"></font>
                        </p>
                        
                        <p>
                          <font size="3"><font face="Segoe UI"><strong>Example</strong>:</font></font>
                        </p>
                        
                        <p>
                          <font face="Segoe UI"></font>
                        </p>
                        
                        <p>
                          <font size="2" face="Segoe UI"><strong>w3wp__DefaultAppPool__PID__10032__Date__05_09_2012__Time_12_52_51PM__406__First chance exception <font style="background-color: rgb(255, 255, 0);" color="#ff0000">0XE0434352</font>.dmp</strong></font>
                        </p>
                        
                        <p>
                          <font face="Segoe UI"></font>
                        </p>
                        
                        <p>
                          <font size="5" face="Segoe UI"><strong>Method 2: Target a specific First Chance Exception (Recommended)</strong></font>
                        </p>
                        
                        <p>
                          <font face="Segoe UI"></font>
                        </p>
                        
                        <p>
                          <font size="3" face="Segoe UI">Follow the above method until step 5. Here we will target a specific First Chance Exception. I will be targeting OOM exception for my example/</font>
                        </p>
                        
                        <p>
                          <font face="Segoe UI"></font>
                        </p>
                        
                        <ol>
                          <font face="Segoe UI"></font> </p> 
                          
                          <li>
                            <font size="3"><font face="Segoe UI">In “<strong>Advanced Configuration (Optional)</strong>” click on the <strong>Exceptions…</strong> button. 
                            
                            <p>
                              </font><a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6428.image59_5438641B.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/6428.image59_5F00_5438641B.png"><font face="Segoe UI"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/2046.image59_thumb_475E0DFD.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/2046.image59_5F00_thumb_5F00_475E0DFD.png" width="498" height="436" /></font></a><font face="Segoe UI"> <br /></font></font></li> 
                              
                              <p>
                                <font face="Segoe UI"></font>
                              </p>
                              
                              <li>
                                <font size="3" face="Segoe UI">In “<strong>First chance Exception Configuration</strong>” click on “<strong>Add Exception…</strong>” <br /></font>
                              </li>
                              <p>
                                <font face="Segoe UI"></font>
                              </p>
                              
                              <li>
                                <font size="3" face="Segoe UI">In “<strong>Configure Exception</strong>” select the Exception code from the LHS and since we are targeting OOM, specify the details as shown below: <br /></font>
                              </li>
                              <p>
                                <font face="Segoe UI"></font>
                              </p>
                              
                              <ol>
                                <font face="Segoe UI"></font> </p> 
                                
                                <li>
                                  <font size="3"><font face="Segoe UI"><strong>.NET Exception Type</strong>: <font style="background-color: rgb(255, 255, 0);">System.OutOfMemoryException</font></font></font>
                                </li>
                                <p>
                                  <font face="Segoe UI"></font>
                                </p>
                                
                                <li>
                                  <font size="3"><font face="Segoe UI"><strong>Action Type</strong>: <font style="background-color: rgb(255, 255, 0);">Full Userdump</font> </font></font>
                                </li>
                                <p>
                                  <font face="Segoe UI"></font>
                                </p>
                                
                                <li>
                                  <font size="3"><font face="Segoe UI"><strong>Action Limit</strong>: </font><font style="background-color: rgb(255, 255, 0);" face="Segoe UI">3 <br /></font></font>
                                </li>
                                <p>
                                  <font face="Segoe UI"></font></ol> 
                                  
                                  <p>
                                    <font face="Segoe UI"></font><a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/3438.image_7635EE47.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/3438.image_5F00_7635EE47.png"><font face="Segoe UI"><img title="image" style="margin-right: auto; margin-left: auto; float: none; display: block; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/0218.image_thumb_2D2FCC81.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/0218.image_5F00_thumb_5F00_2D2FCC81.png" width="500" height="418" /></font></a><font face="Segoe UI"> </p> 
                                    
                                    <p>
                                      <font size="3"><strong>NOTE</strong>: The Exception type is case sensitive. Ensure it is entered correctly. For more details please visit the following link: </font></font><a title="http://msdn.microsoft.com/en-us/library/system.systemexception.aspx" href="http://msdn.microsoft.com/en-us/library/system.systemexception.aspx"><font color="#0000ff" size="3" face="Segoe UI"><u>http://msdn.microsoft.com/en-us/library/system.systemexception.aspx</u></font></a><font face="Segoe UI"> <br /></font>
                                    </p>
                                    
                                    <li>
                                      <font size="3" face="Segoe UI">Click on <strong>Ok</strong> and then click on “<strong>Save & Close</strong>”. <br clear="all" /></font>
                                    </li>
                                    <p>
                                      <font face="Segoe UI"></font>
                                    </p>
                                    
                                    <li>
                                      <font size="3" face="Segoe UI">Click on <strong>Next </strong>twice and then click on <strong>Finish </strong>to activate the rule. <br /></font>
                                    </li></ol> 
                                    
                                    <p>
                                      <font size="3" face="Segoe UI">The dumps created by this rule will be in the following format:</font>
                                    </p>
                                    
                                    <p>
                                      <font face="Segoe UI"></font>
                                    </p>
                                    
                                    <p>
                                      <font style="background-color: rgb(204, 204, 204);"><font size="2"><font face="Segoe UI"><strong><ProcessName></strong>__PID__<strong><PID></strong>__Date__<strong><DateValue></strong>__Time_<strong><TimeValue></strong>__First Chance <strong><ExceptionName></strong>.dmp</font></font></font>
                                    </p>
                                    
                                    <p>
                                      <font face="Segoe UI"></font>
                                    </p>
                                    
                                    <p>
                                      <font size="3"><font face="Segoe UI"><strong>Example</strong>:</font></font>
                                    </p>
                                    
                                    <p>
                                      <font face="Segoe UI"></font>
                                    </p>
                                    
                                    <p>
                                      <font size="2" face="Segoe UI"><strong>w3wp__PID__2364__Date__05_09_2012__Time_12_59_51PM__406__First Chance <font style="background-color: rgb(255, 255, 0);" color="#ff0000">System.OutOfMemoryException</font>.dmp</strong></font>
                                    </p>
                                    
                                    <p>
                                      <font face="Segoe UI"></font>
                                    </p>
                                    
                                    <p>
                                      &#160;
                                    </p>
                                    
                                    <p>
                                      <font face="Segoe UI"></font><font face="Segoe UI"></font><font face="Segoe UI"></font><font face="Segoe UI"></font><font face="Segoe UI"></font>
                                    </p>
                                    
                                    <table style="background: rgb(192, 192, 192);" cellspacing="0" cellpadding="2" width="531" align="center" border="1">
                                      <tr>
                                        <td valign="top" width="529">
                                          <font face="Segoe UI"></font> </p> 
                                          
                                          <p align="justify">
                                            <font size="3"><font face="Segoe UI"><strong>NOTE</strong>: DebugDiag help menu already has documented steps on how to gather data in most of the scenarios. It is preferable to refer that.</font></font>
                                          </p>
                                          
                                          <p>
                                            <font face="Segoe UI"></font></td> </tr> </tbody> </table> 
                                            
                                            <p>
                                              <font face="Segoe UI"></font>
                                            </p>
                                            
                                            <p>
                                              <font size="3" face="Segoe UI">Hope this helps. Until then. Adios! <img class="wlEmoticon wlEmoticon-smile" alt="Smile" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/1460.wlEmoticon-smile_0293EBA4.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/1460.wlEmoticon_2D00_smile_5F00_0293EBA4.png" /></font>
                                            </p>
                                            
                                            <p>
                                              <font face="Segoe UI"></font>
                                            </p>