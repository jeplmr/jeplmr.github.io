---
title: Ramblings on Level Design, Part 1
description: An analysis of my time doing level design. 
date: 2020-12-27
tags:
  - blog
  - Level Design
layout: layouts/post.njk
---
<p>Buckle up, we're going back to 2002.</p>

<p style="text-indent: 2em">I think I got my first "look behind the curtain" with <i>Return to Castle Wolfenstein</i>. My brother brought home a "Game of the Year" edition of the game, which was really cool because it came with a bunch of extras like desktop wallpapers and such. But the coolest extra was a developer highlight reel. I even managed to dig it up from the depths of YouTube! I must have watched that reel at least a dozen times back in the day. I definitely wasn't old enough for the game's <i>M for Mature</i> rating at the time, so actually seeing the people and the creative process engrossed my young, <i>E for Everyone</i> mind. I had only ever known video games as these weird black boxes that suddenly made your TV interactive. I never stopped to think about how theose black boxes were made. But seeing the developers talk about how the sausage gets made was incredibly cool. I especially love what Rich Farrelly said about the level editor; "It can be pretty intimidating at first with all the lines, entities, verticies... and any other -ies you can think of". Oh, and <i>Return to Castle Wolfenstein</i> is a great game. Go play it!

<p style="text-align: center"><iframe width="800" height="600" src="https://www.youtube.com/embed/BC_KoTZbRQA" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></p>

<p style="text-indent: 2em">A couple years later, and a small indie game called <i>Half-Life 2</i> releases in 2004. You've probably never heard of it. But Half-Life 2 was great. Played through single player a bunch. Hurled toilets at other people in HL2 Deathmatch. Loved it. But then I found the modding scene. And, for better or worse, Garry's mod. And it was playing gmod where I found other "normal" (i.e., kids just like me) people making content for a video game. It definitely helped break down this "I could never do that" mindset I was stuck with. I eventually joined the Facepunch forums, got banned a bunch for bad grammar, but <i>then</i> I started looking around the "mapping" threads. And this is where I downloaded Hammer and take a whack at making my own Garry's Mod maps for the first time. 

<p style="text-indent: 2em">And boy oh boy, were they bad. Plus I had no idea what I was doing (then again, I don't think anyone else on the Facepunch mapping forums did either). But it didn't matter. I had a blast making my awful maps. I also met a bunch of really cool people that I otherwise wouldn't have. I made malls, zombie infested towns, remakes, catacombs. I made whatever my highschool mind could think up. My friends and I even tried tackling a full-sized Half-Life 2 mod about a Civil Protection cop caught in the crossfire of Gordon's misadventures. We never finished the mod, unfortunately. But hey, at least a few scrappy highschool kids scattered across the country were willing to give it the old college try. I even managed to scrounge up some really old, really low resolution screenshots! 

<p style="text-align: center"><i>Some catacombs I was working on.</i><br><img src="/img/catacombs.jpg"><p>
<p style="text-align: center"><i>rp_zombiesurvival, one of my more popular Garry's Mod maps.</i><br><img src="/img/zs1.jpg"></p>
<p style="text-align: center"><i>An unfinished shopping mall. Yes, I was going to fill this with zombies, too.</i><br><img src="/img/mall.jpg"></p>
<p style="text-align: center"><i>A remake of Mario Kart 64's Blockfort</i><br><img src="/img/blockfort.jpg"></p>
<p style="text-align: center"><i>An introductory level of the aforementioned HL2 mod that was never finished.</i><br><img src="/img/combinemod.jpg"></p>

<p><i>~ Let's do the time warp again ~</i></p>

<p style="text-indent: 2em">The year is 2015. Corona was only just a beer. I had since graduated college with a "real" degree and landed a "real" adult nine-to-five job. I had dropped any kind of game dev or level design as a hobby. And I was honestly pretty miserable. A friend of mine, Jonathan Schrack, introduced me to a local Unity usergroup in town. This definitely rekindled that spark. I started showing up to meetups, I learned the basics of the Unity engine, I learned how to script gameplay with C#, and I participated in <i>a lot</i> of game jams. One of my games even won <a href="https://ldjam.com/events/ludum-dare/41/modern-art-critic-hero" target="blank">4th place for Humor</a> in Ludum Dare 41!




participated in a bunch of game jams with the group, and quickly learned the basics of Unity. Jonathan eventually brought me onto a team working on a VR beat-em-up called <i>Kung Fu: Shadow Fist</i> (Think <i>Streets of Rage</i>, but in VR). My job was to make levels for the game. And honestly, it was a lot of fun. Just one small problem: I was still terrible at making levels with actual gameplay. The mechanics of KFSF were pretty simple; You could teleport to predetermined locations to navigate through the world, punch with the motion controllers, and use a charged ability called Shadow Strike (This would slow down time and let your punches do extra damage). The vertical slice was pretty awesome, if I do say so myself. But you're here for level design, not features. 

<p style="text-indent: 2em">The main problem with <i>Kung Fu's</i> level design was that the vertical slice level was just a series of corridors. Yeah, it may have looked like city streets, but beneath that thin vaneer was, effectively, an increibly linear hallway. The player literally could not progress or explore if they didn't follow a strict sequence of scripted events. And because this was a vertical slice, some events were still a touch buggy. Meaning the player could inadvertantly break something, and then get soft-locked where they stood. Pretty gross.  


<p style="text-align: center"><i>An early blockout of "The Subway Level" featured in <i>Kung Fu: Shadow Fist's vertical slice.</i><br><img src="/img/kfsf.jpg" class="center"></i></p>

<p style="text-align: center"><i>A top-down view of the entire vertical slice level.</i><br><img src="/img/kfsf_topdown.png" class="center"></p>

<p style="text-align: center"><i>A simple vista featuring lighting from police sirens and placeholder art.</i><br><img src="/img/kfsf_police.gif" class="center"></p>

<p style="text-align: center"><i>A shot of a city street, featuring one of our <i>oh so</i> punchable NPCs.</i><br><img src="/img/kfsf_street.png" class="center"></p>

<p style="text-align: center"><i>"The Subway Level", of course, featured a ride on a subway train. I put together this simple illusion where the tunnel moves past a fixed train car.</i><br>
<iframe width="800" height="600" src="https://www.youtube.com/embed/M-fQaoTNNPk" frameborder="0" allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></p>

<p style="text-indent: 2em">In my mind, every single level I've shown you so far have had the same core problem: I focused on environment art too much. Or maybe too early. My concern for the visuals recieved far more attention than the thought, intention, and arrangement of the gameplay space. Earlier this year I was fighting with a level I was working on. Really, I was banging my head against a wall. Everything I was trying with the level felt.. off, somehow. When I finally took a break, I grabbed my copy of <i>101 Things I Learned in Architecture School</i> for some pointers (While the book is aimed at Architects, I find it incredibly useful for level design). A page pretty much jumped right out of the book and slapped me right in the face:

<p style="background-color: #000000; font-family: serif">
"<b>Architecture begins with an idea.</b>
Good design solutions are not merely physically interesting but are driven by underlying ideas. An idea is a specific mental structre by which we organize, understand, and give meaning to external experiences and information. Without underlying ideas informing their buildings, architects are merely space planners. Space planning with decoration applied to 'dress it up' is not architecture; architecture resides in the DNA of a building, in an embedded sensibility that infuses its whole."
<br><br>
101 Things I learned in Architecture School<br>Matthew Frederick</p>

<p>And there it was, plain as day. Everything I had been doing wrong since I first picked up Hammer.</p>

<img src="/img/scottpilgrim.gif">

<p><i>To be continued...</i></p>

