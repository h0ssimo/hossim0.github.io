---
layout: post
title: 'Workflow: How To Create Texture Map For Game Hair Cards Using Xgen'
excerpt: In this article, I'm gonna quickly go over my workflow of creating texture
  maps for game hair cards as well as some tips on using Maya's excellent Xgen system.
  I guess it's easier than what you think.
date: 2019-01-29 00:00:00 +0330
tags:
- article
- tutorial
- workflow
- maya
categories:
- tutorial
image: "/images/how_to_create_texture_map_for_game_hair_cards_using_xgen_header.jpg"
image-sm: "/images/how_to_create_texture_map_for_game_hair_cards_using_xgen_header.jpg"
featured: true
showtags: true

---
Game hair has always been an interesting topic to talk about because of all the challenges it produces along the way. Every artist have their own way of handling them. But in general, there are only a few methods in terms of creating the texture sheet. One robust and flexible workflow, is to use Maya's Xgen system. I know, Xgen may seem a bit tricky to understand at first glance, but once you're there, it's really easy to get the most out of it.

I have to say though, since it contains a lot of steps, I can only go over important parts. But, the good news is I share some tricks as well, which may help you troubleshoot your situation.

### The Ultimate Goal

In short, we need to render out an image like the image below:

We need thick hair, to create the silhouette and cover most of the head; thinner hair for adding breakups and tinier shapes, and finally some thin strand groups and flyaways to add more details to the hair.

### Overall Workflow

We're gonna use a simple plane geometry for every hair group to grow from, and then will hide them in the end. Then, go to an orthographic camera, like the front cam, and set the render output resolution to a square size. I'll go with 4K, which means -as you know- 4096*4096. Then assign an appropriate hair shader to my Xgen descriptions, and add some lights. Then we will render from there, to see what we got, and adjust it eventually to get the look we want.

### Important Steps

Before you jump into Xgen, there are several general tips to be aware of:

* 