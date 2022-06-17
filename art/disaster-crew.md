---
layout: 1
title: "art: disaster crew"
date: 2018-11-26
artsrc: silhouettes
css: "#date,#info{display:none;}"
---
All [art]({%include url.html%}/art) featuring one or more of [the "disaster crew"]({%include url.html%}/disaster-crew).

<div id="gallery">{%for art in site.art%}{%if art.categories contains "disaster-crew"%}<a href="{%include url.html%}/{{art.url}}"><img src="{%include url.html%}/assets/img/art/{{art.date|date:"%F"}}-tn.jpg" alt="{{art.title}}"/></a>{%endif%}{%endfor%}</div>