p2pool_fancy_front_end
======================

Front end that can be co-located on a separate web server or hosted on the p2pool node.

you can see it running at http://www.norgzpool.net.au

This code is based on goblins stats code https://github.com/m3ta/p2pool-stats-2 from the extended front end for p2pool https://github.com/hardcpp/P2PoolExtendedFrontEnd

I have attempted to add comments where I can but please keep in mind much of this is taken from the above projects. 

Please support the original authors if you can, if you wish to help me out then you may donate to 1BCspL7f75gcU17M62524KSnfh7tyy3ZnF.

Much of the styling is done in css, specifically the bootstrap-responsive.css, menu styling is done in component.css.

Much of the data is taken from json and leverages jquery. 

<h1>How to get it working on your node:</h1>

<b>Step 1.</b> copy the code to the root web folder of your hosting platform or to the web-static folder of p2pool.

<b>Step 2.</b> In the index.html graphs.html and stats.html change "var server = "http://localhost:9332";" to reflect the remote node address or leave if runing on the local web-static folder.

<b>Step 3.</b> load your own logo for the header. make it 711x150 pixels or as close to that as you can. it can be jpg, png or gif and you change it in the header div of the index and other pages <img src="yourlogo" (the dreamweaver template is included if you want to use that so you only change in the index and template).

<b>Step 4.</b> Edit div class="infobox" and include your node address and how to connect. This box can be hidden by clicking the X.

<b>Step 5.</b> edit "Introduction and info on your node goes here" with some info on your node. "Box for more information" can be edited to include other info or news.

<b>Step 6.</b> browse and enjoy p2pool stats in a nice interface and using standard port 80

<b>Step 7.</b> Remove or change the footer donation link and refferal link


Sorry in advance if something is not clear, I am not a developer, I just know enough to piece things together. Happy to assist if required. 

Note: If i have missed crediting anyone or there is something here you do not wish to be redistributed please accept my appology and contact me to have it removed immediately. 

<h1>Known Issues:</h1>

pie charts on graph page do not work


<h1>To Do:</h1>

1. remove server config to external files to make running multiple nodes easier - In progress now only in one place per page in v 0.6
2. find a way to make the info pane stay away if user clicks it away then refreshes
3. add more commenting - in progress
4. find a way to fix the external json issue with the node_ststus front and and integrate the highflow charts from that
5. change code to enable one set of html to connect to different nodes via menu click. i.e. onclick set var to server address, instead of having a full set og html for each node.
