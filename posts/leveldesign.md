---
title: Ramblings on Level Design, Part 1
description: An analysis of my time doing level design. 
date: 2020-12-29
tags:
  - blog
  - Level Design
layout: layouts/post.njk
---
<p>Buckle up, we're going back to 2002.</p>

<p style="text-indent: 2em">I think I got my first "look behind the curtain" with <i>Return to Castle Wolfenstein</i>. My brother brought home a "Game of the Year" edition of the game, which was really cool because it came with a bunch of extras like desktop wallpapers and such. But the coolest extra was a developer highlight reel, which I've linked below. I must have watched that reel at least a dozen times back in the day. I definitely wasn't old enough for the game's <i>M for Mature</i> rating at the time, so seeing the people and the creative process captured the full attention of my young, <i>E for Everyone</i> mind. I had only ever known video games as these weird black boxes that suddenly made your TV interactive. I never stopped to think about how those black boxes were made. But seeing the developers talk about how they made the magic happen was incredibly fascinating, especially for my 13-ish year old self. I especially love what Rich Farrelly said about the level editor; "It can be pretty intimidating at first with all the lines, entities, verticies... and any other -ies you can think of".

<div class="container">
<p style="text-align: center"><iframe width="800" height="600" src="https://www.youtube.com/embed/BC_KoTZbRQA" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen class="video"></iframe></p></div>

<p style="text-indent: 2em">A couple years later, and a small indie game called <i>Half-Life 2</i> releases in 2004. You've probably never heard of it. But Half-Life 2 was great. Played through single player a bunch. Hurled toilets at other people in HL2 Deathmatch. Loved it. But then I found the modding scene. And, for better or worse, Garry's mod. And it was playing gmod where I found other normal people (i.e., kids just like me) making and sharing content for a video game. It definitely helped break down this "I could never do that" mindset I was stuck with. I eventually joined the Facepunch forums, got banned a bunch for bad grammar, but <i>then</i> I started looking around the "mapping" threads. And this is where I downloaded Hammer and took a whack at making my own Garry's Mod maps for the first time. 

<p style="text-indent: 2em">Boy oh boy, were they bad. Plus I had no idea what I was doing (then again, I don't think anyone else on the Facepunch mapping forums did, either). But it didn't matter. I had a blast making my awful maps. I also met a bunch of really cool people that I otherwise wouldn't have. I made malls, zombie infested towns, remakes, catacombs. I made whatever my highschool brain (and limited free time) could think up. My friends and I even tried tackling a full-sized Half-Life 2 mod about a Civil Protection cop caught in the crossfire of Gordon's misadventures. We never finished the mod, unfortunately. But hey, at least a few scrappy highschool kids scattered across the country were willing to even try a project with that scope. We made a surprising amount of progress before SATs, ACTs, and college prep got in the way. Here are some really low resolution screenshots I managed to scrounge up! 

<p style="text-align: center"><i>Some catacombs I was working on.</i><br><img src="/img/catacombs.jpg"><p>
<p style="text-align: center"><i>rp_zombiesurvival, one of my more popular Garry's Mod maps.</i><br><img src="/img/zs1.jpg"></p>
<p style="text-align: center"><i>An unfinished shopping mall. Yes, I was going to fill this with zombies, too.</i><br><img src="/img/mall.jpg"></p>
<p style="text-align: center"><i>A remake of Mario Kart 64's Blockfort, featuring custom textures.</i><br><img src="/img/blockfort.jpg"></p>
<p style="text-align: center"><i>An introductory level of the aforementioned HL2 mod that was never finished.</i><br><img src="/img/combinemod.jpg"></p>

<p><i>~ Let's do the time warp again ~</i></p>

<p style="text-indent: 2em">The year is 2015. Corona is only just a beer. I had recently graduated college a few years prior with a "real" degree and landed a "real" job doing "real" work. I had also dropped any kind of game dev or level design as a hobby. And I was honestly pretty miserable. A friend of mine, Jonathan Schrack, introduced me to a local Unity usergroup in town. I'm grateful glad he did, because it woke up this long dormant love I used to have for making stuff. I started showing up to the meetups, I learned the basics of the Unity engine, I learned how to script gameplay with C#, and I participated in <i>a lot</i> of game jams. I even learned how to use Blender to make custom models and characters somewhat proficiently. One of my jam games even won <a href="https://ldjam.com/events/ludum-dare/41/modern-art-critic-hero" target="blank">4th place for Humor</a> in Ludum Dare 41!


<p style="text-indent: 2em">One year later, Jonathan brought me onto a small team working on a VR beat-em-up called <i>Kung Fu: Shadow Fist</i>. Think <i>Streets of Rage</i>, but in VR. My job was to design levels for the game (shocking, I know). The mechanics of KFSF were pretty simple; You could teleport to predetermined locations to navigate through the world, throw punches with the motion controllers, and use a charged ability called Shadow Strike, which would slow down time and cause your punches to do extra damage. The vertical slice was pretty great, considering the dev team was a fairly ragtag bunch of three part-time developers.</p>

<p style="text-indent: 2em">Adapting the level design of those classic beat-em-ups ended up being pretty challenging. The levels in those games were linear, usually forcing the player to move left-to-right across the screen. This shifted my focus to creating memorable events instead of creating more elaborate, open designs. For example, "The Subway Level" didn't take place <i>just</i> in a subway. The player started the city streets, beating up gang members until they arrived at a bar. Inside the bar were more thugs. Taking them out rewarded the player with a bathroom gag, in which one lone bonehead would exit the restroom in a, hopefully, amusing display of Vincent-Vega-style bad timing. After the bar, the player would finally make their way to the subway, and board a train. This resulted in a climactic battle between the player and the rival gang, all while the train was en route to its destination.</p>

<p style="text-align: center"><i>An early blockout of "The Subway Level" featured in <i>Kung Fu: Shadow Fist's vertical slice.</i><br><img src="/img/kfsf.jpg" class="center"></i></p>

<p style="text-align: center"><i>A top-down view of the entire vertical slice level.</i><br><img src="/img/kfsf_topdown.png" class="center"></p>

<p style="text-align: center"><i>A simple vista featuring lighting from police sirens and placeholder art.</i><br><img src="/img/kfsf_police.gif" class="center"></p>

<p style="text-align: center"><i>A shot of a city street, featuring an extremely punchable NPC. Now that's a face only a mother could love.</i><br><img src="/img/kfsf_street.png" class="center"></p>

<div class="container">
<p style="text-align: center"><i>"The Subway Level" train ride. I put together this simple illusion where the tunnel moves around an immobile train car.</i><br>
<iframe width="800" height="600" src="https://www.youtube.com/embed/M-fQaoTNNPk" frameborder="0" allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen class="video"></iframe></p></div>

<p style="text-indent: 2em">Making this level for KFSF was really fun. But there was something about the level I just couldn't get into. I never really found an identity for it. A feel. I never got into a flow state while working on it. And I think it shows. While I'm really proud of the various events I put together in the level, the space itself feels very.. uninspired. It's basically a long hallway that extends from the city streets to the end of the train station. There are no branching paths, the player isn't presented with interesting choices, and the gameplay gets repetitive very quickly. Don't get me wrong, I don't think the level was that bad. But it certainly wasn't that good, either. I will say that it was a competent vertical slice demo, and looking back at it, I'm proud as hell at what I helped build.<p>

<p style="text-indent: 2em">Do you ever find yourself reading something and it reaches out and slaps you across the face? Well, I did. I was reading through <i>101 Things I learned in Architecture School</i> at the recommendation of, well, a whole bunch of people. And this page stuck with me:</p>

<p style="background-color: #000000; font-family: serif">
<b>Architecture begins with an idea.</b><br><br>
Good design solutions are not merely physically interesting but are driven by underlying ideas. An idea is a specific mental structre by which we organize, understand, and give meaning to external experiences and information. Without underlying ideas informing their buildings, architects are merely space planners. Space planning with decoration applied to 'dress it up' is not architecture; architecture resides in the DNA of a building, in an embedded sensibility that infuses its whole.
<br><br>
101 Things I learned in Architecture School<br>Matthew Frederick</p>

<p style="text-indent: 2em">This one page managed to sum up a bunch of things I was unknowingly doing wrong. I would too quickly jump into making my levels look like the places I wanted them to be, instead of building gameplay spaces that take advantage of a game's mechanics. I want to say I picked this habit up in my Garry's Mod days. Because that mod was so aimless and sandboxy, there were no gameplay mechanics to undertsand, no goals to reach. Which isn't a bad thing, it's just a nature-of-the-beast thing when it comes to gmod. Because I was always so focused on <i>how</i> I built a wall, I never practiced building focused gameplay spaces; i.e., I never thought about if the wall should even be there in the first place.</p>

<p style="text-align: center"><img src="/img/scottpilgrim.gif"></p>

<p><i>In part 2, I'll talk about what I'm working on currently, and how I've been working to improve my level design skills in the last couple years.</i></p>

<p><i>To be continued...</i></p>