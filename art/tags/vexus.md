---
layout: 1
title: "art tagged “vexus”"
css: "#art{display:none;}"
nav: disaster-crew
permalink: art/vexus
---
<div id="gallery">{%for art in site.art%}{%if art.tags contains "vexus"%}<a href="{%include url.html%}{{art.url}}"><img src="{%include url.html%}/assets/img/art/{{art.date|date:"%F"}}-tn{%if art.multi%}-vexus{%endif%}.jpg" alt="{{art.title}}"/></a>{%endif%}{%endfor%}</div>