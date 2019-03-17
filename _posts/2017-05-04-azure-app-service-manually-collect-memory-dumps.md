---
id: 1555
title: 'Azure App Service: Manually collect memory dumps'
date: 2017-05-04T17:05:25+00:00
author: Kaushal Kumar Panday
layout: post
guid: https://blogs.msdn.microsoft.com/kaushal/?p=1555
permalink: /2017/05/04/azure-app-service-manually-collect-memory-dumps/
opengraph_tags:
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Azure App Service: Manually collect memory dumps" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2017/05/04/azure-app-service-manually-collect-memory-dumps/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="While troubleshooting web application performance issues we are sometimes required to gather memory dumps during the time of the issue. In Azure App Service, we do not have RDP access to the machines. However, this doesn’t restrict us from gathering logs &amp; data for troubleshooting. I am listing out few methods using which we can..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2017/01/image_thumb547.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Azure App Service: Manually collect memory dumps" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2017/05/04/azure-app-service-manually-collect-memory-dumps/" />
    <meta name="twitter:description" content="While troubleshooting web application performance issues we are sometimes required to gather memory dumps during the time of the issue. In Azure App Service, we do not have RDP access to the machines. However, this doesn’t restrict us from gathering logs &amp; data for troubleshooting. I am listing out few methods using which we can..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2017/01/image_thumb547.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Azure App Service: Manually collect memory dumps" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2017/05/04/azure-app-service-manually-collect-memory-dumps/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="While troubleshooting web application performance issues we are sometimes required to gather memory dumps during the time of the issue. In Azure App Service, we do not have RDP access to the machines. However, this doesn’t restrict us from gathering logs &amp; data for troubleshooting. I am listing out few methods using which we can..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2017/01/image_thumb547.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Azure App Service: Manually collect memory dumps" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2017/05/04/azure-app-service-manually-collect-memory-dumps/" />
    <meta name="twitter:description" content="While troubleshooting web application performance issues we are sometimes required to gather memory dumps during the time of the issue. In Azure App Service, we do not have RDP access to the machines. However, this doesn’t restrict us from gathering logs &amp; data for troubleshooting. I am listing out few methods using which we can..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2017/01/image_thumb547.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Azure App Service: Manually collect memory dumps" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2017/05/04/azure-app-service-manually-collect-memory-dumps/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="While troubleshooting web application performance issues we are sometimes required to gather memory dumps during the time of the issue. In Azure App Service, we do not have RDP access to the machines. However, this doesn’t restrict us from gathering logs &amp; data for troubleshooting. I am listing out few methods using which we can..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2017/01/image_thumb547.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Azure App Service: Manually collect memory dumps" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2017/05/04/azure-app-service-manually-collect-memory-dumps/" />
    <meta name="twitter:description" content="While troubleshooting web application performance issues we are sometimes required to gather memory dumps during the time of the issue. In Azure App Service, we do not have RDP access to the machines. However, this doesn’t restrict us from gathering logs &amp; data for troubleshooting. I am listing out few methods using which we can..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2017/01/image_thumb547.png" />
    
categories:
  - Azure
  - Azure App Service
  - Azure Web App
  - Azure Websites
  - dumps
  - hang
  - Kudu
  - memory
  - procdump
---
<u></u>

<font size="2">While troubleshooting web application performance issues we are sometimes required to gather memory dumps during the time of the issue.</font>

<font size="2">In <font face="Segoe UI Semibold">Azure App Service</font>, we do not have RDP access to the machines. However, this doesn’t restrict us from gathering logs & data for troubleshooting. I am listing out few methods using which we can generate memory dumps of the process during the time of the issue.</font>

# <u>Method 1: Using ProcDump.exe </u>

> ##### <font size="2"><u><font face="Segoe UI Semibold">Pre-Requisite</font>:</u> For this we need the sysinternals utility: </font><a href="https://live.sysinternals.com/procdump.exe" target="_blank" rel="noopener noreferrer"><font size="2">ProcDump.exe</font></a>

<font size="2">Azure App Service instances include the sysinternals suite in the default image. They can be located here via the KUDU console: <font style="background-color: #cccccc" face="Consolas">D:\devtools\sysinternals</font></font>

<font size="2">The users may also download ProcDump from </font><a href="https://live.sysinternals.com/procdump.exe" target="_blank" rel="noopener noreferrer"><font size="2">here</font></a> <font size="2">and upload it a specific location such as <font style="background-color: #cccccc" face="Consolas">D:\home\LogFiles\Dumps</font> and use it. </font>

  * <font size="2">Browse to the KUDU console </font> 
      * <font size="2">Click on <strong>Process Explorer</strong> menu. </font> 
          * <font size="2">There will be 2 w3wp.exe processes, one for <strong>SCM </strong>(KUDU) and another for the application. </font></ul> 
        > [<img title="image" style="border-top: 0px;border-right: 0px;border-bottom: 0px;padding-top: 0px;padding-left: 0px;border-left: 0px;padding-right: 0px" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/2017/05/image_thumb122.png" width="798" height="171" />](https://msdnshared.blob.core.windows.net/media/2017/05/image121.png)
        
          * <font size="2">Note the <strong>PID </strong>(Process ID) of the w3wp.exe corresponding to the application (see the image above) </font> 
              * <font size="2">Browse to <strong>Debug Console </strong>–> <strong>CMD</strong> </font> 
                  * <font size="2">In the command window, navigate to the <strong>dumps </strong>folder. </font> 
                      * <font size="2">Execute the following command to generate a full memory dump of the process</font></ul> 
                    > <table cellspacing="0" cellpadding="2" width="620" border="2">
                    >   <tr>
                    >     <td bgcolor="#e5f9ff" valign="top" width="616">
                    >       <font size="2" face="Courier New">procdump.exe -accepteula –ma <PID of the process></font>
                    >     </td>
                    >   </tr>
                    >   
                    >   <tr>
                    >     <td bgcolor="#e5f9ff" valign="top" width="616">
                    >       <font size="2">where, <br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; -ma&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Write a dump file with all process memory. The default dump format only includes <br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; thread and handle information<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; -accepteula&nbsp;&nbsp;&nbsp; Use this switch to automatically accept the Sysinternals license agreement.</font>
                    >     </td>
                    >   </tr>
                    > </table>
                    
                    > [<img title="image" style="border-left-width: 0px;border-right-width: 0px;border-bottom-width: 0px;padding-top: 0px;padding-left: 0px;padding-right: 0px;border-top-width: 0px" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/2017/01/image_thumb547.png" width="804" height="506" />](https://msdnshared.blob.core.windows.net/media/2017/01/image630.png)
                    
                    # <u>Method 2: Using Diagnostics as a Service (DaaS) </u>
                    
                    ## <font size="4"><font face="Segoe UI"><u>Via Portal:</u></font></font>
                    
                      * <font size="2">Login to Azure portal. (</font>[<font size="2">https://portal.azure.com</font>](https://portal.azure.com)<font size="2">) </font> 
                          * <font size="2">Select the Azure Web App that you intend to troubleshoot </font> 
                              * <font size="2">Click on <strong>Diagnose and solve problems</strong>.</font> </ul> 
                            > [<img title="image" style="border-left-width: 0px;border-right-width: 0px;border-bottom-width: 0px;padding-top: 0px;padding-left: 0px;margin: 0px;padding-right: 0px;border-top-width: 0px" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/2017/05/image_thumb62.png" width="232" height="272" />](https://msdnshared.blob.core.windows.net/media/2017/05/image59.png)
                            
                              * <font size="2">In the new blade click on <strong>Diagnostics as a Service</strong>. (<em>Bottom right side of the blade.</em>)</font>
                            
                            > [<img title="image" style="border-left-width: 0px;border-right-width: 0px;border-bottom-width: 0px;padding-top: 0px;padding-left: 0px;margin: 0px;padding-right: 0px;border-top-width: 0px" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/2017/05/image_thumb63.png" width="258" height="311" />](https://msdnshared.blob.core.windows.net/media/2017/05/image60.png)
                            
                              * In the new blade, set the following: 
                                  * **Application Type** – Depending on the type of application set the value to **ASP.NET** or **PHP** or **Node.js**. 
                                      * **Diagnosers** – Since this post is about collecting memory dumps, ensure that the check box against **Memory Dump** is selected. If you need **Event Viewer Logs** & **Http Logs** then you can enable them too. 
                                          * **Instances –** If the App Service Plan is configured to use more than one instance, then you can configure this to collect the logs on either multiple instance or specific instances.</ul> </ul> 
                                    > [<img title="image" style="border-left-width: 0px;border-right-width: 0px;border-bottom-width: 0px;padding-top: 0px;padding-left: 0px;margin: 0px;padding-right: 0px;border-top-width: 0px" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/2017/05/image_thumb64.png" width="561" height="310" />](https://msdnshared.blob.core.windows.net/media/2017/05/image61.png)
                                    
                                      * Click on Run to collect the logs. The blade will indicate the status of the operation and will also run analysis on the collected data. 
                                      * This puts the data under **<font style="background-color: #cccccc" size="2" face="Consolas">D:\home\data\DaaS\Logs<font style="background-color: #ffffff"> </font></font>**folder.<!--EndFragment-->
                                    
                                    <font size="4"><font face="Segoe UI"><u>Via KUDU:</u></font></font>
                                    
                                    <font size="2">In scenarios, where the user may not have access to the portal, they can use <strong>Kudu </strong>to access <strong>DaaS</strong>. The option to select instances is not available here as KUDU by default connects to a specific instance. You can refer my previous post on this: </font>[<font size="2">How to connect to the Kudu site of a specific instance</font>](https://blogs.msdn.microsoft.com/kaushal/2016/11/21/azure-app-service-how-to-connect-to-the-kudu-site-of-a-specific-instance/ "https://blogs.msdn.microsoft.com/kaushal/2016/11/21/azure-app-service-how-to-connect-to-the-kudu-site-of-a-specific-instance/")
                                    
                                      * <font size="2">Login to the <strong>KUDU</strong> console and append /<strong>daas</strong> to the path. (</font>[<font size="2">http://<yoursitename>.scm.azurewebsites.net/daas</font>](http://<yoursitename>.scm.azurewebsites.net/daas)<font size="2">) </font> 
                                          * <font size="2">This will launch the <strong>DaaS</strong> portal </font> 
                                              * <font size="2">Reproduce the issue </font> 
                                                  * <font size="2">Click on <strong>Diagnose Now </strong>button as shown below:</font></ul> 
                                                > [<img title="image" style="border-left-width: 0px;border-right-width: 0px;border-bottom-width: 0px;padding-top: 0px;padding-left: 0px;margin: 0px;padding-right: 0px;border-top-width: 0px" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/2017/05/image_thumb65.png" width="877" height="453" />](https://msdnshared.blob.core.windows.net/media/2017/05/image62.png)
                                                
                                                  * This will initiate logs collect. 
                                                      * You can click on Schedule Analysis to select the logs that will be collected and whether you want to run an analysis on that. </ul> 
                                                    > #### <font size="4"><u>More Information:</u></font>
                                                    > 
                                                    > [<font size="2">DaaS – Diagnostics as a Service for Azure Web Sites</font>](https://azure.microsoft.com/en-in/blog/daas/ "https://azure.microsoft.com/en-in/blog/daas/")
                                                    > 
                                                    > [<font size="2">New Updates to DaaS &#8211; Diagnostics as a Service for Azure Websites</font>](https://azure.microsoft.com/en-in/blog/new-updates-to-daas-diagnostics-as-a-service-for-azure-websites/ "https://azure.microsoft.com/en-in/blog/new-updates-to-daas-diagnostics-as-a-service-for-azure-websites/")<font size="2">&nbsp;</font>
                                                    > 
                                                    > [<font size="2">https://sunithamk.wordpress.com/2015/11/04/diagnose-and-mitigate-issues-with-azure-web-apps-support-portal/</font>](https://sunithamk.wordpress.com/2015/11/04/diagnose-and-mitigate-issues-with-azure-web-apps-support-portal/ "https://sunithamk.wordpress.com/2015/11/04/diagnose-and-mitigate-issues-with-azure-web-apps-support-portal/")&nbsp;
                                                    
                                                    # <u>Method 3: Using Process Explorer (KUDU) (<em>least favorable</em>)</u>
                                                    
                                                    <font face="Segoe UI Semibold"><font size="2"><font style="background-color: #ffff00" color="#c0504d">This method is the least favorable as it generates the memory dump and the prompts the user to download it. If the download is interrupted due to some reason then the data is lost.</font> </font></font>
                                                    
                                                      * Login to the KUDU console. ([http://<yoursitename>.scm.azurewebsites.net](http://%3cyoursitename%3e.scm.azurewebsites.net)) 
                                                          * Click on **Process Explorer** menu 
                                                              * There will be 2 w3wp.exe processes, one for **SCM** (KUDU) and another for the application. 
                                                                  * Reproduce the issue 
                                                                      * Right click the w3wp process (_without the **scm** tag_) and select **Download memory dump** –> **Full Dump** as shown below:</ul> 
                                                                    > [<img title="clip_image001" style="border-left-width: 0px;border-right-width: 0px;border-bottom-width: 0px;padding-top: 0px;padding-left: 0px;padding-right: 0px;border-top-width: 0px" border="0" alt="clip_image001" src="https://msdnshared.blob.core.windows.net/media/2017/05/clip_image001_thumb1.jpg" width="1028" height="221" />](https://msdnshared.blob.core.windows.net/media/2017/05/clip_image0012.jpg) 
                                                                    
                                                                      * <font size="2">Depending on the size of the process it will take couple of seconds or few minutes to generate the dump on the VM and prompt you to download the file</font>
                                                                    <h3 align="center">
                                                                      <u><font color="#ff0000" size="4" face="Segoe UI Semibold">****IMPORTANT****</font></u>
                                                                    </h3>
                                                                    
                                                                      * <div align="left">
                                                                          <font size="2">Using <strong>Daas </strong>via portal is the preferable method. When the web app is scaled out to run on more than one instance, then you can use DaaS to collect the memory dump from a specific instance. <strong>Method 2 & 3 </strong>will generate memory dump on a specific instance and is not fool proof as the issue may or may not be occurring on the connected instance. You can however connect to the KUDU of a specific instance using my previous post here: <a title="https://blogs.msdn.microsoft.com/kaushal/2016/11/21/azure-app-service-how-to-connect-to-the-kudu-site-of-a-specific-instance/" href="https://blogs.msdn.microsoft.com/kaushal/2016/11/21/azure-app-service-how-to-connect-to-the-kudu-site-of-a-specific-instance/">How to connect to the Kudu site of a specific instance</a></font>
                                                                        </div>
                                                                        
                                                                          * <div align="left">
                                                                              <font size="2">The downloading of the memory dump will contribute towards the outbound bandwidth of the App service plan. For more details refer: </font><a href="http://azure.microsoft.com/en-us/pricing/details/data-transfers/"><font size="2">http://azure.microsoft.com/en-us/pricing/details/data-transfers/</font></a>
                                                                            </div>
                                                                            
                                                                              * <div align="left">
                                                                                  <font size="2">When the memory dump is being written, the process remains in a frozen state for the entire duration of operation. So this impacts the application’s availability.</font>
                                                                                </div>
                                                                                
                                                                                  * <div align="left">
                                                                                      <font size="2">You can compress the memory dump via <strong>7zip</strong> which is availably by default on Azure App Service instances. You can run the following command:</font>
                                                                                    </div></ul> 
                                                                                
                                                                                > <p align="left">
                                                                                >   <font style="background-color: #cccccc" size="2" face="Consolas">D:\home\Logfiles\Dumps>D:\7zip\7za.exe a <strong>MemoryDumps</strong>.zip *.dmp</font>
                                                                                > </p>
                                                                                > 
                                                                                > <p align="left">
                                                                                >   <font style="background-color: #cccccc" size="2">NOTE: Compression consumes CPU cycles, so you may want to re-consider when running this on a <strong>Small </strong>sized instance</font>
                                                                                > </p>
                                                                                > 
                                                                                > <p align="left">
                                                                                >   <a href="https://msdnshared.blob.core.windows.net/media/2017/05/image63.png"><img title="image" style="border-left-width: 0px;border-right-width: 0px;border-bottom-width: 0px;padding-top: 0px;padding-left: 0px;padding-right: 0px;border-top-width: 0px" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/2017/05/image_thumb66.png" width="781" height="491" /></a>
                                                                                > </p>