---
layout: post
title:  "Shrineflow - Perforce"
summary: "Unreal and Perforce"
date:   2023-04-13 00:00:00
preview: /assets/postpreview.png
---

![Picture 1](/assets/fullsize.png)

Here's some impressive stuff I did:

* Worked with friends also working on senior project
* Theme was parallel worlds, made a game about a wizard that travels between parallel worlds with different elements to solve puzzles
* I did general programming, but the biggest thing that I was proud of was making a persistance system.
* Stored in the game state, I created a list of enums that represented things that need to be recorded, like puzzles already solved, keys obtained, and "gates" already unlocked. This all needed to work with switching between levels.
* Inspired by this [redit post](https://www.reddit.com/r/unrealengine/comments/6ejnfg/question_in_bp_how_can_i_increment_an_enum_to_its/)
* On game start, creates a map of enum/integer to boolean which stores progress. Objects would get progress by calling a function that returned it's progress, and it would change state accordingly.
