---
title: Ramblings on Level Design. 
description: An analysis of my time making levels in video games      . 
date: 2020-12-27
tags:
  - blog
  - Level Design
layout: layouts/post.njk
---
This might be a bit of a long post. It's kind of my "how I got here" story, I guess. 

I think I got my first "look behind the curtain" was with <i>Return to Castle Wolfenstein</i>. I remember when my brother bought the game at a local Walmart. I think it may have been a "Game of the Year" edition or something, because I vaguely remember the box came with a bunch of extras. Most notably, a developer highlight reel (After some quick Googling, I found the reel <a href="https://youtu.be/BC_KoTZbRQA" target="blank">here</a>). I guess that must have been around 2002. So. I was well under the "M 17+" age rating of the game. But yeah, RtCW, great game. 

A couple years later, and a small indie game called <i>Half-Life 2</i> came out in 2004. You've probably never heard of it. Anyway, my brother and I both were looking forward to this one as we were both fans of the first game. Now that I'm writing this, I just remembered that we were gifted the game on Christmas 2004. Was that really 16 years ago? Damn, time flies. Sorry, got sidetracked. So, yeah, Half-Life 2 was great. Played through it a bunch. Hurled toilets at other people in HL2 Deathmatch. Loved it. But then I found the modding scene. And, for better or worse, Garry's mod. 

I think it was playing Garry's Mod that it hit me that a lot of the content was made by other "normal" people just like me. It definitely helped break down this "I could never do that" mindset that I was stuck in. I eventually joined the Facepunch forums, got banned a bunch for bad grammar, but _then_ I started looking around the "mapping" threads. And here, three paragraphs in, was where I downloaded Hammer and take a whack at making my own maps. 

Holy shit, I had no idea what I was doing. But then again, I don't think the majority of the other mappers on the forums did, either. But I trudged on. gm_catacombs, gm_blockfort, gm_zombiesurvivl, rp_varrock. I know I made more maps, but I can't remember for the life of me what I called them. 

<img src="/img/catacombs.jpg">
<img src="/img/zs1.jpg">
<img src="/img/mall.jpg">
<img src="/img/combinemod.jpg">
<img src="/img/blockfort.jpg">


I had a blast making these maps, and I met a bunch of really cool people playing gmod back in the day. But there was a problem with all those levels I made. They had no gameplay (except maybe gm_zombiedurvival, but it wasn't that great). Yeah, each level had a defined location and theme. But there wasn't anything fun or interesting going on inside the levels. Looking back at it, I think the heart of that problem was the platform I was making maps for. A lot of gmod users would simply load up a cool <i>looking</i> map for the scenery, and not the gameplay (if you've ever played Garry's Mod, this will make sense to you. If not, gmod was kind of this aimless, sandbox mod). Because of this, I would focus too early on making my levels look good and interesting, instead of actually fun to play. TL;DR, I focused on how to make a wall instead of where to make a wall. I can elaborate on this a bit, but my mapping hobby eventually fizzed out in the late naughties (with a brief stint in 2011)

Fast forward to 2015. I had since graduated college, got a "real" full-time job, and dropped any kind of game dev as a hobby. And honestly, I was pretty miserable. A friend of mine, Jonathan, introduced me to a local Unity usergroup in town, and with that, my game dev hobby was reawakened. I participated in a bunch of game jams with the group, and quickly learned the basics of Unity. Jonathan eventually brought me onto a team working on a VR beat-em-up called <i>Kung Fu: Shadow Fist</i> (Think <i>Streets of Rage</i>, but in VR). My job was to make levels for the game. And honestly, it was a lot of fun. Just one small problem: I was still terrible at making levels with actual gameplay. The mechanics of KFSF were pretty simple; You could teleport to predetermined locations to navigate through the world, punch with the motion controllers, and use a charged ability called Shadow Strike (This would slow down time and let your punches do extra damage). The vertical slice was pretty awesome, if I do say so myself. But you're here for level design, not features. 

The main problem with <i>Kung Fu's</i> level design was that the vertical slice level was just a series of corridors. Yeah, it may have looked like city streets, but beneath that thin vaneer was, effectively, an increibly linear hallway. The player literally could not progress or explore if they didn't follow a strict sequence of scripted events. And because this was a vertical slice, some events were still a touch buggy. Meaning the player could inadvertantly break something, and then get soft-locked where they stood. Pretty gross.  


<p style="text-align: center">~ An early blockout and critical path of "The Subway Level" featured in <i>Kung Fu: Shadow Fist's vertical slice ~<img src="/img/kfsf.jpg" class="center"></i>
~ A top-down view of the entire vertical slice level ~<img src="/img/kfsf_topdown.png" class="center">
~ A simple vista featuring lighting from police sirens and placeholder art ~
<img src="/img/kfsf_police.gif" class="center">
~ A shot of a city street, featuring one of our <i>oh so</i> punchable NPCs ~
<img src="/img/kfsf_street.png" class="center">
~  "The Subway Level", of course, featured a ride on a subway train. I put together this simple illusion in which the train cars are fixed, but the tunnel moves past the train ~
<iframe width="800" height="600" src="https://www.youtube.com/embed/M-fQaoTNNPk" frameborder="0" allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</p>

In my mind, every single level I've shown you so far have had the same core problem: I focused on environment art too much. Or maybe too early. My concern for the visuals recieved far more attention than the thought, intention, and arrangement of the gameplay space. 