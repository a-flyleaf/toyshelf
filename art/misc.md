---
layout: 1
title: "art: miscellaneous characters"
date: 2018-11-26
css: "#date,#info{display:none;}"
---
All [art]({%include url.html%}/art) with one of [the miscellaneous characters]({%include url.html%}/misc).

<div id="gallery">{%for art in site.art%}{%if art.categories contains "misc"%}<a href="{{art.url}}"><img src="{%include url.html%}/assets/img/art/{{art.date|date:"%F"}}-tn.jpg" alt="{{art.title}}"/></a>{%endif%}{%endfor%}</div>