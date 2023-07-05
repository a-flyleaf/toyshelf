---
layout: 1-profile
title: “sawface” (and human)
nm: sawface
imgsrc: figure-drawing

info: |-
  A funky monster that spawned some time during or before 2016, plus a human who appears with it sometimes. I have no idea what inspired either, honestly. Any semblance of a character bio is also beyond me, as are names (hence typically writing "sawface" in quotes). But I think they look cool, and That's What Matters™.
---
<div id="gallery">{%for art in site.art%}{%if art.tags contains "sawface"%}<a href="{%include url.html%}{{art.url}}"><img src="{%include url.html%}/assets/img/art/{{art.date|date:"%F"}}-tn{%if art.tags.size>1%}-{{page.nm}}{%endif%}.jpg" alt="{{art.title}}"/></a>{%endif%}{%endfor%}</div>

Not shown: art by other people [courtesy ArtFight](https://a-flyleaf.github.io/artfight/etc/roster#sawface). Go check it out!