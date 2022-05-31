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
    gTopicId = "0_9";
  
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
<meta name="OriginalFile" content="CLOSELIST.DOCX"/>
<meta name="generator" content="Adobe RoboHelp 2020"/>
<title>CLOSELIST</title>
<link rel="StyleSheet" href="assets/css/htmlhelp.css" type="text/css"/>
<meta name="rh-index-keywords" content="closing lists,CLOSELIST command"/></head>

<body style="word-wrap: break-word;">
  <div class="topic-header rh-hide" id="rh-topic-header" onclick="rh._.goToFullLayout()">
    <div class="logo">
    </div>
    <div class="nav">
      <div class="title" title="CLOSELIST">
        <span>CLOSELIST</span>
      </div>
      <div class="gotohome" title="Click here to see this page in full context">
        <span>Click here to see this page in full context</span>
      </div>
    </div>
  </div>
  <div class="topic-header-shadow rh-hide" id="rh-topic-header-shadow"></div>



<h1>CLOSELIST</h1>
<p>The CLOSELIST command closes the Worldox Web file list.</p>
<p class="Bullet_list"><a href="#CLOSELIST_Example">CLOSELIST_Example</a></p>
<p class="Bullet_list"><a href="#JSON_Successful_CLOSELIST_Response">JSON_Successful_CLOSELIST_Response</a></p>
<p class="Bullet_list"><a href="#JSON_Failed_CLOSELIST_Response">JSON_Failed_CLOSELIST_Response</a></p>
<h3> </h3>
<h2><a id="CLOSELIST_Example"></a>CLOSELIST Example</h2>
<p class="Code">/cgi-bin/wdwebcgi.exe?CLOSELIST&amp;wd_SID={{session}}</p>
<h3>Parameters</h3>
<p class="Code">wd_SID</p>
<p style="text-indent: .5in;">The Worldox session ID</p>
<p class="Code">wd_List_ID</p>
<p style="text-indent: .5in;">The Worldox list to close</p>
<p class="Code">HTMLOnOK</p>
<p style="text-indent: .5in;">This is the page to return on a successful 
 call to CLOSELIST.</p>
<p class="Code" style="text-indent: .5in;">v4\fileActions\closeList.json</p>
<p class="Code" style="text-indent: .5in;"><b><span style="font-size: 11.0pt; 
													 font-family: Calibri, sans-serif; 
													 color: windowtext;">Note:</span></b> 
 api <span style="font-size: 11.0pt; font-family: Calibri, sans-serif; 
			 color: windowtext;">is deprecated but still can be used. Going 
 forward</span> v4 <span style="font-size: 11.0pt; font-family: Calibri, sans-serif; 
						 color: windowtext;">is the best practice.</span></p>
<p class="Code">HTMLOnFail</p>
<p style="text-indent: .5in;">This is the page to return on a failed CLOSELIST.</p>
<p class="Code" style="text-indent: .5in;">v4\fileActions\closeList.json</p>
<p class="Code" style="text-indent: .5in;"><b><span style="font-size: 11.0pt; 
													 font-family: Calibri, sans-serif; 
													 color: windowtext;">Note:</span></b> 
 api <span style="font-size: 11.0pt; font-family: Calibri, sans-serif; 
			 color: windowtext;">is deprecated but still can be used. Going 
 forward</span> v4 <span style="font-size: 11.0pt; font-family: Calibri, sans-serif; 
						 color: windowtext;">is the best practice.</span></p>
<p class="up_arrow"><span style="font-style: italic; font-weight: bold;"><i><b><a href="#"><img src="assets/images/up_arrow.gif" alt="up_arrow.gif" title="up_arrow.gif" style="border: none;" width="14" height="16" border="0"/></a></b></i></span></p>
<h2><a id="JSON_Successful_CLOSELIST_Response"></a>JSON Successful CLOSELIST 
 Response</h2>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">{</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">    </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;root&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: {</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">        </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;errorStatus&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: {</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;ErrorCount&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_RCID&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_RCTX&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_MSG&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_VAR&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_VAL&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;&quot;</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">        },</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">        </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;data&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;&quot;</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">    }</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">}</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"> </p>
<h2><a id="JSON_Failed_CLOSELIST_Response"></a>JSON Failed CLOSELIST 
 Response</h2>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">{</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">    </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;root&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: {</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">        </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;errorStatus&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: {</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515; background: #ffff00;">&quot;ErrorCount&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000; background: #ffff00;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5; background: #ffff00;">&quot;1&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000; background: #ffff00;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_RCID&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;8380&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_RCTX&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;WDRC_LISTID_UNDEFINED&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_MSG&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;Error no List ID\nYour request returned without a &#39;List ID&#39;, please refresh.\n\n\n\n\nlock, wdInfo\ncloseCircle, wdErrorIco\n\nRefresh\n&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_VAR&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">,</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">            </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;wd_Error_VAL&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;&quot;</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">        },</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">        </span><span style="font-size: 9.0pt; font-family: Consolas; color: #A31515;">&quot;data&quot;</span><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">: </span><span style="font-size: 9.0pt; font-family: Consolas; color: #0451A5;">&quot;&quot;</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">    }</span></p>
<p style="margin: 0in; line-height: 13.5pt; background-color: #fffffe;"><span style="font-size: 9.0pt; font-family: Consolas; color: #000000;">}</span></p>
<p> </p>
<p class="up_arrow"><span style="font-style: italic; font-weight: bold;"><i><b><a href="#"><img src="assets/images/up_arrow.gif" alt="up_arrow.gif" title="up_arrow.gif" style="border: none;" width="14" height="16" border="0"/></a></b></i></span></p>
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