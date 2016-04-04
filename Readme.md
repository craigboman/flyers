Html, javascript, and CSS code for flyers.udayton.edu

Although the majority of this code may be used freely, some fonts may be licensed. If licensed font is used by you or your organization, the authors of this code bear no responsibility for your unlicensed use of someone else's fonts.

This repository was designed by a library for the purposes of searching a library catalog. Using this code for other purposes may be useless and futile. Any errors caused by the use of this code on your web servers are your own fault and not the fault of the authors of this respository. These errors only show you probably don't know how to do html and javascript coding. 

This code is provided to your feely, but it would be appropriate if you recognized the use of our code publicly or privately. Perhaps mail us a letter letting us know how appreciative you are for our hard work. If you use a lot of our code perhaps leave an html comment in your code stating <!--thanks to flyers.udayton.edu for use of their awesome code -->.

It is expected that no support will be provided by these authors. The code is <b>AS-IS</b>. Best of luck. Having said that, please review these notes below for more information.

<b>Build Notes (or notes to help you/us [re]implement our code)</b>

1. We combined all of the searchhelp_x.html files into one file and then we use a bat file to copy the contents of the index.html into all of the searchhelp_*.html pages. If you make changes to index.html, run the /search/batch_srchelp.bat file to copy its contents programmatically.
<pre><code>
cat ../index.html > mainmenu.html
cat ../index.html > srchhelp_X_nojavascript.html
</pre></code>
As a result, /search directory above is effectively your /screens directory, minus index.html, briefcit.html, and bibdisplay.html

2. On bibdisplay.html, we made most of the buttons generated by the navrow token css style hidden. This allows us to use a javascript to load those navrow buttons any where else on the page.

3. After patrons log in, we have not made these pages responsive yet (it is not a bug).