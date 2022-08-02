---
layout: 1
title: "art tagged “ava”"
css: "#art{display:none;}"
nav: disaster-crew
permalink: art/ava
---
<div id="gallery">{%for art in site.art%}{%if art.tags contains "ava"%}<a href="{%include url.html%}{{art.url}}"><img src="{%include url.html%}/assets/img/art/{{art.date|date:"%F"}}-tn{%if art.multi%}-ava{%endif%}.jpg" alt="{{art.title}}"/></a>{%endif%}{%endfor%}</div>