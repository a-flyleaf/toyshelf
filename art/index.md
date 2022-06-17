---
layout: 1
title: art feed
css: "#art{display:none;}"
---
All the art on this site, ordered chronologically.
<!--200x200 JPG90%-->

<div id="gallery">{%-for art in site.art-%}
	<a href="{%include url.html%}/{{art.url}}"><img src="{%include url.html%}/assets/img/art/{{art.date|date:"%F"}}-tn.jpg" alt="{{art.title}}"/></a>
{%-endfor-%}</div>

<!--not quite sure how I want to handle this yet but storing the code anyway
<div id="gallery">{%for art in site.art%}{%capture year%}{{art.date|date:"%Y"}}{%endcapture%}{%if year<="2013"%}<a href="{{art.url}}"><img src="{%include url.html%}/assets/img/art/{{art.date|date:"%F"}}-tn.jpg" alt="{{art.title}}"/></a>{%endif%}{%endfor%}</div>
-->