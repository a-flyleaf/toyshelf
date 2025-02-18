---
layout: 1
title: art feed
css: "#art{display:none;}"
---
All the art on this site, ordered chronologically.
<!--200x200 JPG90%-->

<div id="gallery">{%-for art in site.art-%}
	<a href="{%include url.html%}{{art.url}}"><img src="{%include url.html%}/assets/img/art/{{art.date|date:"%F"}}-tn.jpg" alt="{{art.title}}"/></a>
{%-endfor-%}</div>