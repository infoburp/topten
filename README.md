# topten
top ten singles on the UK chart from json endpoint (live data)

endpoint url
------------

example item
------------
{"position":1,"previousPosition":1,"numWeeks":3,"artist":"Ellie Goulding","title":"Love Me Like You Do","change":{"direction":"none","amount":0,"actual":0}}

page layout/stylesheet
----------------------
ordered list of top ten positions

<ol>
	<li>ARTIST-TITLE</li>
</ol>

colour background by change (down=red value,up=green value,blue=no move)

automatic youtube embedding
---------------------------
<script src="http://www.yvoschaap.com/ytpage/ytembed.js" type="text/javascript"></script>
<div id="ytThumbs"></div>

<script type="text/javascript">
	ytEmbed.init({'block':'ytThumbs','q':'ellie goulding love me like you do','type':'search','results':1,'order':'most_relevance','player':'embed','layout':'full'});
</script>

http://www.yvoschaap.com/youtube.html

+some custom jquery

chart loading
-------------

jquery code to load current top40 from endpoint url : "http://ben-major.co.uk/labs/top40/api/singles/" and cut it down to the top ten, before feeding this data into the page layout..
