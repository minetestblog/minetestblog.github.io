---
layout: post
title:  "This Month in Minetest 02"
description: >
  Mapgen Work, Main Menu Redesign
hero: /assets/img/default_hero.png
overlay: White
published: true
---

# Table of contents
*  [Briefing](#overview)
*  [Engine](#engine)
*  [Games](#games)
*  [Mods](#mods)
*  [Art/Builds](#art)
*  [Server Spotlight](#s-spotlight)
*  [Server News](#s-news)
*  [In Other News](#o-news)


## Briefing <a name="overview"></a>


A short overview of today's post

## Engine News <a name="engine"></a>

Where is minetest lacking? You might be able to think of a few areas, but a big one is the available mapgens. Yes, we have stuff that is as good as minecraft's built-in maps: small scale mountians, repetative landscapes. This is clearly an issue...

Jordach is making a more realistic C++ mapgen. Imagine: Deep, wide oceans span the map, making it possible to get lost at sea. Small islands dot the expanse. Oceanic trenches yawn in the depths below. Sheer cliff faces poke out of the sea, marking the boundary, while long beaches snake around the remaining coastline. On the continents, crags kilometers high scrape the clouds, and the wide, low-lying plains are lightly crinkled by rolling hills, providing excellent building space. 

In order to accomplish this, he made a model of the entire map in blender, using the sampled noise sources encoded into pngs. He was then able to mix the noise sources in blender, designing them to produce the large-scale landscape in real-time. The mixing code was translated from blender to lua, and from lua to C++.

The [mapgen](https://github.com/Jordach/minetest/tree/mg_reverb) is WIP, and will continue development until its ready for an engine PR. 



![Jordachs Mapgen](/assets/img/jordach_mapgen.png?raw=true "Jordachs Mapgen")

Another area that we can all agree needs improvement is minetest's main menu. Zughy and Giova are working on a detailed design for the menu. While they are not actually implementing it (just doing the planning and asset work), there are rumors that someone else is working on actual implementation. Stay tuned, this could go somewhere nice.

Paradust is trying to port minetest to run in a browser. The demo works, though there are many bugs. Try seed 2222.
https://minetest.dustlabs.io/


![Minetest in Browser](/assets/img/minetest_in_browser.png?raw=true "Minetest in Browser")

Minetest 5.6 development is underway. After re-enabling dynamic shadows x2048 has been improving the api. Shadows are now [rendered on entities](https://github.com/minetest/minetest/pull/11747), and and [api has been added](https://github.com/minetest/minetest/pull/11944) to allow games to control shadow intensity.


## Game News <a name="games"></a>

Early this month, AiTechEye added added a new realm to XAenvironment. It contains macroscopic fauna and flora. You can use the game's unique parkour system to explore among the towering grass and mushrooms, while avoiding being eaten by giant bugs.

<iframe width="853" height="480" src="https://www.youtube.com/embed/ZqjNQ8NcXw0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


In Colorhop, there's a new end-game building that allows for mass-production of complex structures. It takes much study to figure out, and even more to master. There's no release date yet, but "soon".

![Two Labs](/assets/img/two_labs.png?raw=true "Two Labs")

Mantar is preparing for an Exile release which will add a dye system.

## Mod News <a name="mods"></a>

Apercy has made an official release of his [Ju52 airplane](https://content.minetest.net/packages/apercy/ju52/). Also, many of his vehicles now have inventories.

![Ju52](/assets/img/ju52.png?raw=true "Ju52"). 


Elceejo is experimenting with new ways to use his Creatura Api. The latest product is Spiradilus, a new Boss. It is heavily based on [SCP-682](https://scp-wiki.wikidot.com/scp-682). You can expect a public release in early April.
<iframe width="853" height="480" src="https://www.youtube.com/embed/fkrxO_gAJGg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


Wsor has been quietly working on mods in the [mt-mods](https://github.com/mt-mods) repo, making them game-agnostic. A few recently changes are unified_dyes, basic_materials, steel, and pipeworks. That means that other mods that only depend on those can now also be game agnostic.




## Art and Builds <a name="art"></a>

![Atlas](/assets/img/atlas.png?raw=true "Atlas")
Atlas by GreenXenith

![AI Map](/assets/img/ai_map.png?raw=true "AI Map")
Lemente made this with imaging and an AI-generated picture


![MSS_Faraday](/assets/img/MSS_Faraday.png?raw=true "MSS_Faraday")
"MSS Faraday: Boldly going above Y = 20000", by BuckarooBanzai
You can get the schematic [here](https://blockexchange.minetest.land/api/static/schema/BuckarooBanzai/mss_faraday).


## Server Spotlight <a name="s-spotlight"></a>


If there is a server that wants to be advertised here, A paragraph and screenshots.
One server per article

## Server News <a name="s-news"></a>


Small news blips for servers in general. Great for announcing new servers, server events, major server updates, etc.

## In Other News <a name="s-news"></a>


Anything else that is news-worthy but doesnt fit in the other categories.
