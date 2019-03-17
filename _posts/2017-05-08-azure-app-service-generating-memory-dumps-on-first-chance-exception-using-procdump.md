---
id: 1787
title: 'Azure App Service: Generating memory dumps on first chance exception using Procdump'
date: 2017-05-08T21:00:45+00:00
author: Kaushal Kumar Panday
layout: post
guid: https://blogs.msdn.microsoft.com/kaushal/?p=1787
permalink: /2017/05/08/azure-app-service-generating-memory-dumps-on-first-chance-exception-using-procdump/
opengraph_tags:
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Azure App Service: Generating memory dumps on first chance exception using Procdump" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2017/05/08/azure-app-service-generating-memory-dumps-on-first-chance-exception-using-procdump/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="In one of my older posts, I have explained on how we can generate memory dumps on first chance exceptions using Debug Diag. In certain scenarios where the users do not have permissions to install tools, users have to look for alternate options. For example, in Azure App Service, the users do not have permissions..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2017/05/image_thumb121.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Azure App Service: Generating memory dumps on first chance exception using Procdump" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2017/05/08/azure-app-service-generating-memory-dumps-on-first-chance-exception-using-procdump/" />
    <meta name="twitter:description" content="In one of my older posts, I have explained on how we can generate memory dumps on first chance exceptions using Debug Diag. In certain scenarios where the users do not have permissions to install tools, users have to look for alternate options. For example, in Azure App Service, the users do not have permissions..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2017/05/image_thumb121.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Azure App Service: Generating memory dumps on first chance exception using Procdump" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2017/05/08/azure-app-service-generating-memory-dumps-on-first-chance-exception-using-procdump/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="In one of my older posts, I have explained on how we can generate memory dumps on first chance exceptions using Debug Diag. In certain scenarios where the users do not have permissions to install tools, users have to look for alternate options. For example, in Azure App Service, the users do not have permissions..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2017/05/image_thumb121.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Azure App Service: Generating memory dumps on first chance exception using Procdump" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2017/05/08/azure-app-service-generating-memory-dumps-on-first-chance-exception-using-procdump/" />
    <meta name="twitter:description" content="In one of my older posts, I have explained on how we can generate memory dumps on first chance exceptions using Debug Diag. In certain scenarios where the users do not have permissions to install tools, users have to look for alternate options. For example, in Azure App Service, the users do not have permissions..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2017/05/image_thumb121.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Azure App Service: Generating memory dumps on first chance exception using Procdump" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2017/05/08/azure-app-service-generating-memory-dumps-on-first-chance-exception-using-procdump/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="In one of my older posts, I have explained on how we can generate memory dumps on first chance exceptions using Debug Diag. In certain scenarios where the users do not have permissions to install tools, users have to look for alternate options. For example, in Azure App Service, the users do not have permissions..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2017/05/image_thumb121.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Azure App Service: Generating memory dumps on first chance exception using Procdump" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2017/05/08/azure-app-service-generating-memory-dumps-on-first-chance-exception-using-procdump/" />
    <meta name="twitter:description" content="In one of my older posts, I have explained on how we can generate memory dumps on first chance exceptions using Debug Diag. In certain scenarios where the users do not have permissions to install tools, users have to look for alternate options. For example, in Azure App Service, the users do not have permissions..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2017/05/image_thumb121.png" />
    
categories:
  - Azure
  - Azure App Service
  - Azure Web App
  - Azure Websites
  - dump
  - dumps
  - exception
  - first chance exception
  - IIS
  - memory
  - procdump
---
In one of my older [posts](https://blogs.msdn.microsoft.com/kaushal/2012/05/09/using-debugdiag-to-capture-a-dump-on-first-chance-exception/), I have explained on how we can generate memory dumps on first chance exceptions using **[Debug Diag](https://www.microsoft.com/en-us/download/details.aspx?id=49924)**. In certain scenarios where the users do not have permissions to install tools, users have to look for alternate options. For example, in **Azure App Service**, the users do not have permissions to install anything on the VM. 

However, Azure App Service provides the KUDU console, using which the users can use a command line utility like [procdump.exe](https://technet.microsoft.com/en-in/sysinternals/dd996900.aspx) to generate memory dumps. We can also use procdump to generate memory dumps on _**first chance exception**_ using the below command:

> <table cellspacing="0" cellpadding="2" width="613" border="2">
>   <tr>
>     <td bgcolor="#003300" valign="top" width="609">
>       <p align="left">
>         <font style="background-color: #cccccc" size="2" face="Courier New"></font><font color="#00ff00" size="2" face="Courier New">procdump.exe -accepteula -ma <strong>-e 1 -f</strong> &#8220;<Exception Name>&#8221; <Process ID></font>
>       </p>
>     </td>
>   </tr>
>   
>   <tr>
>     <td bgcolor="#003300" valign="top" width="609">
>       <p>
>         <font color="#ffffff" size="2">where,<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <strong>-ma</strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Write a dump file with all process memory. The default dump format only includes<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; thread and handle information<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <strong>-accepteula</strong>&nbsp;&nbsp; Use this switch to automatically accept the Sysinternals license agreement.</font>
>       </p>
>       
>       <p>
>         <font color="#ffffff"><font size="2">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <strong>-e</strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Write a dump when the process encounters an unhandled exception. Include the&nbsp; <br /></font><font size="2">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <strong>1</strong> to create dump on first chance exceptions.</font></font>
>       </p>
>       
>       <p>
>         <font color="#ffffff" size="2">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <strong>-f</strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Filter the first chance exceptions. Wildcards (*) are supported. To just display <br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; the names without dumping, use a blank (&#8220;&#8221;) filter</font>
>       </p>
>     </td>
>   </tr>
> </table>

<font size="2">Azure App Service instances include the sysinternals suite in the default image. They can be located here via the KUDU console: <font style="background-color: #cccccc" face="Courier New">D:\devtools\sysinternals</font></font> 

<font size="2">The users may also download ProcDump from </font>[<font size="2">here</font>](https://live.sysinternals.com/procdump.exe) <font size="2">and upload it a specific location such as <font style="background-color: #cccccc" face="Courier New">D:\home\Dumps</font> and use it. </font> 

<font size="2">You would need to determine the process ID of the process against which procdump would be executed. You can determine that by navigating to the Process explorer in the KUDU console as shown below: (<em>Note the PID of the w3wp process without the SCM tag</em>)</font> 

[<img title="image" style="border-left-width: 0px;border-right-width: 0px;border-bottom-width: 0px;padding-top: 0px;padding-left: 0px;padding-right: 0px;border-top-width: 0px" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/2017/05/image_thumb121.png" width="833" height="168" />](https://msdnshared.blob.core.windows.net/media/2017/05/image120.png) 

<font size="2">Here is an example<font face="Courier New">:</font></font> 

> <table cellspacing="0" cellpadding="2" width="700" bgcolor="#000000" border="2">
>   <tr>
>     <td bgcolor="#000000" valign="top" width="696">
>       <p>
>         <font color="#ffffff"><font face="Consolas"><font size="2">D:\home\Dumps><font color="#00ff00">procdump.exe -accepteula -ma -e 1 -f &#8220;System.UnauthorizedAccessException&#8221; 7808</font></font> </font></font>
>       </p>
>       
>       <p>
>         <font color="#ffffff" size="2" face="Consolas">ProcDump v8.2 &#8211; Sysinternals process dump utility<br /></font><font color="#ffffff"><font face="Consolas"><font size="2">Copyright (C) 2009-2016 Mark Russinovich and Andrew Richards<br /></font><font size="2">Sysinternals &#8211; </font></font></font><a href="http://www.sysinternals.com"><font color="#ffffff" size="2" face="Consolas">www.sysinternals.com</font></a><font color="#ffffff" face="Consolas"> </font>
>       </p>
>       
>       <p>
>         <font color="#ffffff" size="2" face="Consolas">Process:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; w3wp.exe (7808)<br /></font><font color="#ffffff" size="2" face="Consolas">Process image:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; D:\Windows\SysWOW64\inetsrv\w3wp.exe<br /></font><font color="#ffffff" size="2" face="Consolas">CPU threshold:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; n/a<br /></font><font color="#ffffff" size="2" face="Consolas">Performance counter:&nbsp;&nbsp; n/a<br /></font><font color="#ffffff" size="2" face="Consolas">Commit threshold:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; n/a<br /></font><font color="#ffffff" size="2" face="Consolas">Threshold seconds:&nbsp;&nbsp;&nbsp;&nbsp; n/a<br /></font><font color="#ffffff" size="2" face="Consolas">Hung window check:&nbsp;&nbsp;&nbsp;&nbsp; Disabled<br /></font><font color="#ffffff" size="2" face="Consolas">Log debug strings:&nbsp;&nbsp;&nbsp;&nbsp; Disabled<br /></font><font color="#ffffff" size="2" face="Consolas">Exception monitor:&nbsp;&nbsp;&nbsp;&nbsp; <font color="#ff0000">First Chance+Unhandled</font><br /></font><font color="#ffffff" size="2" face="Consolas">Exception filter:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; [Includes]<br /></font><font color="#ffffff" size="2" face="Consolas">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <font color="#ff0000">*System.UnauthorizedAccessException*</font><br /></font><font color="#ffffff" size="2" face="Consolas">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; [Excludes]<br /></font><font color="#ffffff" size="2" face="Consolas">Terminate monitor:&nbsp;&nbsp;&nbsp;&nbsp; Disabled<br /></font><font color="#ffffff" size="2" face="Consolas">Cloning type:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Disabled<br /></font><font color="#ffffff" size="2" face="Consolas">Concurrent limit:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; n/a<br /></font><font color="#ffffff" size="2" face="Consolas">Avoid outage:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; n/a<br /></font><font color="#ffffff" size="2" face="Consolas">Number of dumps:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1<br /></font><font color="#ffffff" size="2" face="Consolas">Dump folder:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; D:\home\Dumps\<br /></font><font color="#ffffff" size="2" face="Consolas">Dump filename/mask:&nbsp;&nbsp;&nbsp; PROCESSNAME_YYMMDD_HHMMSS<br /></font><font color="#ffffff" size="2" face="Consolas">Queue to WER:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Disabled<br /></font><font color="#ffffff" size="2" face="Consolas">Kill after dump:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Disabled<br /></font><font size="2"></font>
>       </p>
>       
>       <p>
>         <font color="#ffffff" size="2" face="Consolas">Press Ctrl-C to end monitoring without terminating the process.<br /></font><font color="#ffffff" size="2" face="Consolas">CLR Version: v4.0.30319<br /></font><font style="background-color: #ffff00" color="#c0504d"></font><font color="#ffc000" size="2" face="Consolas"><strong>[10:02:46] Exception: E0434F4D.System.Exception (&#8220;There was a problem processing this request&#8221;)<br /></strong></font><font color="#ffc000" size="2" face="Consolas"><strong>[10:02:47] Exception: E0434F4D.System.UnauthorizedAccessException (&#8220;Access is denied.&#8221;)<br /></strong></font><font color="#ffc000" size="2" face="Consolas"><strong>[10:02:47] Dump 1 initiated: D:\home\Dumps\w3wp.exe_170426_100247.dmp<br /></strong></font><font size="2"><strong><font face="Consolas"><font color="#ffc000">[10:02:52] Dump 1 writing: Estimated dump file size is 306 MB.</font><br /></font></strong></font><strong><font size="2"><font color="#ffc000" face="Consolas">[10:03:16] Dump 1 complete: 306 MB written in 29.8 seconds<br />[10:03:17] Dump count reached</font></font></strong><font style="background-color: #ffff00"><font color="#c0504d"><font size="2" face="Courier New"></font></font></font>
>       </p>
>     </td>
>   </tr>
> </table>

HTH!<img class="wlEmoticon wlEmoticon-smile" style="border-top-style: none;border-left-style: none;border-bottom-style: none;border-right-style: none" alt="Smile" src="https://msdnshared.blob.core.windows.net/media/2017/05/wlEmoticon-smile2.png" />