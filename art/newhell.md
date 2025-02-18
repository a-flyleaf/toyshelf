---
layout: 1
title: "art: “new hell”"
css: "#art{display:none;}"
# nav: newhell
---
All [art]({%include url.html%}/art) featuring one or more of [the "new hell" characters]({%include url.html%}/newhell).

<div id="gallery">{%for art in site.art%}{%if art.categories contains "newhell"%}<a href="{%include url.html%}{{art.url}}"><img src="{%include url.html%}/assets/img/art/{{art.date|date:"%F"}}-tn.jpg" alt="{{art.title}}"/></a>{%endif%}{%endfor%}</div>