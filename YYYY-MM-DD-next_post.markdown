---
layout: post
title:  "This Week in Minetest"
date:   2022-01-22 14:39:05 -0500
categories: jekyll update
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
------------------------------------------------
Minetest 5.5 was released last month, with some significant improvements.

A short overview of today's post

## Engine News <a name="engine"></a>
------------------------------------------------
<sup>Written by MisterE and Rubenwardy</sup>

Minetest 5.5.0 has been released! 

While you may not see many visible changes, there's been a considerable amount of work under the hood to improve the rendering system. Minetest now uses its own fork of the Irrlicht rendering library, which will make further improvement easier. It's already allowed several longstanding bugs to be fixed. 

Be warned: when you update to 5.5, it'll upgrade worlds to a new map encoding. This is irreversible, and will prevent you from running those worlds on older Minetest versions. If you aren't sure about the upgrade, then backup your map beforehand. 

There were some interesting changes to the modding API. Various features have been de-hardcoded, allowing mods and games more control. For example, liquid features have been decoupled from liquid drawtypes (making it easier to make things like spiderwebs). Player fall damage is also changeable using armor groups; you can avoid red flashes from disabled fall damage. 

Possibly the most interesting change to the API was an upgrade to the dynamic media API. Modders and game creators can now send media to individual clients, and label it as "ephemeral", meaning the client will forget it when they disconnect. Previously, dynamic media was sent to all clients, and became part of the media sent to clients on when they joined. With the new version, individualized media is finally possible! The applications are huge, especially regarding background music (BGM), which used to extend login times enormously. BGM can now be sent one track at a time after the player has joined. 

As always, you can check out [the full changelog](https://dev.minetest.net/Changelog#5.4.0_.E2.86.92_5.5.0). Also see the [official announcement](https://forum.minetest.net/viewtopic.php?f=18&t=27754).


## Game News <a name="games"></a>
------------------------------------------------



## Mod News <a name="mods"></a>
------------------------------------------------


New mods and major Mod development updates

## Art and Builds <a name="art"></a>
------------------------------------------------


Amazing builds, Minetest-related art

## Server Spotlight <a name="s-spotlight"></a>
------------------------------------------------


If there is a server that wants to be advertised here, A paragraph and screenshots.
One server per article

## Server News <a name="s-news"></a>
------------------------------------------------


Small news blips for servers in general. Great for announcing new servers, server events, major server updates, etc.

## In Other News <a name="s-news"></a>
------------------------------------------------


Anything else that is news-worthy but doesnt fit in the other categories.

## Continue the Discussion:
------------------------------------------------


<iframe src="https://forum.minetest.net/viewtopic.php?f=3&t=27713" style="width: 100%; height: 400px; border: 0px"></iframe>

