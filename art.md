---
layout: 1
title: art feed
---
## all/basic loop
{%for art in site.art%}
- title: <b>{{art.title}}</b>
- content: {{art.content}}
- category: {{art.categories}}
- tags: {%for tag in art.tags%}#{{tag}} {%endfor%}
{%endfor%}

## specific tags
{%for art in site.art%}{%if art.tags contains "two"%}
- title: <b>{{art.title}}</b>
- content: {{art.content}}
- category: {{art.categories}}
- tags: {%for tag in art.tags%}#{{tag}} {%endfor%}
{%endif%}{%endfor%}