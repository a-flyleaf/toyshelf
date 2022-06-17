---
layout: 1
title: "art: miscellaneous characters"
date: 2021-11-14
artsrc: menagerie
css: "#date,#info{display:none;} #art img{border:0;}"
---
All [art]({%include url.html%}/art) featuring one or more of [the miscellaneous characters]({%include url.html%}/misc).

<div id="gallery">{%for art in site.art%}{%if art.categories contains "misc"%}<a href="{%include url.html%}/{{art.url}}"><img src="{%include url.html%}/assets/img/art/{{art.date|date:"%F"}}-tn.jpg" alt="{{art.title}}"/></a>{%endif%}{%endfor%}</div>