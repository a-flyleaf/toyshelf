---
layout: 1
title: "art tagged “levi”"
css: "#art{display:none;}"
nav: disaster-crew
permalink: art/levi
---
<div id="gallery">{%for art in site.art%}{%if art.tags contains "levi"%}<a href="{%include url.html%}{{art.url}}"><img src="{%include url.html%}/assets/img/art/{{art.date|date:"%F"}}-tn{%if art.tags.size>1%}-levi{%endif%}.jpg" alt="{{art.title}}"/></a>{%endif%}{%endfor%}</div>