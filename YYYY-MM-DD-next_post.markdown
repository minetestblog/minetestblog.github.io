---
layout: post
title:  "This Month in Minetest 02"
description: >
  Mapgen Work, Main Menu Redesign
hero: /assets/img/Sunrays.png
overlay: White
published: true
---

# Table of contents
*  [Briefing](#overview)
*  [Engine](#engine)
*  [Games](#games)
*  [Mods](#mods)
*  [Art/Builds](#art)
*  [In Other News](#o-news)


## Briefing <a name="overview"></a>

This month, there is big news regarding engine-related side projects. Shadows receive an update, and a couple games get major new features. Last, but not least, the blog is becoming official!

## Engine News <a name="engine"></a>

Where is Minetest lacking? You might be able to think of a few areas, but a big one is the available mapgens. Sure, we have stuff that is as good as Minecraft's built-in maps: small scale mountains, repetitive landscapes. This is clearly an issue...

Jordach is making a more realistic C++ mapgen. Imagine deep, wide oceans spanning the map; getting lost at sea is a real danger. Small islands dot the expanse. Oceanic trenches yawn in the depths below. Long beaches snake the coastline. On the continents, crags kilometers high scrape the clouds, and the wide, low-lying plains are lightly crinkled by rolling hills, providing excellent building area. 

In order to accomplish this, Jordach made a model of the entire map in blender, using the sampled noise sources encoded into images. He was then able to mix the noise sources in blender, designing them to produce the large-scale landscape in real-time. The mixing code was translated from blender to lua, and from lua to C++.

The [mapgen](https://github.com/Jordach/minetest/tree/mg_reverb) is WIP, and will continue development until its ready for an engine PR. 



![Jordachs Mapgen](/assets/img/jordach_mapgen.png?raw=true "Jordachs Mapgen")

Another area that we can agree needs improvement is Minetest's main menu. Zughy and Giova are working on a detailed design for the menu. While they are not actually implementing it (just doing the planning and asset work); there are rumors that someone else is working on actual implementation. Stay tuned, this could go somewhere nice.

![Menu](/assets/img/menu_concept.png?raw=true "Menu")

Concept art for the main menu redesign singleplayer new-game interface.


Paradust is trying to port minetest to run in a browser. The demo is playable (YMMV), though there are many bugs. Try seed 2222.
https://minetest.dustlabs.io/

![Minetest in Browser](/assets/img/minetest_in_browser.png?raw=true "Minetest in Browser")

Minetest 5.6 development is underway. After the team re-enabled dynamic shadows, x2048 began improving them. Shadows are now [rendered on entities](https://github.com/minetest/minetest/pull/11747), and and [api has been added](https://github.com/minetest/minetest/pull/11944) to allow games to control shadow intensity.



## Game News <a name="games"></a>

Earlier this month, AiTechEye added added a new realm to XAenvironment. It contains macroscopic fauna and flora. You can use the game's unique parkour system to explore among the towering grass and mushrooms, while avoiding being eaten by giant bugs.

<iframe width="853" height="480" src="https://www.youtube.com/embed/ZqjNQ8NcXw0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


In ColourHop, there's a new end-game building that allows for mass-production of complex structures. It takes much study to figure out, and even more to master. There's no official release yet, but its "coming soon".

![Two Labs](/assets/img/two_labs.png?raw=true "Two Labs")


Mantar is preparing for an Exile release which will add a dye system.

## Mod News <a name="mods"></a>

Apercy has made an official release of his [Ju52 airplane](https://content.minetest.net/packages/apercy/ju52/). Also, many of his vehicles now have inventories.

![Ju52](/assets/img/ju52.png?raw=true "Ju52")


Elceejo is experimenting with new ways to use his Creatura Api. The latest product is Spiradilus, a new Boss. It is heavily based on [SCP-682](https://scp-wiki.wikidot.com/scp-682). You can expect a public release in early April.


<iframe width="853" height="480" src="https://www.youtube.com/embed/fkrxO_gAJGg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


Wsor has been quietly working on mods in the [mt-mods](https://github.com/mt-mods) repo, making them game-agnostic. A few recently updated mods are: unified_dyes, basic_materials, steel, and pipeworks. That means that other mods that only depend on those can now be game agnostic as well.


BuckarooBanzai has developed a mod and server software called BlockExchange. It allows you to share and use your builds (schematics) across different worlds. (think: Thingiverse for Minetest builds)
You can browse available builds [here](https://blockexchange.minetest.land/), and with the mod installed on singleplayer or on a server, you can download and place builds, or upload new builds.

![Block Exchange](/assets/img/blockexchange.png?raw=true "Block Exchange")

## Art and Builds <a name="art"></a>

![Atlas](/assets/img/atlas.png?raw=true "Atlas")

Atlas by GreenXenith

![AI Map](/assets/img/ai_map.png?raw=true "AI Map")

Lemente made this with imaging and an AI-generated picture


![MSS_Faraday](/assets/img/MSS_Faraday.png?raw=true "MSS_Faraday")

"MSS Faraday: Boldly going above Y = 20000", by BuckarooBanzai
You can get the schematic [here](https://blockexchange.minetest.land/api/static/schema/BuckarooBanzai/mss_faraday).

## In Other News <a name="s-news"></a>

The Minetest blog is going to be made official! Plans are being worked on to move the blog repository to the Minetest github account and possibly embed the latest posts on the Minetest Website. Stay tuned for changes.
