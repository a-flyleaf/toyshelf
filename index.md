---
layout: 1
title: a-flyleaf’s toyshelf

skip: [roommates,sika,holly,judge]
img:
  - nm: nightpath
    dt: 2021-11-14
  - nm: lucien
    dt: 2023-01-06
---
A [Toyhou.se](https://toyhou.se/) knockoff site, for various characters without established story canons & art featuring them.

<div id="gallery">{%for c in site.data.characters%}{%unless page.skip contains c.name%}<a href="{%include url.html%}/{%if c.group=='cmyk'%}disaster-crew/{{c.name}}{%elsif c.group=='hl'%}newhell{%else%}misc#{{c.name}}{%endif%}"><img src="{%include url.html%}/assets/img/art/{%assign c-first=site.art|where:"tags",c.name|first%}{{c-first.date|date:"%F"}}{%if c.name=='lucien'%}2022-11-21{%endif%}-tn{%if c-first.tags.size>1%}-{{c.name}}{%endif%}.jpg" alt=""></a>{%endunless%}{%endfor%}</div>

- [super nifty About page]({%include url.html%}/about)
- character categories:
	- [disaster crew]({%include url.html%}/disaster-crew)
	- [miscellaneous randos]({%include url.html%}/misc)
	- [new hell]({%include url.html%}/newhell)
- [all the art. <em style="text-transform:uppercase;font-style:normal;">all</em> of it.]({%include url.html%}/art) (image-heavy)

Updates noted on [the changelog](changelog).

<!--convoluted nightmare scraps

{%for c in site.data.characters%}
{{c.name}} {%assign date2=page.img|where:"nm",c.name%} ( {%for d in date2%}{{d.dt}}{%endfor%} )
{%endfor%}




<div id="gallery">{%for c in site.data.characters%}{%unless page.skip contains c.name%}<a href="{%include url.html%}/{%if c.group=='cmyk'%}disaster-crew/{{c.name}}{%elsif c.group=='hl'%}newhell{%else%}misc#{{c.name}}{%endif%}"><img src="{%include url.html%}/assets/img/art/{%assign c-first=site.art|where:"tags",c.name|first%}{%assign c-img=page.img|where:"nm",c.name%}{%capture c-date%}{%for i in c-img%}{{i.dt}}{%endfor%}{{c-first.date|date:"%F"}}{%endcapture%}{%capture c-datestrip%}{%if c-date.size>10%}{{c-date|truncate:10,""}}{%else%}{{c-date}}{%endif%}{%endcapture%}{{c-datestrip}}-tn{%if c-first.tags.size>1%}-{{c.name}}{%endif%}.jpg" alt=""></a>{%endunless%}

{{c-datestrip}}
{{c-datestrip.date|date:"%a"}}
{%assign c-art=site.art|where:"date",c-datestrip%}
{{c-art}}


{%endfor%}</div>

/!--code breakdown (yw):
	- for c in site.data.characters
	- unless page.skip contains c.name
	- a href= disaster-crew/{{c.name}} OR misc#{{c.name}} OR newhell
	- c-first = first art where the character is tagged
	- c-img = array containing the page.img where c.name = data.nm
	- c-date captures BOTH c-img and c-first, in that order
	- c-datestrip = if c-date is long, just grab the second (c-img); else will only pull c-first
--/
-->