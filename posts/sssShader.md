---
title: Subsurface Scattering Shader
description: Who needs industry standard 3D software suites anyway? 
date: 2021-06-01
tags:
  - Portfolio
  - Unity
  - HLSL
layout: layouts/post.njk
---

<p>Here's an old shader I was working on ages ago. I've since lost the code because I'm bad at saving things, but I managed to dig up two captures. The first video shows the shader having been applied to three busts in a scene. As the light slowly revolves around the statues, you can see how light "flows" through each object. The second video shows off a more practical application of the shader; a lamp shade. A light is turned off and on from inside the shade, and makes the shade "glow". The entire effect is faked using custom-baked, grayscale thinkness maps. The lighter parts of the texture map allow more light to glow through, darker areas dim the effect. Huge shout out to Alan Zucconi for his write ups on various shader techniques.</p>

<p style="text-align: center"></p>
<div class="container">
<p style="text-align: center"><iframe width="800" height="600" src="https://www.youtube.com/embed/BjjJmR12BHA" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen class="video"></iframe></p></div>

<p style="text-align: center"></p>
<div class="container">
<p style="text-align: center"><iframe width="800" height="600" src="https://www.youtube.com/embed/tbisNoHhfew" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen class="video"></iframe></p></div>