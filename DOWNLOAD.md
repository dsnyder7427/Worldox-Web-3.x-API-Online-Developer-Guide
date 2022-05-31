<?xml version="1.0" encoding="utf-8" ?>
<!DOCTYPE html>
<html xmlns="http://www.w3.org/1999/xhtml"><head>

  <script type="text/javascript" language="JavaScript">
    //<![CDATA[
    function reDo() {
      if (innerWidth != origWidth || innerHeight != origHeight)
        location.reload();
    }
    if ((parseInt(navigator.appVersion) == 4) && (navigator.appName == "Netscape")) {
      origWidth = innerWidth;
      origHeight = innerHeight;
      onresize = reDo;
    }
    onerror = null;
  //]]>
  </script>
  <style type="text/css">/*<![CDATA[*/

    < !-- div.WebHelpPopupMenu {
      position: absolute;
      left: 0px;
      top: 0px;
      z-index: 4;
      visibility: hidden;
    }

    p.WebHelpNavBar {
      text-align: right;
    }

    -->
  
/*]]>*/</style>

  <script type="text/javascript">//<![CDATA[

    gRootRelPath = ".";
    gCommonRootRelPath = ".";
    gTopicId = "0_10";
  
//]]></script>

  <script type="text/javascript" src="./template/scripts/rh.min.js"></script>
  <script type="text/javascript" src="./template/scripts/common.min.js"></script>
  <script type="text/javascript" src="./template/scripts/topic.min.js"></script>
  <script type="text/javascript" src="./template/scripts/topicwidgets.min.js"></script>
<script type="text/javascript" src="./whxdata/projectsettings.js"></script>
  <link rel="stylesheet" type="text/css" href="./template/styles/topic.min.css"/>
  <link rel="stylesheet" type="text/css" href="./template/Blue_Worldox/topicheader.css"/>
  <meta name="topic-status" content="Draft"/>

<meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
<meta name="OriginalFile" content="DOWNLOAD.DOCX"/>
<meta name="generator" content="Adobe RoboHelp 2020"/>
<title>DOWNLOAD</title>
<link rel="StyleSheet" href="assets/css/htmlhelp.css" type="text/css"/>
<meta name="rh-index-keywords" content="downloading files,DOWNLOAD command"/></head>

<body style="word-wrap: break-word;">
  <div class="topic-header rh-hide" id="rh-topic-header" onclick="rh._.goToFullLayout()">
    <div class="logo">
    </div>
    <div class="nav">
      <div class="title" title="DOWNLOAD">
        <span>DOWNLOAD</span>
      </div>
      <div class="gotohome" title="Click here to see this page in full context">
        <span>Click here to see this page in full context</span>
      </div>
    </div>
  </div>
  <div class="topic-header-shadow rh-hide" id="rh-topic-header-shadow"></div>



<h1>DOWNLOAD</h1>
<p>The DOWNLOAD command prepares a file for download. This is a GET request.</p>
<p class="Bullet_list"><a href="#DOWNLOAD_Example">DOWNLOAD_Example</a></p>
<p class="Bullet_list"><a href="#JSON_Successful_DOWNLOAD_Response">JSON_Successful_DOWNLOAD_Response</a></p>
<p class="Bullet_list"><a href="#JSON_Successful_DOWNLOAD_Response">JSON_Successful_DOWNLOAD_Response</a></p>
<p> </p>
<h2><a id="DOWNLOAD_Example"></a>DOWNLOAD Example</h2>
<p class="Code">{Worldox Web Domain}  +  &#39;cgi-bin/wdwebcgi.exe?DOWNLOAD&amp;wd_SID=&#39; 
 + {Worldox Web User Session) + &#39;&amp;html=v4/fileActions/download.json&amp;wd_List_RecNum=&#39; 
 + x.RN + &#39;&amp;wd_List_ID=&#39; + x.LID + &#39;&amp;wd_List_Offset=&#39; + x.LN</p>
<h3>Parameters</h3>
<p class="Code">HTMLOnOK</p>
<p style="text-indent: .5in;">This is the page to return on a successful 
 call to DOWNLOAD.</p>
<p class="Code" style="text-indent: .5in;">v4 \fileActions\download.json</p>
<p class="Code" style="text-indent: .5in;"><b><span style="font-size: 11.0pt; 
													 font-family: Calibri, sans-serif; 
													 color: windowtext;">Note:</span></b> 
 api <span style="font-size: 11.0pt; font-family: Calibri, sans-serif; 
			 color: windowtext;">is deprecated but still can be used. Going 
 forward</span> v4 <span style="font-size: 11.0pt; font-family: Calibri, sans-serif; 
						 color: windowtext;">is the best practice.</span></p>
<p class="Code">HTMLOnFail</p>
<p style="text-indent: .5in;">This is the page to return on a failed DOWNLOAD.</p>
<p class="Code" style="text-indent: .5in;">v4 \fileActions\download.json</p>
<p class="Code" style="text-indent: .5in;"><b><span style="font-size: 11.0pt; 
													 font-family: Calibri, sans-serif; 
													 color: windowtext;">Note:</span></b> 
 api <span style="font-size: 11.0pt; font-family: Calibri, sans-serif; 
			 color: windowtext;">is deprecated but still can be used. Going 
 forward</span> v4 <span style="font-size: 11.0pt; font-family: Calibri, sans-serif; 
						 color: windowtext;">is the best practice.</span></p>
<p class="Code">{Worldox Web Domain}</p>
<p>                Is 
 the domain name.</p>
<p class="Code">wd_SID</p>
<p>                Is 
 the session ID</p>
<p class="Code">{Worldox Web User Session)</p>
<p>                Is 
 the variable</p>
<p class="Code">wd_List_RecNum</p>
<p style="text-indent: .5in;">Is the record number of the files in the 
 list that you want to download.</p>
<p class="Code">wd_List_ID</p>
<p style="text-indent: .5in;">Is the record number of the file on the list 
 that you want to download</p>
<p class="Code">wd_List_Offset</p>
<p style="margin-left: .5in;">(Starting offset) set to 1</p>
<p class="up_arrow"><span style="font-style: italic; font-weight: bold;"><i><b><a href="#"><img src="assets/images/up_arrow.gif" alt="up_arrow.gif" title="up_arrow.gif" style="border: none;" width="14" height="16" border="0"/></a></b></i></span></p>
<h2><a id="JSON_Successful_DOWNLOAD_Response"></a>JSON Successful DOWNLOAD 
 Response</h2>
<p><b>Note:</b> You can view the file’s location in the fileLoc line. You 
 can view the file’s name in the FileNme line. <a id="fileLoc" data-indexterm="fileLoc"></a><a id="fileNme" data-indexterm="fileNme"></a><a name="Note_You_can_view_the" id="Note_You_can_view_the"></a></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">{</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">    </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;root&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: {</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">        </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;data&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: {</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;fileLoc&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;/cgi-bin/WDSIDS/1FZMVYfcOQrBNmi8kr3HWUuwCGHwTYqLNJX4XMEokPlk0D2sQKhwMWBz2FE%243D/OPEN/005/20000/200/Terms%20and%20Conditions%20of%20QC%20%2800001079-2x51615%29.DOC&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;FileNme&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;Terms%20and%20Conditions%20of%20QC%20%2800001079-2x51615%29.DOC&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;FileZMS&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;\\WORLDOX\\ZMS\\005\\20000\\200\\00001079.DOC&quot;</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">        },</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">        </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;errorStatus&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: {</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;ErrorCount&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_RCID&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_RCTX&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_MSG&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_VAR&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_VAL&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_DOCID&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_DOCNAME&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;req_ID&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;Error&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;&quot;</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">        }</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">    }</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">}</span></p>
<span style="font-size: 9.0pt; font-family: Consolas; color: #000000;"><br style="clear: all;" clear="all"/>
</span> 
<p style="margin: 0in;"> </p>
<p class="up_arrow"><span style="font-style: italic; font-weight: bold;"><i><b><a href="#"><img src="assets/images/up_arrow.gif" alt="up_arrow.gif" title="up_arrow.gif" style="border: none;" width="14" height="16" border="0"/></a></b></i></span></p>
<h2><a id="JSON_Failed_DOWNLOAD_Response"></a>JSON Failed DOWNLOAD Response</h2>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">{</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">    </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;root&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: {</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">        </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;data&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: {</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;fileLoc&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;FileNme&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;FileZMS&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;&quot;</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">        },</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">        </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;errorStatus&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: {</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515; background: #ffff00;">&quot;ErrorCount&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000; background: #ffff00;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5; background: #ffff00;">&quot;2&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000; background: #ffff00;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_RCID&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;8525&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_RCTX&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;WDRC_PATH_INVALID&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_MSG&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;Invalid Path\n\n\nThe path is invalid.\n\n\n\n\nOK\n&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_VAR&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_VAL&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_DOCID&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_DOCNAME&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;req_ID&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;Error&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: [</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">                {</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">                    </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_RCID&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;8525&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">                    </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_RCTX&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;WDRC_PATH_INVALID&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">                    </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_MSG&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;Invalid Path\n\n\nThe path is invalid.\n\n\n\n\nOK\n&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">                    </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_VAR&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">                    </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_VAL&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;&quot;</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">                },</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">                {</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">                    </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_RCID&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;8380&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">                    </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_RCTX&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;WDRC_LISTID_UNDEFINED&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">                    </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_MSG&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;Error no List ID\nYour request returned without a &#39;List ID&#39;, please refresh.\n\n\n\n\nlock, wdInfo\ncloseCircle, wdErrorIco\n\nRefresh\n&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">                    </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_VAR&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">                    </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_VAL&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;&quot;</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">                }</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            ]</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">        }</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">    }</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe; 
	 font-size: 9.0pt; font-family: Consolas; color: #000000;">}</p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"> </p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe; 
	 font-size: 9.0pt; font-family: Consolas; color: #000000;"> </p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe; 
	 font-size: 9.0pt; font-family: Consolas; color: #000000;"> </p>
<span style="font-size: 9.0pt; font-family: Consolas; color: #000000;"><br style="clear: all;" clear="all"/>
</span> 
<p class="up_arrow"><span style="font-style: italic; font-weight: bold;"><i><b><a href="#"><img src="assets/images/up_arrow.gif" alt="up_arrow.gif" title="up_arrow.gif" style="border: none;" width="14" height="16" border="0"/></a></b></i></span></p>
<p style="margin: 0in;"> </p>
<p> </p>
<p><script type="text/javascript">//<![CDATA[
var mailSubject = 'Useful online help topic'; 
var mailBody    = 'This online help page might help: ' + location.href; 
var mailDisplay = 'Email this topic to another user.'; 
document.write( 
    '<a href="mailto:yourname@yourSite.com' 
    + '?subject=' + escape(mailSubject) 
    + '&body=' + escape(mailBody) 
    + '">' + mailDisplay + '<\/a>' 
    );
//]]></script></p>

</body></html>