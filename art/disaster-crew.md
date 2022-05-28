---
layout: 1
title: disaster crew art feed
css: "#art{display:none;}"
---
All [art]({%include url.html%}/art) pertaining to the [disaster crew]({%include url.html%}/disaster-crew) specifically. (Currently redundant with the general art page, but this could change later.)

<div id="gallery">{%for art in site.art%}<a href="{{art.url}}"><img src="{%include url.html%}/assets/img/art/{{art.date|date:"%F"}}-tn.jpg" alt="{{art.title}}"/></a>{%endfor%}</div>