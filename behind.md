---
title: Behind the Scenes
author: Cipher Prime
date: 2015/11/05
description: With any kind of art show, there are so many things that happen behind the curtain. We really wanted to pull that back a little. Here are some general sections of good stuff.
layout: default
order: 4
---

![Large Piece Overview]

### Find out more
With any kind of art show, there are so many things that happen behind the curtain. We really wanted to pull that back a little. Here are some general sections of good stuff.


1. [Selfie Booth Digital Construction Process](#selfie_booth)
2. [Selfie Booth User Testing](#selfie_booth_testing)
3. [Selfie Booth Construction](#selfie_button_constrution)
3. [Selfie Presentation](#selfie_presentation)
4. [Light and Dark Compositions](#light_and_dark)
5. [Sigils and Painting](#sigils)
6. [Original Concept Art](#concept)
7. [Postcard](#postcard)
8. [Light Violins](#violins)

***

<div id="selfie_booth">&nbsp;</div>

# How to Make a Selfie Light Booth

## &#9679; &#9679; &#9679;

1. ![Raw Depth Input]
2. ![Surface Mapping]
3. ![Particle System]


### 01 Raw Depth Input
The Leap Motion uses two infrared (IR) cameras to detect depth. This is what it sees.

### 02 Surface Mapping
A Sobel filter is applied to generated a normal map that will be used to add more detail to the displacement later.

### 03 Particle System
Auditorium Duet's particle system, Rho, uses a dynamically-generated mesh to represent simulated particles as ribbons of light.

## &#9679; &#9679; &#9679;

1. ![Texture and Color]
2. ![Threshold]
3. ![Depth Displacement]


### 04 Texture and Color Correction
Combining the last three passes yields this result.

### 05 Threshold
With a basic threshold, we can remove objects that are too far from the camera.

### 06 Depth Displacement
Using the depth image and the normal map, we distort the particle system to flow across the subject in three dimensions.

## &#9679; &#9679; &#9679;



1. ![Camera Bloom]
2. ![Depth Masking]
3. ![Final]


### 07 Camera Bloom
Using [Sonic Ether's bloom tech][Sonic Ether], we generate light from the particles, simulating the interactions that take place in a real camera lens.

### 08 Depth Masking
Now, with our virtual camera, we detect distance and use that generate a new depth mask.

### 09 Depth of Field
Finally, we apply a Depth of Field effect, simulating the focal depth of a real camera. This is the final result.

## &#9679; &#9679; &#9679;

<p>
<iframe src="//player.vimeo.com/video/143423100?autoplay=1&loop=1" width="400" height="600" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
</p>

## 10 Put it Together in Real Time
All of this is done in real time, yielding an effect unlike anything you've ever seen.

## &#9679; &#9679; &#9679;

![Selfie Booth in Unity3d]

2. ![Selfie Booth Screenshot Test]
3. ![Selfie Booth Print Test]

# Software and Print Testing
We created the Selife Light Booth using a popular game engine we're familiar with called *Unity3d*. The beams of light were originally created for *Auditorium Duet*, the sequel to our very first game *Auditorium*.

One of our biggest concerns in this whole process was having beauitful, fast, and affordable prints. After quite a few printer tests, we settled on using the *Canon Selphy*. Here is our very first print test on this printer. [Above Right]

## &#9679; &#9679; &#9679;

<div id="selfie_booth_testing">&nbsp;</div>

![Selfie Booth User Test]

# User Testing
We spent quite a while talking about what the process of printing would look like. What kind of experience did we want someone to have when they walked up and played with the booth? How many photos could they take? Ultimately, we decided to use an iPad app software called *Livebooth* to handle these needs. After some extensive testing, we were able to get the process down flawlessly.

## &#9679; &#9679; &#9679;

![Selfie Booth Electronic]

# Hardware
We used *Arduino* to interface with our Light Selfie Booth Application. We used a glowing white button to take your selfie with two knobs used to control hue and saturation. We have a lot of fun variables to play with, but ultimatly went with this simple interface. It might be cool to add controls for things like particle turbulence in the future.

## &#9679; &#9679; &#9679;

<div id="selfie_booth_construction">&nbsp;</div>

1. ![Selfie Booth Construction]
2. ![Selfie Booth Without Top]

# Booth Construction
It's sort of ridiculous how hard it was to find a cheap white presentation platform. Searching online yielded few affordable options, so we opted to create our own. The entire process of creating the booth took around three days. (We even created our own tools, building a square from scrap timber we had laying around.)

## &#9679; &#9679; &#9679;

<div id="selfie_presentation">&nbsp;</div>

1. ![Sigil Rubber Block]
2. ![Stamped Wax Paper Sleeves]

# Selfie Sleeves
Art is all about the experience, so we created Wax Paper Sleeves by carving the Auditorium Duet Logo into a Rubber Block and hand-stamping them. This was a very lengthly process, but yielded a simple, elegant result.

***

<div id="light_and_dark">&nbsp;</div>

![Light and Dark Compositions]

# Showing Duality Between the Past and the Future
From the moment we had accepted the challenge of creating this show, we knew we wanted to offer at least three scales of pieces. But more importantly, we also knew we wanted the medium and large pieces to mirror each other. A lot of care and craftsmanship went into making sure we could portay both worlds with the exact same content.

***

<div id="concept">&nbsp;</div>

![Original Concept Art]

# Original Concept Art
The world of Auditorium is quite flat. At some point, we decided to use the background of the game as a horizon line to create unique compositions. With the thought of creating a brand new renderer firmly in mind, this was the final concept design that we created before developing this new rendering technique.

***

<div id="sigils">&nbsp;</div>

1. ![Sigil Sketches]
2. ![Typtic Painting in Progress]

# Sigils and Painting
Each large piece was printed with archival ink then hand-embellished with their respective sigils. These sigils represent the mood and spirit of each world these game elements are encountered in *Auditorium Duet*. Here you can see Sean Martorana from Indy Hall Arts taking a look at our tryptic during its initial painting process.

***

<div id="postcard">&nbsp;</div>

1. ![First Draft Postcard]
2. ![Print Ready Postcard]

# PostCard
This was our very first art show! Of course we made some baller postcards to both celebrate and promote. Our initial concept used the game title *Auditorium Duet* before we had completely finalized the show name, *We've Traveled So Far*.

***

<div id="violins">&nbsp;</div>

![Light Violin]

# Light Violins
Not everything we tried made it into the show. Here is a prototype of the Light Violins we were going to use for the window display.




[Raw Depth Input]:  /img/behind_the_scenes/booth_process/01%20Raw%20Depth%20Input%20-%20scaled.png
[Surface Mapping]: /img/behind_the_scenes/booth_process/02%20Surface%20Mapping%20-%20scaled.png
[Particle System]: /img/behind_the_scenes/booth_process/03%20Particle%20System.png
[Texture and Color]: /img/behind_the_scenes/booth_process/04%20Texture%20and%20Color.png
[Threshold]: /img/behind_the_scenes/booth_process/05%20Threshold.png
[Depth Displacement]: /img/behind_the_scenes/booth_process/06%20Depth%20Displacement.png
[Camera Bloom]: /img/behind_the_scenes/booth_process/07%20Camera%20Bloom.png
[Depth Masking]: /img/behind_the_scenes/booth_process/08%20Depth%20Masking.png
[Final]: /img/behind_the_scenes/booth_process/10%20Final.png


[Leap Motion]: http://www.leapmotion.com/
[Sonic Ether]: https://www.assetstore.unity3d.com/en/#!/content/17324



[Image 1]: /img/behind_the_scenes/city%20paper%20october%205th%202015.jpg

[Light and Dark Compositions]: /img/behind_the_scenes/duality.jpg

[Original Concept Art]: /img/behind_the_scenes/duet_concept_art.jpg

[First Draft Postcard]: /img/behind_the_scenes/postcard_first_draft.jpg
[Print Ready Postcard]: /img/behind_the_scenes/postcard_front_printready.png

[Sigil Sketches]: /img/behind_the_scenes/sigil_sketches.jpg
[Typtic Painting in Progress]: /img/behind_the_scenes/typtic_painting_progress.jpg

[Selfie Booth Electronic]: /img/behind_the_scenes/selfie_booth_electronics.jpg
[Selfie Booth Construction]: /img/behind_the_scenes/selfie_booth_contruction.jpg
[Selfie Booth Without Top]: /img/behind_the_scenes/selfie_booth_raw.jpg

[Sigil Rubber Block]: /img/behind_the_scenes/sigil_rubber_block.jpg
[Stamped Wax Paper Sleeves]: /img/behind_the_scenes/stamped_wax_paper_sleeves.jpg

[Selfie Booth Screenshot Test]: /img/behind_the_scenes/selfie_booth_unity3d.jpg
[Selfie Booth Print Test]: /img/behind_the_scenes/selfie_booth_first_print.jpg
[Selfie Booth in Unity3d]: /img/behind_the_scenes/selfie_booth_unity3d.png

[Selfie Booth User Test]: /img/behind_the_scenes/selfie_booth_user_test.jpg

[Large Piece Overview]: /img/large/overview_pieces_ground.jpg

[Light Violin]: /img/behind_the_scenes/violins/light_violin.jpg
