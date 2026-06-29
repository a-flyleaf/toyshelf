---
layout: 1-profile
title: Slade Auctor
nm: slade
imgsrc: lineless-yote

info: |-
  A young ’yote made for [’Souls RPG](https://soulsrpg.com/forum/) in 2010, and essentially a self-insert. Like [Nightpath](INC_URL/misc#nightpath), I haven't felt the need to do much with him past the RP he was made for. He gets used a lot more often for random art, though---enough that he now has a separate page.


trivia: |-
  - When I was developing Slade, some character creation guide somewhere suggested finding a voiceclaim. I vaguely remember spending a very long time trawling a site where voice actors uploaded portfolio reels, primarily consisting of voiceovers for commercials and the stray audiobook. Small- or no-name stuff. I cannot for the life of me find this site again, but the voice I landed on for Slade was an even-toned, mild-mannered young guy. Fella who'd hold a door open for you and help old ladies cross the street. A little awkward.
  - Slade's "design" is a simplified rendition of assorted default [northeastern coyote](https://wiki.soulsrpg.com/index.php?n=Resources.NortheasternCoyote) avatars from the forum. I specifically picture him as [this photo](https://www.flickr.com/photos/10574543@N08/2761106350/in/photostream/), although the agouti patches are far from a perfect match.
  - Like any fledgling writer's self-insert, Slade was a storyteller. In a world where off-brand werewolves are the central species, he totally could've been a writer. Opposable thumbs were on the table. Slade never got (not-)werewolf form, though; didn't join the game with one, wasn't played enough to make it happen. He's feral 5ever in my heart.
  - Art and photos of coyotes where coyotes shouldn't be tend to make me think of him. [This painting](https://artbycreeps.tumblr.com/post/769862237053714432/somber-22x28-inches-oil-on-wood-sold), for instance, and [this roof dog](https://bestthingfortoday.tumblr.com/post/115113583299/wild-coyote-on-the-roof-of-a-bar-queens-ny). ...Hm, now that I write that, maybe I should use the concept for my own art....

css: "main li{margin:.5em 0;}"

---
<div id="gallery">{%for art in site.art%}{%if art.tags contains "slade"%}<a href="{%include url.html%}{{art.url}}"><img src="{%include url.html%}/assets/img/art/{{art.date|date:"%F"}}-tn{%if art.tags.size>1%}-{{page.nm}}{%endif%}.jpg" alt="{{art.title}}"/></a>{%endif%}{%endfor%}</div>

Has at least one 2026 art in [that year's gallery](https://a-flyleaf.github.io/art-2026).