**Who am i:**<br><b>my name is meir yanovich and im c++/java developer mostly doing server infra cross  platform (unix/linux/window) stuff in my day job.</b><br>
but sometimes i like to experiment stuff in my spare time.<br>
also If you interested in facebook api and ways to interact this project may interest<br> you:<br><a href='http://code.google.com/p/facebook-cpp-graph-api/'>http://code.google.com/p/facebook-cpp-graph-api/</a><br>
or if you have young kids:<br>
<a href='http://code.google.com/p/kidsbrowser/'>http://code.google.com/p/kidsbrowser/</a><br>

<br>
you can find my on-line profile in here :<br>
<a href='http://il.linkedin.com/in/meiryanovich'>http://il.linkedin.com/in/meiryanovich</a> <br>
if you have any cool ideas on how to use this code and you need help please email me<br>
Email: meiry242@gmail.com<br><br>
twitter: <a href='https://twitter.com/meiryanovich'>https://twitter.com/meiryanovich</a><br>



<b><i>Implementation of web crawler / spider in c++</i></b> <br>
------------------------------------------------------------------------------------<br><br>


Web crawler / spider used for web data mining or data aggregations <br>
<ul><li>using  regular expressions rules to collect data.<br>
</li><li>Programmed using pure c++ (stl) and bunch of open source libraries.<br>
</li><li>web spider that can fallow links based on single domain.<br>
</li><li>output to xml file with configurable tags.</li></ul>

I tried to keep the "keep it simple keep it clean"  rule , using as much of ready made open source c/c++ libraries.<br>

<b><i>How to build  it:</i></b><br>
The application only tested on windows xp 32 bit although I pay attention on using only cross platform libraries.<br>
and not to write OS depended code.<br>
The libraries the Driller depend  on are :<br>
<ul><li><a href='http://www.pcre.org/'>pcre</a> : for regular expressions.<br>
</li><li><a href='http://sources.redhat.com/pthreads-win32/'>Pthreads</a> : for cross platform threads wrapper.<br>
</li><li><a href='http://curl.haxx.se/'>Curl</a> + <a href='http://c-ares.haxx.se/'>c-ares</a> : for http requests / response.<br>
In Driller source code I supply visual studio express 2008 solution and project files and all the libraries are already<br>
build in debug mode. all you have to do is configure it and build it<br>
this will save you time on configuring and compiling to test the application.<br>
for more information see <a href='http://code.google.com/p/driller-cpp-web-crawler/wiki/how_to_build_drill?ts=1301911759&updated=how_to_build_drill'>*how_to_build_drill*</a><br><br>
<b><i>How to configure it:</i></b><br>
The driller web spider doesn’t come with fancy configuration GUI or configuration file.<br>
All configurations must be done in code , then compile it then run it and see the results come in.<br>
The reasons is because I used it for my personal use without much time in my hands and didn't planed to<br>
Open source it ..any way all those features will be added later.<br>
Step by step guide can be found here in <a href='http://code.google.com/p/driller-cpp-web-crawler/wiki/how_to_configure_drill'>how_to_configure_drill</a>.<br><br><br>
if you find this useful consider to donate.<br> all donations will go to charity.<br>
<a href='https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=MDEDYTWMS8JKL&lc=IL&item_name=open%20source%20facebook%20graph%20api&item_number=1&currency_code=USD&bn=PP%2dDonationsBF%3abtn_donateCC_LG%2egif%3aNonHosted'><img src='https://www.paypal.com/en_US/i/btn/btn_donateCC_LG.gif' /></a></li></ul>


