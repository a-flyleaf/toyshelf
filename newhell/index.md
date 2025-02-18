---
layout: 1
title: “new” hell…?

# css ripped from the misc index, with a slight margin adjustment
css: "#gallery{width:auto; margin:.5em 0 0;} #gallery a{width:31%;}"
---
Character concepts I was toying with in 2022. I'd recently made this site when they spawned, so they got a whole folder here---even though in retrospect (writing this in 2025), development didn't get far enough to really warrant that. Oh well!

Main points of note:
- <span id="hollucien">Features a character named <b>Holly</b> and/or <b>Lucien</b>, a sardonic waiter who gets some kind of design change and also has a demon mode. Lives alone in a small apartment with at least one houseplant.</span>
- <span id="judge">There's also a fella who for some reason I remember as being called "the <b>judge</b>." Judge of what, you may ask? Great question! But the job entails keeping an eye on Holly/Lucien. The judge is generally more enthusiastic about this than the one being watched.</span>
- <span id="brother">The judge also has a younger <b>brother</b>. Bro has one of judge's eyes. I don't know how this works, either.</span>

And that's it, that's all I got. The old pages are [still here](oldhell), but consider everything there indefinitely outdated.

## gallery
<div id="gallery">{%for art in site.art%}{%if art.categories contains "newhell"%}<a href="{%include url.html%}{{art.url}}"><img src="{%include url.html%}/assets/img/art/{{art.date|date:"%F"}}-tn.jpg" alt="{{art.title}}"/></a>{%endif%}{%endfor%}</div>