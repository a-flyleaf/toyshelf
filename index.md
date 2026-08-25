---
layout: 1
title: a-flyleaf’s toyshelf
---
It's like a [Toyhou.se](https://toyhou.se/) page, but Mine™

<div id="gallery">{%for c in site.data.characters%}<a href="{%include url.html%}/{%if c.group=='cmyk'%}disaster-crew/{{c.name}}{%elsif c.group=='hl'%}newhell{%else%}misc#{{c.name}}{%endif%}"><img src="{%include url.html%}/assets/img/art/{%assign c-first=site.art|where:"tags",c.name|first%}{{c-first.date|date:"%F"}}-tn{%if c-first.tags.size>1%}-{{c.name}}{%endif%}.jpg" alt=""></a>{%endfor%}</div>

- [super nifty About page]({%include url.html%}/about)
- actual character pages:
	- [disaster crew]({%include url.html%}/disaster-crew)
	- [miscellaneous randos]({%include url.html%}/misc)
	- [new hell]({%include url.html%}/newhell)
- [all the art. <em style="text-transform:uppercase;font-style:normal;">all</em> of it.]({%include url.html%}/art) (image-heavy)

Updates noted on [the changelog](changelog).