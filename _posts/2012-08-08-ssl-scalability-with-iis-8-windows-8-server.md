---
id: 112
title: SSL Scalability with IIS 8 (Windows 8 Server)
date: 2012-08-08T01:34:40+00:00
author: kaushal
layout: post
guid: https://blogs.msdn.microsoft.com/kaushal/2012/08/08/ssl-scalability-with-iis-8-windows-8-server/
permalink: /2012/08/08/ssl-scalability-with-iis-8-windows-8-server/
orig_url:
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2012/08/08/ssl-scalability-with-iis-8-windows-8-server.aspx
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2012/08/08/ssl-scalability-with-iis-8-windows-8-server.aspx
  - http://blogs.msdn.microsoft.com/b/kaushal/archive/2012/08/08/ssl-scalability-with-iis-8-windows-8-server.aspx
orig_site_id:
  - "13803"
  - "13803"
  - "13803"
orig_post_id:
  - "10337778"
  - "10337778"
  - "10337778"
orig_parent_id:
  - "10337778"
  - "10337778"
  - "10337778"
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
  - http://blogs.msdn.com/b/kaushal/archive/2012/08/08/ssl-scalability-with-iis-8-windows-8-server.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2012/08/08/ssl-scalability-with-iis-8-windows-8-server.aspx
  - http://blogs.msdn.com/b/kaushal/archive/2012/08/08/ssl-scalability-with-iis-8-windows-8-server.aspx
orig_post_name:
  - ssl scalability with iis 8 windows 8 server
  - ssl scalability with iis 8 windows 8 server
  - ssl scalability with iis 8 windows 8 server
orig_thread_id:
  - "817057"
  - "817057"
  - "817057"
orig_post_author_email:
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
  - kaushalp@microsoft.com
orig_attachment_count:
  - "0"
  - "0"
  - "0"
total_views:
  - "8677"
  - "8677"
  - "8677"
opengraph_tags:
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="SSL Scalability with IIS 8 (Windows 8 Server)" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/08/08/ssl-scalability-with-iis-8-windows-8-server/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="One of the biggest problems with IIS on the previous versions of IIS was in regards to scalability. This restriction was at the OS level at the kernel mode. There is nothing much that we could do to address this in IIS. One cannot bind more than one Certificate to a combination of &lt;IP:Port&gt;. The..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6153.image_thumb_3C582A10.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="SSL Scalability with IIS 8 (Windows 8 Server)" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/08/08/ssl-scalability-with-iis-8-windows-8-server/" />
    <meta name="twitter:description" content="One of the biggest problems with IIS on the previous versions of IIS was in regards to scalability. This restriction was at the OS level at the kernel mode. There is nothing much that we could do to address this in IIS. One cannot bind more than one Certificate to a combination of &lt;IP:Port&gt;. The..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6153.image_thumb_3C582A10.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="SSL Scalability with IIS 8 (Windows 8 Server)" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/08/08/ssl-scalability-with-iis-8-windows-8-server/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="One of the biggest problems with IIS on the previous versions of IIS was in regards to scalability. This restriction was at the OS level at the kernel mode. There is nothing much that we could do to address this in IIS. One cannot bind more than one Certificate to a combination of &lt;IP:Port&gt;. The..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6153.image_thumb_3C582A10.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="SSL Scalability with IIS 8 (Windows 8 Server)" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/08/08/ssl-scalability-with-iis-8-windows-8-server/" />
    <meta name="twitter:description" content="One of the biggest problems with IIS on the previous versions of IIS was in regards to scalability. This restriction was at the OS level at the kernel mode. There is nothing much that we could do to address this in IIS. One cannot bind more than one Certificate to a combination of &lt;IP:Port&gt;. The..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6153.image_thumb_3C582A10.png" />
    
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="SSL Scalability with IIS 8 (Windows 8 Server)" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/08/08/ssl-scalability-with-iis-8-windows-8-server/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="One of the biggest problems with IIS on the previous versions of IIS was in regards to scalability. This restriction was at the OS level at the kernel mode. There is nothing much that we could do to address this in IIS. One cannot bind more than one Certificate to a combination of &lt;IP:Port&gt;. The..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6153.image_thumb_3C582A10.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="SSL Scalability with IIS 8 (Windows 8 Server)" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2012/08/08/ssl-scalability-with-iis-8-windows-8-server/" />
    <meta name="twitter:description" content="One of the biggest problems with IIS on the previous versions of IIS was in regards to scalability. This restriction was at the OS level at the kernel mode. There is nothing much that we could do to address this in IIS. One cannot bind more than one Certificate to a combination of &lt;IP:Port&gt;. The..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6153.image_thumb_3C582A10.png" />
    
categories:
  - Uncategorized
tags:
  - CCS
  - Central Certificate Store
  - IIS 8
  - Scalability
  - Server Name Indication
  - SNI
  - SSL
  - TLS
---
<meta name="ProgId" content="Word.Document" />

<meta name="Generator" content="Microsoft Word 15" />

<meta name="Originator" content="Microsoft Word 15" />

<link rel="File-List" href="One%20of%20the%20biggest%20problems%20with%20IIS%20on%20the%20previous%20versions%20of%20IIS%20was%20in%20regards%20to%20scalability_files/filelist.xml" />

<link rel="Edit-Time-Data" href="One%20of%20the%20biggest%20problems%20with%20IIS%20on%20the%20previous%20versions%20of%20IIS%20was%20in%20regards%20to%20scalability_files/editdata.mso" />

<!--[if !mso]>

<![endif]-->

<!--[if gte mso 9]><xml>
 <o:DocumentProperties>
  <o:Author>Kaushal Kumar Panday</o:Author>
  <o:LastAuthor>Kaushal Kumar Panday</o:LastAuthor>
  <o:Revision>4</o:Revision>
  <o:TotalTime>49</o:TotalTime>
  <o:Created>2012-08-08T07:40:00Z</o:Created>
  <o:LastSaved>2012-08-08T08:29:00Z</o:LastSaved>
  <o:Pages>1</o:Pages>
  <o:Words>722</o:Words>
  <o:Characters>4119</o:Characters>
  <o:Lines>34</o:Lines>
  <o:Paragraphs>9</o:Paragraphs>
  <o:CharactersWithSpaces>4832</o:CharactersWithSpaces>
  <o:Version>15.00</o:Version>
 </o:DocumentProperties>
 <o:OfficeDocumentSettings>
  <o:AllowPNG/>
 </o:OfficeDocumentSettings>
</xml><![endif]-->

<link rel="themeData" href="One%20of%20the%20biggest%20problems%20with%20IIS%20on%20the%20previous%20versions%20of%20IIS%20was%20in%20regards%20to%20scalability_files/themedata.thmx" />

<link rel="colorSchemeMapping" href="One%20of%20the%20biggest%20problems%20with%20IIS%20on%20the%20previous%20versions%20of%20IIS%20was%20in%20regards%20to%20scalability_files/colorschememapping.xml" />

<!--[if gte mso 9]><xml>
 <w:WordDocument>
  <w:SpellingState>Clean</w:SpellingState>
  <w:GrammarState>Clean</w:GrammarState>
  <w:TrackMoves>false</w:TrackMoves>
  <w:TrackFormatting/>
  <w:PunctuationKerning/>
  <w:ValidateAgainstSchemas/>
  <w:SaveIfXMLInvalid>false</w:SaveIfXMLInvalid>
  <w:IgnoreMixedContent>false</w:IgnoreMixedContent>
  <w:AlwaysShowPlaceholderText>false</w:AlwaysShowPlaceholderText>
  <w:DoNotPromoteQF/>
  <w:LidThemeOther>EN-IN</w:LidThemeOther>
  <w:LidThemeAsian>X-NONE</w:LidThemeAsian>
  <w:LidThemeComplexScript>X-NONE</w:LidThemeComplexScript>
  <w:Compatibility>
   <w:BreakWrappedTables/>
   <w:SnapToGridInCell/>
   <w:WrapTextWithPunct/>
   <w:UseAsianBreakRules/>
   <w:DontGrowAutofit/>
   <w:SplitPgBreakAndParaMark/>
   <w:EnableOpenTypeKerning/>
   <w:DontFlipMirrorIndents/>
   <w:OverrideTableStyleHps/>
  </w:Compatibility>
  <m:mathPr>
   <m:mathFont m:val="Cambria Math"/>
   <m:brkBin m:val="before"/>
   <m:brkBinSub m:val="&#45;-"/>
   <m:smallFrac m:val="off"/>
   <m:dispDef/>
   <m:lMargin m:val="0"/>
   <m:rMargin m:val="0"/>
   <m:defJc m:val="centerGroup"/>
   <m:wrapIndent m:val="1440"/>
   <m:intLim m:val="subSup"/>
   <m:naryLim m:val="undOvr"/>
  </m:mathPr></w:WordDocument>
</xml><![endif]-->

<!--[if gte mso 9]><xml>
 <w:LatentStyles DefLockedState="false" DefUnhideWhenUsed="false"
  DefSemiHidden="false" DefQFormat="false" DefPriority="99"
  LatentStyleCount="371">
  <w:LsdException Locked="false" Priority="0" QFormat="true" Name="Normal"/>
  <w:LsdException Locked="false" Priority="9" QFormat="true" Name="heading 1"/>
  <w:LsdException Locked="false" Priority="9" SemiHidden="true"
   UnhideWhenUsed="true" QFormat="true" Name="heading 2"/>
  <w:LsdException Locked="false" Priority="9" SemiHidden="true"
   UnhideWhenUsed="true" QFormat="true" Name="heading 3"/>
  <w:LsdException Locked="false" Priority="9" SemiHidden="true"
   UnhideWhenUsed="true" QFormat="true" Name="heading 4"/>
  <w:LsdException Locked="false" Priority="9" SemiHidden="true"
   UnhideWhenUsed="true" QFormat="true" Name="heading 5"/>
  <w:LsdException Locked="false" Priority="9" SemiHidden="true"
   UnhideWhenUsed="true" QFormat="true" Name="heading 6"/>
  <w:LsdException Locked="false" Priority="9" SemiHidden="true"
   UnhideWhenUsed="true" QFormat="true" Name="heading 7"/>
  <w:LsdException Locked="false" Priority="9" SemiHidden="true"
   UnhideWhenUsed="true" QFormat="true" Name="heading 8"/>
  <w:LsdException Locked="false" Priority="9" SemiHidden="true"
   UnhideWhenUsed="true" QFormat="true" Name="heading 9"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="index 1"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="index 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="index 3"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="index 4"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="index 5"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="index 6"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="index 7"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="index 8"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="index 9"/>
  <w:LsdException Locked="false" Priority="39" SemiHidden="true"
   UnhideWhenUsed="true" Name="toc 1"/>
  <w:LsdException Locked="false" Priority="39" SemiHidden="true"
   UnhideWhenUsed="true" Name="toc 2"/>
  <w:LsdException Locked="false" Priority="39" SemiHidden="true"
   UnhideWhenUsed="true" Name="toc 3"/>
  <w:LsdException Locked="false" Priority="39" SemiHidden="true"
   UnhideWhenUsed="true" Name="toc 4"/>
  <w:LsdException Locked="false" Priority="39" SemiHidden="true"
   UnhideWhenUsed="true" Name="toc 5"/>
  <w:LsdException Locked="false" Priority="39" SemiHidden="true"
   UnhideWhenUsed="true" Name="toc 6"/>
  <w:LsdException Locked="false" Priority="39" SemiHidden="true"
   UnhideWhenUsed="true" Name="toc 7"/>
  <w:LsdException Locked="false" Priority="39" SemiHidden="true"
   UnhideWhenUsed="true" Name="toc 8"/>
  <w:LsdException Locked="false" Priority="39" SemiHidden="true"
   UnhideWhenUsed="true" Name="toc 9"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Normal Indent"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="footnote text"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="annotation text"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="header"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="footer"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="index heading"/>
  <w:LsdException Locked="false" Priority="35" SemiHidden="true"
   UnhideWhenUsed="true" QFormat="true" Name="caption"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="table of figures"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="envelope address"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="envelope return"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="footnote reference"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="annotation reference"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="line number"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="page number"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="endnote reference"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="endnote text"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="table of authorities"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="macro"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="toa heading"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List Bullet"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List Number"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List 3"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List 4"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List 5"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List Bullet 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List Bullet 3"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List Bullet 4"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List Bullet 5"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List Number 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List Number 3"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List Number 4"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List Number 5"/>
  <w:LsdException Locked="false" Priority="10" QFormat="true" Name="Title"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Closing"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Signature"/>
  <w:LsdException Locked="false" Priority="1" SemiHidden="true"
   UnhideWhenUsed="true" Name="Default Paragraph Font"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Body Text"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Body Text Indent"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List Continue"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List Continue 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List Continue 3"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List Continue 4"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="List Continue 5"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Message Header"/>
  <w:LsdException Locked="false" Priority="11" QFormat="true" Name="Subtitle"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Salutation"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Date"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Body Text First Indent"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Body Text First Indent 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Note Heading"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Body Text 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Body Text 3"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Body Text Indent 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Body Text Indent 3"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Block Text"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Hyperlink"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="FollowedHyperlink"/>
  <w:LsdException Locked="false" Priority="22" QFormat="true" Name="Strong"/>
  <w:LsdException Locked="false" Priority="20" QFormat="true" Name="Emphasis"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Document Map"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Plain Text"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="E-mail Signature"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="HTML Top of Form"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="HTML Bottom of Form"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Normal (Web)"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="HTML Acronym"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="HTML Address"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="HTML Cite"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="HTML Code"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="HTML Definition"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="HTML Keyboard"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="HTML Preformatted"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="HTML Sample"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="HTML Typewriter"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="HTML Variable"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Normal Table"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="annotation subject"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="No List"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Outline List 1"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Outline List 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Outline List 3"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Simple 1"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Simple 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Simple 3"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Classic 1"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Classic 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Classic 3"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Classic 4"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Colorful 1"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Colorful 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Colorful 3"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Columns 1"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Columns 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Columns 3"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Columns 4"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Columns 5"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Grid 1"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Grid 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Grid 3"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Grid 4"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Grid 5"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Grid 6"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Grid 7"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Grid 8"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table List 1"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table List 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table List 3"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table List 4"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table List 5"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table List 6"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table List 7"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table List 8"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table 3D effects 1"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table 3D effects 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table 3D effects 3"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Contemporary"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Elegant"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Professional"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Subtle 1"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Subtle 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Web 1"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Web 2"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Web 3"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Balloon Text"/>
  <w:LsdException Locked="false" Priority="39" Name="Table Grid"/>
  <w:LsdException Locked="false" SemiHidden="true" UnhideWhenUsed="true"
   Name="Table Theme"/>
  <w:LsdException Locked="false" SemiHidden="true" Name="Placeholder Text"/>
  <w:LsdException Locked="false" Priority="1" QFormat="true" Name="No Spacing"/>
  <w:LsdException Locked="false" Priority="60" Name="Light Shading"/>
  <w:LsdException Locked="false" Priority="61" Name="Light List"/>
  <w:LsdException Locked="false" Priority="62" Name="Light Grid"/>
  <w:LsdException Locked="false" Priority="63" Name="Medium Shading 1"/>
  <w:LsdException Locked="false" Priority="64" Name="Medium Shading 2"/>
  <w:LsdException Locked="false" Priority="65" Name="Medium List 1"/>
  <w:LsdException Locked="false" Priority="66" Name="Medium List 2"/>
  <w:LsdException Locked="false" Priority="67" Name="Medium Grid 1"/>
  <w:LsdException Locked="false" Priority="68" Name="Medium Grid 2"/>
  <w:LsdException Locked="false" Priority="69" Name="Medium Grid 3"/>
  <w:LsdException Locked="false" Priority="70" Name="Dark List"/>
  <w:LsdException Locked="false" Priority="71" Name="Colorful Shading"/>
  <w:LsdException Locked="false" Priority="72" Name="Colorful List"/>
  <w:LsdException Locked="false" Priority="73" Name="Colorful Grid"/>
  <w:LsdException Locked="false" Priority="60" Name="Light Shading Accent 1"/>
  <w:LsdException Locked="false" Priority="61" Name="Light List Accent 1"/>
  <w:LsdException Locked="false" Priority="62" Name="Light Grid Accent 1"/>
  <w:LsdException Locked="false" Priority="63" Name="Medium Shading 1 Accent 1"/>
  <w:LsdException Locked="false" Priority="64" Name="Medium Shading 2 Accent 1"/>
  <w:LsdException Locked="false" Priority="65" Name="Medium List 1 Accent 1"/>
  <w:LsdException Locked="false" SemiHidden="true" Name="Revision"/>
  <w:LsdException Locked="false" Priority="34" QFormat="true"
   Name="List Paragraph"/>
  <w:LsdException Locked="false" Priority="29" QFormat="true" Name="Quote"/>
  <w:LsdException Locked="false" Priority="30" QFormat="true"
   Name="Intense Quote"/>
  <w:LsdException Locked="false" Priority="66" Name="Medium List 2 Accent 1"/>
  <w:LsdException Locked="false" Priority="67" Name="Medium Grid 1 Accent 1"/>
  <w:LsdException Locked="false" Priority="68" Name="Medium Grid 2 Accent 1"/>
  <w:LsdException Locked="false" Priority="69" Name="Medium Grid 3 Accent 1"/>
  <w:LsdException Locked="false" Priority="70" Name="Dark List Accent 1"/>
  <w:LsdException Locked="false" Priority="71" Name="Colorful Shading Accent 1"/>
  <w:LsdException Locked="false" Priority="72" Name="Colorful List Accent 1"/>
  <w:LsdException Locked="false" Priority="73" Name="Colorful Grid Accent 1"/>
  <w:LsdException Locked="false" Priority="60" Name="Light Shading Accent 2"/>
  <w:LsdException Locked="false" Priority="61" Name="Light List Accent 2"/>
  <w:LsdException Locked="false" Priority="62" Name="Light Grid Accent 2"/>
  <w:LsdException Locked="false" Priority="63" Name="Medium Shading 1 Accent 2"/>
  <w:LsdException Locked="false" Priority="64" Name="Medium Shading 2 Accent 2"/>
  <w:LsdException Locked="false" Priority="65" Name="Medium List 1 Accent 2"/>
  <w:LsdException Locked="false" Priority="66" Name="Medium List 2 Accent 2"/>
  <w:LsdException Locked="false" Priority="67" Name="Medium Grid 1 Accent 2"/>
  <w:LsdException Locked="false" Priority="68" Name="Medium Grid 2 Accent 2"/>
  <w:LsdException Locked="false" Priority="69" Name="Medium Grid 3 Accent 2"/>
  <w:LsdException Locked="false" Priority="70" Name="Dark List Accent 2"/>
  <w:LsdException Locked="false" Priority="71" Name="Colorful Shading Accent 2"/>
  <w:LsdException Locked="false" Priority="72" Name="Colorful List Accent 2"/>
  <w:LsdException Locked="false" Priority="73" Name="Colorful Grid Accent 2"/>
  <w:LsdException Locked="false" Priority="60" Name="Light Shading Accent 3"/>
  <w:LsdException Locked="false" Priority="61" Name="Light List Accent 3"/>
  <w:LsdException Locked="false" Priority="62" Name="Light Grid Accent 3"/>
  <w:LsdException Locked="false" Priority="63" Name="Medium Shading 1 Accent 3"/>
  <w:LsdException Locked="false" Priority="64" Name="Medium Shading 2 Accent 3"/>
  <w:LsdException Locked="false" Priority="65" Name="Medium List 1 Accent 3"/>
  <w:LsdException Locked="false" Priority="66" Name="Medium List 2 Accent 3"/>
  <w:LsdException Locked="false" Priority="67" Name="Medium Grid 1 Accent 3"/>
  <w:LsdException Locked="false" Priority="68" Name="Medium Grid 2 Accent 3"/>
  <w:LsdException Locked="false" Priority="69" Name="Medium Grid 3 Accent 3"/>
  <w:LsdException Locked="false" Priority="70" Name="Dark List Accent 3"/>
  <w:LsdException Locked="false" Priority="71" Name="Colorful Shading Accent 3"/>
  <w:LsdException Locked="false" Priority="72" Name="Colorful List Accent 3"/>
  <w:LsdException Locked="false" Priority="73" Name="Colorful Grid Accent 3"/>
  <w:LsdException Locked="false" Priority="60" Name="Light Shading Accent 4"/>
  <w:LsdException Locked="false" Priority="61" Name="Light List Accent 4"/>
  <w:LsdException Locked="false" Priority="62" Name="Light Grid Accent 4"/>
  <w:LsdException Locked="false" Priority="63" Name="Medium Shading 1 Accent 4"/>
  <w:LsdException Locked="false" Priority="64" Name="Medium Shading 2 Accent 4"/>
  <w:LsdException Locked="false" Priority="65" Name="Medium List 1 Accent 4"/>
  <w:LsdException Locked="false" Priority="66" Name="Medium List 2 Accent 4"/>
  <w:LsdException Locked="false" Priority="67" Name="Medium Grid 1 Accent 4"/>
  <w:LsdException Locked="false" Priority="68" Name="Medium Grid 2 Accent 4"/>
  <w:LsdException Locked="false" Priority="69" Name="Medium Grid 3 Accent 4"/>
  <w:LsdException Locked="false" Priority="70" Name="Dark List Accent 4"/>
  <w:LsdException Locked="false" Priority="71" Name="Colorful Shading Accent 4"/>
  <w:LsdException Locked="false" Priority="72" Name="Colorful List Accent 4"/>
  <w:LsdException Locked="false" Priority="73" Name="Colorful Grid Accent 4"/>
  <w:LsdException Locked="false" Priority="60" Name="Light Shading Accent 5"/>
  <w:LsdException Locked="false" Priority="61" Name="Light List Accent 5"/>
  <w:LsdException Locked="false" Priority="62" Name="Light Grid Accent 5"/>
  <w:LsdException Locked="false" Priority="63" Name="Medium Shading 1 Accent 5"/>
  <w:LsdException Locked="false" Priority="64" Name="Medium Shading 2 Accent 5"/>
  <w:LsdException Locked="false" Priority="65" Name="Medium List 1 Accent 5"/>
  <w:LsdException Locked="false" Priority="66" Name="Medium List 2 Accent 5"/>
  <w:LsdException Locked="false" Priority="67" Name="Medium Grid 1 Accent 5"/>
  <w:LsdException Locked="false" Priority="68" Name="Medium Grid 2 Accent 5"/>
  <w:LsdException Locked="false" Priority="69" Name="Medium Grid 3 Accent 5"/>
  <w:LsdException Locked="false" Priority="70" Name="Dark List Accent 5"/>
  <w:LsdException Locked="false" Priority="71" Name="Colorful Shading Accent 5"/>
  <w:LsdException Locked="false" Priority="72" Name="Colorful List Accent 5"/>
  <w:LsdException Locked="false" Priority="73" Name="Colorful Grid Accent 5"/>
  <w:LsdException Locked="false" Priority="60" Name="Light Shading Accent 6"/>
  <w:LsdException Locked="false" Priority="61" Name="Light List Accent 6"/>
  <w:LsdException Locked="false" Priority="62" Name="Light Grid Accent 6"/>
  <w:LsdException Locked="false" Priority="63" Name="Medium Shading 1 Accent 6"/>
  <w:LsdException Locked="false" Priority="64" Name="Medium Shading 2 Accent 6"/>
  <w:LsdException Locked="false" Priority="65" Name="Medium List 1 Accent 6"/>
  <w:LsdException Locked="false" Priority="66" Name="Medium List 2 Accent 6"/>
  <w:LsdException Locked="false" Priority="67" Name="Medium Grid 1 Accent 6"/>
  <w:LsdException Locked="false" Priority="68" Name="Medium Grid 2 Accent 6"/>
  <w:LsdException Locked="false" Priority="69" Name="Medium Grid 3 Accent 6"/>
  <w:LsdException Locked="false" Priority="70" Name="Dark List Accent 6"/>
  <w:LsdException Locked="false" Priority="71" Name="Colorful Shading Accent 6"/>
  <w:LsdException Locked="false" Priority="72" Name="Colorful List Accent 6"/>
  <w:LsdException Locked="false" Priority="73" Name="Colorful Grid Accent 6"/>
  <w:LsdException Locked="false" Priority="19" QFormat="true"
   Name="Subtle Emphasis"/>
  <w:LsdException Locked="false" Priority="21" QFormat="true"
   Name="Intense Emphasis"/>
  <w:LsdException Locked="false" Priority="31" QFormat="true"
   Name="Subtle Reference"/>
  <w:LsdException Locked="false" Priority="32" QFormat="true"
   Name="Intense Reference"/>
  <w:LsdException Locked="false" Priority="33" QFormat="true" Name="Book Title"/>
  <w:LsdException Locked="false" Priority="37" SemiHidden="true"
   UnhideWhenUsed="true" Name="Bibliography"/>
  <w:LsdException Locked="false" Priority="39" SemiHidden="true"
   UnhideWhenUsed="true" QFormat="true" Name="TOC Heading"/>
  <w:LsdException Locked="false" Priority="41" Name="Plain Table 1"/>
  <w:LsdException Locked="false" Priority="42" Name="Plain Table 2"/>
  <w:LsdException Locked="false" Priority="43" Name="Plain Table 3"/>
  <w:LsdException Locked="false" Priority="44" Name="Plain Table 4"/>
  <w:LsdException Locked="false" Priority="45" Name="Plain Table 5"/>
  <w:LsdException Locked="false" Priority="40" Name="Grid Table Light"/>
  <w:LsdException Locked="false" Priority="46" Name="Grid Table 1 Light"/>
  <w:LsdException Locked="false" Priority="47" Name="Grid Table 2"/>
  <w:LsdException Locked="false" Priority="48" Name="Grid Table 3"/>
  <w:LsdException Locked="false" Priority="49" Name="Grid Table 4"/>
  <w:LsdException Locked="false" Priority="50" Name="Grid Table 5 Dark"/>
  <w:LsdException Locked="false" Priority="51" Name="Grid Table 6 Colorful"/>
  <w:LsdException Locked="false" Priority="52" Name="Grid Table 7 Colorful"/>
  <w:LsdException Locked="false" Priority="46"
   Name="Grid Table 1 Light Accent 1"/>
  <w:LsdException Locked="false" Priority="47" Name="Grid Table 2 Accent 1"/>
  <w:LsdException Locked="false" Priority="48" Name="Grid Table 3 Accent 1"/>
  <w:LsdException Locked="false" Priority="49" Name="Grid Table 4 Accent 1"/>
  <w:LsdException Locked="false" Priority="50" Name="Grid Table 5 Dark Accent 1"/>
  <w:LsdException Locked="false" Priority="51"
   Name="Grid Table 6 Colorful Accent 1"/>
  <w:LsdException Locked="false" Priority="52"
   Name="Grid Table 7 Colorful Accent 1"/>
  <w:LsdException Locked="false" Priority="46"
   Name="Grid Table 1 Light Accent 2"/>
  <w:LsdException Locked="false" Priority="47" Name="Grid Table 2 Accent 2"/>
  <w:LsdException Locked="false" Priority="48" Name="Grid Table 3 Accent 2"/>
  <w:LsdException Locked="false" Priority="49" Name="Grid Table 4 Accent 2"/>
  <w:LsdException Locked="false" Priority="50" Name="Grid Table 5 Dark Accent 2"/>
  <w:LsdException Locked="false" Priority="51"
   Name="Grid Table 6 Colorful Accent 2"/>
  <w:LsdException Locked="false" Priority="52"
   Name="Grid Table 7 Colorful Accent 2"/>
  <w:LsdException Locked="false" Priority="46"
   Name="Grid Table 1 Light Accent 3"/>
  <w:LsdException Locked="false" Priority="47" Name="Grid Table 2 Accent 3"/>
  <w:LsdException Locked="false" Priority="48" Name="Grid Table 3 Accent 3"/>
  <w:LsdException Locked="false" Priority="49" Name="Grid Table 4 Accent 3"/>
  <w:LsdException Locked="false" Priority="50" Name="Grid Table 5 Dark Accent 3"/>
  <w:LsdException Locked="false" Priority="51"
   Name="Grid Table 6 Colorful Accent 3"/>
  <w:LsdException Locked="false" Priority="52"
   Name="Grid Table 7 Colorful Accent 3"/>
  <w:LsdException Locked="false" Priority="46"
   Name="Grid Table 1 Light Accent 4"/>
  <w:LsdException Locked="false" Priority="47" Name="Grid Table 2 Accent 4"/>
  <w:LsdException Locked="false" Priority="48" Name="Grid Table 3 Accent 4"/>
  <w:LsdException Locked="false" Priority="49" Name="Grid Table 4 Accent 4"/>
  <w:LsdException Locked="false" Priority="50" Name="Grid Table 5 Dark Accent 4"/>
  <w:LsdException Locked="false" Priority="51"
   Name="Grid Table 6 Colorful Accent 4"/>
  <w:LsdException Locked="false" Priority="52"
   Name="Grid Table 7 Colorful Accent 4"/>
  <w:LsdException Locked="false" Priority="46"
   Name="Grid Table 1 Light Accent 5"/>
  <w:LsdException Locked="false" Priority="47" Name="Grid Table 2 Accent 5"/>
  <w:LsdException Locked="false" Priority="48" Name="Grid Table 3 Accent 5"/>
  <w:LsdException Locked="false" Priority="49" Name="Grid Table 4 Accent 5"/>
  <w:LsdException Locked="false" Priority="50" Name="Grid Table 5 Dark Accent 5"/>
  <w:LsdException Locked="false" Priority="51"
   Name="Grid Table 6 Colorful Accent 5"/>
  <w:LsdException Locked="false" Priority="52"
   Name="Grid Table 7 Colorful Accent 5"/>
  <w:LsdException Locked="false" Priority="46"
   Name="Grid Table 1 Light Accent 6"/>
  <w:LsdException Locked="false" Priority="47" Name="Grid Table 2 Accent 6"/>
  <w:LsdException Locked="false" Priority="48" Name="Grid Table 3 Accent 6"/>
  <w:LsdException Locked="false" Priority="49" Name="Grid Table 4 Accent 6"/>
  <w:LsdException Locked="false" Priority="50" Name="Grid Table 5 Dark Accent 6"/>
  <w:LsdException Locked="false" Priority="51"
   Name="Grid Table 6 Colorful Accent 6"/>
  <w:LsdException Locked="false" Priority="52"
   Name="Grid Table 7 Colorful Accent 6"/>
  <w:LsdException Locked="false" Priority="46" Name="List Table 1 Light"/>
  <w:LsdException Locked="false" Priority="47" Name="List Table 2"/>
  <w:LsdException Locked="false" Priority="48" Name="List Table 3"/>
  <w:LsdException Locked="false" Priority="49" Name="List Table 4"/>
  <w:LsdException Locked="false" Priority="50" Name="List Table 5 Dark"/>
  <w:LsdException Locked="false" Priority="51" Name="List Table 6 Colorful"/>
  <w:LsdException Locked="false" Priority="52" Name="List Table 7 Colorful"/>
  <w:LsdException Locked="false" Priority="46"
   Name="List Table 1 Light Accent 1"/>
  <w:LsdException Locked="false" Priority="47" Name="List Table 2 Accent 1"/>
  <w:LsdException Locked="false" Priority="48" Name="List Table 3 Accent 1"/>
  <w:LsdException Locked="false" Priority="49" Name="List Table 4 Accent 1"/>
  <w:LsdException Locked="false" Priority="50" Name="List Table 5 Dark Accent 1"/>
  <w:LsdException Locked="false" Priority="51"
   Name="List Table 6 Colorful Accent 1"/>
  <w:LsdException Locked="false" Priority="52"
   Name="List Table 7 Colorful Accent 1"/>
  <w:LsdException Locked="false" Priority="46"
   Name="List Table 1 Light Accent 2"/>
  <w:LsdException Locked="false" Priority="47" Name="List Table 2 Accent 2"/>
  <w:LsdException Locked="false" Priority="48" Name="List Table 3 Accent 2"/>
  <w:LsdException Locked="false" Priority="49" Name="List Table 4 Accent 2"/>
  <w:LsdException Locked="false" Priority="50" Name="List Table 5 Dark Accent 2"/>
  <w:LsdException Locked="false" Priority="51"
   Name="List Table 6 Colorful Accent 2"/>
  <w:LsdException Locked="false" Priority="52"
   Name="List Table 7 Colorful Accent 2"/>
  <w:LsdException Locked="false" Priority="46"
   Name="List Table 1 Light Accent 3"/>
  <w:LsdException Locked="false" Priority="47" Name="List Table 2 Accent 3"/>
  <w:LsdException Locked="false" Priority="48" Name="List Table 3 Accent 3"/>
  <w:LsdException Locked="false" Priority="49" Name="List Table 4 Accent 3"/>
  <w:LsdException Locked="false" Priority="50" Name="List Table 5 Dark Accent 3"/>
  <w:LsdException Locked="false" Priority="51"
   Name="List Table 6 Colorful Accent 3"/>
  <w:LsdException Locked="false" Priority="52"
   Name="List Table 7 Colorful Accent 3"/>
  <w:LsdException Locked="false" Priority="46"
   Name="List Table 1 Light Accent 4"/>
  <w:LsdException Locked="false" Priority="47" Name="List Table 2 Accent 4"/>
  <w:LsdException Locked="false" Priority="48" Name="List Table 3 Accent 4"/>
  <w:LsdException Locked="false" Priority="49" Name="List Table 4 Accent 4"/>
  <w:LsdException Locked="false" Priority="50" Name="List Table 5 Dark Accent 4"/>
  <w:LsdException Locked="false" Priority="51"
   Name="List Table 6 Colorful Accent 4"/>
  <w:LsdException Locked="false" Priority="52"
   Name="List Table 7 Colorful Accent 4"/>
  <w:LsdException Locked="false" Priority="46"
   Name="List Table 1 Light Accent 5"/>
  <w:LsdException Locked="false" Priority="47" Name="List Table 2 Accent 5"/>
  <w:LsdException Locked="false" Priority="48" Name="List Table 3 Accent 5"/>
  <w:LsdException Locked="false" Priority="49" Name="List Table 4 Accent 5"/>
  <w:LsdException Locked="false" Priority="50" Name="List Table 5 Dark Accent 5"/>
  <w:LsdException Locked="false" Priority="51"
   Name="List Table 6 Colorful Accent 5"/>
  <w:LsdException Locked="false" Priority="52"
   Name="List Table 7 Colorful Accent 5"/>
  <w:LsdException Locked="false" Priority="46"
   Name="List Table 1 Light Accent 6"/>
  <w:LsdException Locked="false" Priority="47" Name="List Table 2 Accent 6"/>
  <w:LsdException Locked="false" Priority="48" Name="List Table 3 Accent 6"/>
  <w:LsdException Locked="false" Priority="49" Name="List Table 4 Accent 6"/>
  <w:LsdException Locked="false" Priority="50" Name="List Table 5 Dark Accent 6"/>
  <w:LsdException Locked="false" Priority="51"
   Name="List Table 6 Colorful Accent 6"/>
  <w:LsdException Locked="false" Priority="52"
   Name="List Table 7 Colorful Accent 6"/>
 </w:LatentStyles>
</xml><![endif]-->

<p align="justify">
  <!--[if gte mso 10]>

<![endif]-->
  
  <!--[if gte mso 9]><xml>
 <o:shapedefaults v:ext="edit" spidmax="1026"/>
</xml><![endif]-->
  
  <!--[if gte mso 9]><xml>
 <o:shapelayout v:ext="edit">
  <o:idmap v:ext="edit" data="1"/>
 </o:shapelayout></xml><![endif]-->
</p>

<div class="WordSection1" align="justify">
</div>

<p class="MsoNormal" style="line-height: normal; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto;" align="justify">
  <span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"><font size="2">One of the biggest problems with IIS on the previous versions of IIS was in regards to scalability. This restriction was at the OS level at the kernel mode. There is nothing much that we could do to address this in IIS. One cannot bind more than one Certificate to a combination of <b><<span class="SpellE">IP<span class="GramE">:Port</span></span>></b>. The workarounds were:</font></span>
</p>

<div class="WordSection1" align="justify">
</div>

<div class="WordSection1" align="justify">
  <ul>
    <li>
      <div class="MsoNormal" style="line-height: normal; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto;">
        <span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"><font size="2">Use a Wild Card Certificate</font></span>
      </div>
    </li>
    
    <li>
      <div class="MsoNormal" style="line-height: normal; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto;">
        <span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"><font size="2">Use a SAN Certificate</font></span>
      </div>
    </li>
    
    <li>
      <div class="MsoNormal" style="line-height: normal; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto;">
        <span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"><font size="2">Use a different combination of <strong>IP:Port</strong></font></span>
      </div>
    </li>
  </ul>
</div>

<p align="justify">
  <p class="MsoNormal" style="line-height: normal; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto;" align="justify">
    <span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"></span><font size="2"><!--[endif]--></font>
    
    <span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"><font size="2">None of this was an ideal workaround. You could read more about this restriction here: <br /></font><a title="http://blogs.msdn.com/b/anilpras/archive/2012/05/23/server-certificate-bindings-and-its-restrictions-in-iis-6-0-amp-iis-7-x.aspx" href="http://blogs.msdn.com/b/anilpras/archive/2012/05/23/server-certificate-bindings-and-its-restrictions-in-iis-6-0-amp-iis-7-x.aspx"><font color="#0000ff" size="2"><u>http://blogs.msdn.com/b/anilpras/archive/2012/05/23/server-certificate-bindings-and-its-restrictions-in-iis-6-0-amp-iis-7-x.aspx</u></font></a><o:p></o:p></span>
  </p>
  
  <p align="justify">
    <font size="2"></font>
  </p>
  
  <p class="MsoNormal" style="line-height: normal; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto;" align="justify">
    <span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"><font size="2">This has been finally addressed in Windows 8 and here are the solutions.</font></span>
  </p>
  
  <ul>
    <li>
      <div class="MsoNormal" style="line-height: normal; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto;" align="justify">
        <span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"><strong>Server Name Indication</strong> or <strong>SNI</strong></span>
      </div>
    </li>
    
    <li>
      <div class="MsoNormal" style="line-height: normal; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto;" align="justify">
        <span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"><strong>Central Certificate Store </strong>or <strong>CCS</strong></span>
      </div>
    </li>
  </ul>
  
  <p class="MsoNormal" style="line-height: normal; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto;" align="left">
    <span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"></span><span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"><font size="2">For SNI: </font><a title="http://learn.iis.net/page.aspx/1096/iis-80-server-name-indication-sni-ssl-scalability/" href="http://learn.iis.net/page.aspx/1096/iis-80-server-name-indication-sni-ssl-scalability/"><font color="#0000ff" size="2"><u>http://learn.iis.net/page.aspx/1096/iis-80-server-name-indication-sni-ssl-scalability/</u></font></a></span>
  </p>
  
  <p class="MsoNormal" style="line-height: normal; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto;" align="left">
    <span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"></span><span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"><font size="2">Also refer the Wiki article: </font><a href="http://en.wikipedia.org/wiki/Server_Name_Indication"><font color="#0000ff" size="2"><u>http://en.wikipedia.org/wiki/Server_Name_Indication</u></font></a><font size="2"> </font></span>
  </p>
  
  <p class="MsoNormal" style="line-height: normal; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto;" align="left">
    <span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"></span><span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"><font size="2">For CCS: <u><span style="color: blue;"><a title="http://learn.iis.net/page.aspx/1091/iis-80-centralized-ssl-certificate-support-ssl-scalability-and-manageability/" href="http://learn.iis.net/page.aspx/1091/iis-80-centralized-ssl-certificate-support-ssl-scalability-and-manageability/"><font color="#0000ff">http://learn.iis.net/page.aspx/1091/iis-80-centralized-ssl-certificate-support-ssl-scalability-and-manageability/</font></a></span></u></font></span>
  </p>
  
  <p align="justify">
    <p class="MsoNormal" style="line-height: normal; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto;" align="justify">
      <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-fareast-language: en-in; mso-no-proof: yes;"><font size="2">The result of this change is that now you would see 2 additional entries under the following registry key as shown below:</font></span>
    </p>
    
    <p align="justify">
      <p class="MsoNormal" style="line-height: normal; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto;" align="justify">
        <span style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-fareast-language: en-in; mso-no-proof: yes;"><font style="background-color: rgb(255, 255, 0);"><b style="mso-bidi-font-weight: normal;"><font size="2">HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\HTTP\Parameters</font></b> </font></span>
      </p>
      
      <p align="justify">
        <p class="MsoNormal" style="line-height: normal; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto;" align="justify">
          <a href="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/5811.image_7E3F0F5E.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/5811.image_5F00_7E3F0F5E.png"><img title="image" style="display: inline; background-image: none;" border="0" alt="image" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/6153.image_thumb_3C582A10.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/6153.image_5F00_thumb_5F00_3C582A10.png" width="606" height="208" /></a>
        </p>
        
        <p align="justify">
          <p class="MsoNormal" style="line-height: normal; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto;" align="justify">
            <span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"> <br /><font size="2">Let’s discuss these keys a little bit:</font></span>
          </p>
          
          <p class="MsoNormal" style="line-height: normal; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto;" align="justify">
            <span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"></span><font size="2"><span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Segoe UI&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"><span style="mso-list: ignore;"><strong>1.</strong><span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;"><font face="Segoe UI">&#160;&#160;&#160; </font></span></span></span><!--[endif]-->
            
            <b style="mso-bidi-font-weight: normal;"><span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;">SslBindingsInfo</span></b></font><span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"><font size="2">: <br /><span style="mso-spacerun: yes;">&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span>This legacy registry key was also present in earlier version of Windows prior to Windows 8. The bindings were of the type <span class="SpellE"><b style="mso-bidi-font-weight: normal;">IP<span class="GramE">:Port</span></b></span>. Only one certificate could be associated with an entry (or that key) and hence the limitation. We could add multiple SSL bindings by creating multiple combination of <span class="SpellE"><b style="mso-bidi-font-weight: normal;">IP<span class="GramE">:Port</span></b></span> and then associating each with a SSL Server Certificate.</font> <o:p></o:p></span>
          </p>
          
          <p align="justify">
            <div align="justify">
              <table class="MsoTableGrid" style="border: currentcolor; margin-left: 36pt; border-collapse: collapse; mso-border-alt: solid #00b0f0 2.25pt; mso-yfti-tbllook: 1184; mso-padding-alt: 0cm 5.4pt 0cm 5.4pt; mso-border-insideh: 2.25pt solid #00b0f0; mso-border-insidev: 2.25pt solid #00b0f0;" cellspacing="0" cellpadding="0" border="1">
                <tr style="mso-yfti-irow: 0; mso-yfti-firstrow: yes; mso-yfti-lastrow: yes;">
                  <td style="background: rgb(0, 32, 96); padding: 0cm 5.4pt; border: 2.25pt solid rgb(0, 176, 240); width: 367.75pt;" valign="top" width="490">
                    <p class="MsoNormal" style="line-height: normal; margin-bottom: 0pt;">
                      <b style="mso-bidi-font-weight: normal;"><span lang="EN-US" style="color: white; font-family: &quot;Courier New&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en-us; mso-themecolor: background1;">SSL Certificate bindings:<o:p></o:p></span></b>
                    </p>
                    
                    <p class="MsoNormal" style="line-height: normal; margin-bottom: 0pt;">
                      <b style="mso-bidi-font-weight: normal;"><span lang="EN-US" style="color: white; font-family: &quot;Courier New&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en-us; mso-themecolor: background1;">&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8211;<o:p></o:p></span></b>
                    </p>
                    
                    <p class="MsoNormal" style="line-height: normal; margin-bottom: 0pt;">
                      <span class="SpellE"><b style="mso-bidi-font-weight: normal;"><span lang="EN-US" style="background: yellow; color: black; font-family: &quot;Courier New&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en-us; mso-themecolor: text1; mso-highlight: yellow;">IP:port</span></b></span><b style="mso-bidi-font-weight: normal;"><span lang="EN-US" style="color: black; font-family: &quot;Courier New&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en-us; mso-themecolor: text1;"><span style="mso-spacerun: yes;">&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></span></b><b style="mso-bidi-font-weight: normal;"><span lang="EN-US" style="color: white; font-family: &quot;Courier New&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en-us; mso-themecolor: background1;">: 192.168.1.1:443</span></b><b style="mso-bidi-font-weight: normal;"><span style="color: white; font-family: &quot;Courier New&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-themecolor: background1;"><o:p></o:p></span></b>
                    </p>
                    
                    <p class="MsoNormal" style="line-height: normal; margin-bottom: 0pt;">
                      <b style="mso-bidi-font-weight: normal;"><span lang="EN-US" style="color: white; font-family: &quot;Courier New&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en-us; mso-themecolor: background1;">Certificate Hash : 2114e944c1e63dcdcd033e5d3fdb832ba423a52e<o:p></o:p></span></b>
                    </p>
                    
                    <p class="MsoNormal" style="line-height: normal; margin-bottom: 0pt;">
                      <b style="mso-bidi-font-weight: normal;"><span lang="EN-US" style="color: white; font-family: &quot;Courier New&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en-us; mso-themecolor: background1;">&#8230;</span></b><b style="mso-bidi-font-weight: normal;"><span style="font-family: &quot;Courier New&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in;"><o:p></o:p></span></b>
                    </p>
                  </td>
                </tr>
              </table>
            </div>
            
            <p align="justify">
              <p class="MsoListParagraphCxSpFirst" style="line-height: normal; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto; mso-add-space: auto;" align="justify">
                <span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"><span style="mso-spacerun: yes;">&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span><font size="2">The problem was that it was not feasible to have multiple ports open on the server. The ideal choice was always going to be the default SSL <b style="mso-bidi-font-weight: normal;">443</b>. So this suggests that we need to have more IP Addresses on the server. In the real world, this is not an acceptable solution and hence we had to use SAN or Wild Card certificates.</font></span>
              </p>
              
              <p class="MsoListParagraphCxSpFirst" style="line-height: normal; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto; mso-add-space: auto;" align="justify">
                <span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"></span><font size="2"><b style="mso-bidi-font-weight: normal;"><span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Segoe UI&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"><span style="mso-list: ignore;">2.<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;"><font face="Segoe UI">&#160;&#160;&#160; </font></span></span></span></b><!--[endif]-->
                
                <b style="mso-bidi-font-weight: normal;"><span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;">SslSniBindingsInfo</span></b></font><span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"><font size="2">:</font><b style="mso-bidi-font-weight: normal;"> <br /><font size="2"><span style="mso-spacerun: yes;">&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span></font></b><font size="2">This is<b style="mso-bidi-font-weight: normal;"> </b>new in<b style="mso-bidi-font-weight: normal;"> </b>Windows 8 and is not available in previous Windows Versions. The bindings are of the type <b style="mso-bidi-font-weight: normal;">Hostname:Port</b>. As the previous one, only one certificate could be bound to <b style="mso-bidi-font-weight: normal;">Hostname<span class="GramE">:Port</span></b> key.<b style="mso-bidi-font-weight: normal;"><o:p></o:p></b></font></span>
              </p>
              
              <p align="justify">
                <div align="justify">
                  <table class="MsoTableGrid" style="border: currentcolor; margin-left: 36pt; border-collapse: collapse; mso-border-alt: solid #00b0f0 2.25pt; mso-yfti-tbllook: 1184; mso-padding-alt: 0cm 5.4pt 0cm 5.4pt; mso-border-insideh: 2.25pt solid #00b0f0; mso-border-insidev: 2.25pt solid #00b0f0;" cellspacing="0" cellpadding="0" border="1">
                    <tr style="mso-yfti-irow: 0; mso-yfti-firstrow: yes; mso-yfti-lastrow: yes;">
                      <td style="background: rgb(0, 32, 96); padding: 0cm 5.4pt; border: 2.25pt solid rgb(0, 176, 240); width: 367.75pt;" valign="top" width="490">
                        <p class="MsoNormal" style="line-height: normal; margin-bottom: 0pt;">
                          <b style="mso-bidi-font-weight: normal;"><span lang="EN-US" style="color: white; font-family: &quot;Courier New&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en-us; mso-themecolor: background1;">SSL Certificate bindings:<o:p></o:p></span></b>
                        </p>
                        
                        <p class="MsoNormal" style="line-height: normal; margin-bottom: 0pt;">
                          <b style="mso-bidi-font-weight: normal;"><span lang="EN-US" style="color: white; font-family: &quot;Courier New&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en-us; mso-themecolor: background1;">&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8211;<o:p></o:p></span></b>
                        </p>
                        
                        <p class="MsoNormal" style="line-height: normal; margin-bottom: 0pt;">
                          <span class="SpellE"><b style="mso-bidi-font-weight: normal;"><span lang="EN-US" style="background: yellow; color: black; font-family: &quot;Courier New&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en-us; mso-themecolor: text1; mso-highlight: yellow;">Hostname:port</span></b></span><b style="mso-bidi-font-weight: normal;"><span lang="EN-US" style="color: black; font-family: &quot;Courier New&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en-us; mso-themecolor: text1;"><span style="mso-spacerun: yes;">&#160;&#160;&#160; </span></span></b><b style="mso-bidi-font-weight: normal;"><span lang="EN-US" style="color: white; font-family: &quot;Courier New&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en-us; mso-themecolor: background1;">: www.mycontoso.com:443<o:p></o:p></span></b>
                        </p>
                        
                        <p class="MsoNormal" style="line-height: normal; margin-bottom: 0pt;">
                          <b style="mso-bidi-font-weight: normal;"><span lang="EN-US" style="color: white; font-family: &quot;Courier New&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en-us; mso-themecolor: background1;">Certificate Hash : 0e62ac0f4deb8d6d78ac93a3088157e624ee540b<o:p></o:p></span></b>
                        </p>
                        
                        <p class="MsoNormal" style="line-height: normal; margin-bottom: 0pt;">
                          <b style="mso-bidi-font-weight: normal;"><span lang="EN-US" style="color: white; font-family: &quot;Courier New&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en-us; mso-themecolor: background1;">&#8230;</span></b><b style="mso-bidi-font-weight: normal;"><span style="font-family: &quot;Courier New&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in;"><o:p></o:p></span></b>
                        </p>
                      </td>
                    </tr>
                  </table>
                </div>
                
                <p align="justify">
                  <p class="MsoListParagraphCxSpFirst" style="line-height: normal; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto; mso-add-space: auto;" align="justify">
                    <span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"><span style="mso-spacerun: yes;">&#160;&#160;&#160;&#160;&#160;&#160; <font size="2"></font></span><font size="2">In this case we don’t have to use additional IP Addresses. We can use the hostname present in the certificate and then continue using the default SSL Port 443. Since Hostnames are always unique, 2 bindings could never have the same certificate.</font></span>
                  </p>
                  
                  <p class="MsoListParagraphCxSpFirst" style="line-height: normal; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto; mso-add-space: auto;" align="justify">
                    <span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"></span><font size="2"><b style="mso-bidi-font-weight: normal;"><span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Segoe UI&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"><span style="mso-list: ignore;">3.<span style="font: 7pt/normal &quot;Times New Roman&quot;; font-size-adjust: none; font-stretch: normal;">&#160;&#160;&#160; </span></span></span></b><!--[endif]-->
                    
                    <b style="mso-bidi-font-weight: normal;"><span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;">SslCcsBindingsInfo</span></b></font><span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"><font size="2">: <br /><span style="mso-spacerun: yes;">&#160;&#160;&#160;&#160;&#160;&#160;&#160; </span>This is new in Windows 8 and was not available in earlier versions of Windows. True SSL Scalability was achieved with this. This reads the certificates from a File Share. There is only one binding for a specific port and you could have multiple Site listening on this binding. The <b style="mso-bidi-font-weight: normal;">Server certificate</b> is loaded based on hostname section available from the <b style="mso-bidi-font-weight: normal;">Client Hello</b> at run time. If you try to list out the SSL bindings then this is how it would look:<b style="mso-bidi-font-weight: normal;"><o:p></o:p></b></font></span>
                  </p>
                  
                  <p align="justify">
                    <div align="justify">
                      <table class="MsoTableGrid" style="background: rgb(0, 32, 96); border: currentcolor; margin-left: 36pt; border-collapse: collapse; mso-border-alt: solid #00b0f0 2.25pt; mso-yfti-tbllook: 1184; mso-padding-alt: 0cm 5.4pt 0cm 5.4pt; mso-border-insideh: 2.25pt solid #00b0f0; mso-border-insidev: 2.25pt solid #00b0f0;" cellspacing="0" cellpadding="0" border="1">
                        <tr style="mso-yfti-irow: 0; mso-yfti-firstrow: yes; mso-yfti-lastrow: yes;">
                          <td style="padding: 0cm 5.4pt; border: 2.25pt solid rgb(0, 176, 240); width: 367.75pt;" valign="top" width="490">
                            <p class="MsoNormal" style="line-height: normal; margin-bottom: 0pt;">
                              <b style="mso-bidi-font-weight: normal;"><span lang="EN-US" style="color: white; font-family: &quot;Courier New&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en-us; mso-themecolor: background1;">SSL Certificate bindings:<o:p></o:p></span></b>
                            </p>
                            
                            <p class="MsoNormal" style="line-height: normal; margin-bottom: 0pt;">
                              <b style="mso-bidi-font-weight: normal;"><span lang="EN-US" style="color: white; font-family: &quot;Courier New&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en-us; mso-themecolor: background1;">&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8212;&#8211;<o:p></o:p></span></b>
                            </p>
                            
                            <p class="MsoNormal" style="line-height: normal; margin-bottom: 0pt;">
                              <b style="mso-bidi-font-weight: normal;"><span lang="EN-US" style="background: yellow; color: black; font-family: &quot;Courier New&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en-us; mso-themecolor: text1; mso-highlight: yellow;">Central Certificate Store</span></b><b style="mso-bidi-font-weight: normal;"><span lang="EN-US" style="color: black; font-family: &quot;Courier New&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en-us; mso-themecolor: text1;"><span style="mso-spacerun: yes;">&#160;&#160;&#160; </span></span></b><b style="mso-bidi-font-weight: normal;"><span lang="EN-US" style="color: white; font-family: &quot;Courier New&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en-us; mso-themecolor: background1;">: www.mycontoso.com:443<o:p></o:p></span></b>
                            </p>
                            
                            <p class="MsoNormal" style="line-height: normal; margin-bottom: 0pt;">
                              <b style="mso-bidi-font-weight: normal;"><span lang="EN-US" style="color: white; font-family: &quot;Courier New&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en-us; mso-themecolor: background1;">Certificate Hash : 0e62ac0f4deb8d6d78ac93a3088157e624ee540b<o:p></o:p></span></b>
                            </p>
                            
                            <p class="MsoNormal" style="line-height: normal; margin-bottom: 0pt;">
                              <b style="mso-bidi-font-weight: normal;"><span lang="EN-US" style="color: white; font-family: &quot;Courier New&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en-us; mso-themecolor: background1;">&#8230;</span></b><b style="mso-bidi-font-weight: normal;"><span style="font-family: &quot;Courier New&quot;; font-size: 10pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in;"><o:p></o:p></span></b>
                            </p>
                          </td>
                        </tr>
                      </table>
                    </div>
                    
                    <p align="justify">
                      <p class="MsoListParagraphCxSpFirst" style="line-height: normal; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto; mso-add-space: auto;" align="justify">
                        <span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"><span style="mso-spacerun: yes;">&#160;&#160;&#160;&#160;&#160;&#160; <font size="2"></font></span><font size="2">This allows you to configure multiple sites on a single binding, as the certificates are loaded at run time. The management of certificates is also easier as we can have multiple certificates read from a central file location. If a certificate expires we can just update the certificate on that particular file share.</font></span>
                      </p>
                      
                      <p class="MsoListParagraphCxSpFirst" style="line-height: normal; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto; mso-add-space: auto;" align="justify">
                        <span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"></span>
                      </p>
                      
                      <p class="MsoListParagraphCxSpFirst" style="line-height: normal; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto; mso-add-space: auto;" align="justify">
                        <span lang="EN" style="font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"></span><span lang="EN" style="line-height: 107%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"><font size="2">I will blog in more detail on how this works with scenarios to help this understand better. There is more to the Central Certificate Store and I will blog multiple posts with more detailed explanation.</font></span>
                      </p>
                      
                      <p class="MsoListParagraphCxSpFirst" style="line-height: normal; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto; mso-add-space: auto;" align="justify">
                        <span lang="EN" style="line-height: 107%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"></span>
                      </p>
                      
                      <p class="MsoListParagraphCxSpFirst" style="line-height: normal; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto; mso-add-space: auto;" align="justify">
                        <span lang="EN" style="line-height: 107%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"></span><font size="2" face="Segoe UI">You can read more on IIS 8 here:</font>
                      </p>
                      
                      <p class="MsoListParagraphCxSpFirst" style="line-height: normal; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto; mso-add-space: auto;" align="justify">
                        <a href="http://weblogs.asp.net/owscott/archive/2012/03/01/what-s-new-in-iis-8.aspx"><font color="#0000ff" size="2" face="Segoe UI"><u>http://weblogs.asp.net/owscott/archive/2012/03/01/what-s-new-in-iis-8.aspx</u></font></a><font color="#0000ff"><u> <br /><font size="2" face="Segoe UI"></font></u></font><a href="http://learn.iis.net/page.aspx/1087/what39s-new-in-iis-80-for-windows-8/"><font color="#0000ff" size="2" face="Segoe UI"><u>http://learn.iis.net/page.aspx/1087/what39s-new-in-iis-80-for-windows-8/</u></font></a><font color="#0000ff"><u> <br /><font size="2" face="Segoe UI"></font></u></font><a href="http://technet.microsoft.com/en-us/library/hh831725.aspx"><font color="#0000ff" size="2" face="Segoe UI"><u>http://technet.microsoft.com/en-us/library/hh831725.aspx</u></font></a>
                      </p>
                      
                      <p align="justify">
                        <p align="justify">
                          <span lang="EN" style="line-height: 107%; font-family: &quot;Segoe UI&quot;,&quot;sans-serif&quot;; font-size: 12pt; mso-fareast-font-family: &quot;Times New Roman&quot;; mso-font-kerning: 0pt; mso-ligatures: none; mso-fareast-language: en-in; mso-ansi-language: en;"><font size="2">Until then. Adios! <img class="wlEmoticon wlEmoticon-smile" alt="Smile" src="https://msdnshared.blob.core.windows.net/media/MSDNBlogsFS/prod.evol.blogs.msdn.com/CommunityServer.Blogs.Components.WeblogFiles/00/00/01/38/03/metablogapi/2744.wlEmoticon-smile_5336FB8C.png" original-url="http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-weblogfiles/00-00-01-38-03-metablogapi/2744.wlEmoticon_2D00_smile_5F00_5336FB8C.png" /></font></span>
                        </p>
                        
                        <p align="justify">
                          <!--?xml:namespace prefix = "o" /--><o:p></o:p>
                        </p>