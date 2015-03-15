# Introduction #

How to configure Drill (the web spider)<br>
<b>Note:</b> this is the first draft of the configuration ,<br>
I understand some logic will be hard to grasp at first , I will try to explain in simple words as I can<br>
The configuration is done in code this means hard coded. <br>


<h1>Details</h1>

Add your content here.  Format your content with:<br>
<ul><li>Define the url you like to drill down with the spider, Find the <b>drill.cpp</b> file & look for linkVec.push_back(<code>"http://www.xxxx.com/somthing/"</code>)<code>;</code> Here instead of the string enter the site url.<br>
</li><li>Find the file <b>Config.cpp</b> , there you will find different data structures that needs to be filled.<br>
<ol><li><i>infoHolder.linksBlackList.insert (…)</i> , are the strings that shouldn't be in the links the spider follow.for example if you define infoHolder.linksBlackList.insert ("#comments")  all links that contain this string will be ignored<br>
</li><li><i>infoHolder.linksMastHaveList.insert(…)</i> are the strings that must be in in the links the spider follow .this is to insure the spider stays in our target web site scope.for example: infoHolder.linksMastHaveList.insert(<code>"http://www.xxxx.com/somthing"</code>)<code>;</code>
</li><li>infoHolder.BaseUrl again to insure the spider stays in our target web site scope for example : <i>infoHolder.BaseUrl = <code>"http://www.xxxx.com/"</code></i>
</li><li><i>infoHolder.iThreadsToInvoke = 1</i> ; how much threads to invoke  <i>infoHolder.iThreadPoolSize = 1</i> ; thread pool size please keep it single threads for now the multi thread option still very experimental<br>
</li><li>Scraplet are regexp units each unit hold rule . the rule is regexp that capture/scrap string from the current web page the drill spider visit <i>Scraplet.regExp</i> : is the regexp string  <i>Scraplet.IsUnique</i> : looks only for one pattern result of the regexp if true,if false meny patterns can be capture in the same page<br>
</li></ol></li></ul><ul><li>Find the file <b>ProcessingUnit.cpp</b> search for the   <i>HandlePageScanResults</i>  function here you will configure the xml output file .basclly you poll the keys you defined in the Config.cpp Hash map and Concat strings to build the xml look at the code it very straightforward.