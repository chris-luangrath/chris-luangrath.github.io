---
layout: post
title:  "Senior Game Project - Programming and Design"
summary: "Unreal and Design"
date:   2023-12-03 00:00:00
preview: /assets/y24/preview1-small.png
---

![Picture 1](/assets/y24/preview1.png)

<!-- # Shrineflow -->
Since April 2023, I've been working on BYU's senior game capstone, a year-long project that simulates the operations of actual studios. This game, which has the temp name "Shrineflow", is an asymetrical game of chase between a ninja that hides around the map and collects objectives and a fox sorceress (kitsune) that has to catch the ninja. With the teams of artists, animators, designers, and programmers, we'll work on this project together until April 2024.

- Design and Iteration
- Prototyping
- Networking and GAS
- Abilities
- Menus

## Design and Iteration
From April to about August 2023, we rapidly iterated over the game to make it where it is today. There has been many things that have greatly changed since we started working on it, including character abilities, game objectives, and many other concepts. All of these changes came from extensive playtesting, both internal and external. We're very excited about where the game is right now!

## Prototyping
Prototyping was done in bluprints for quick implementation and iteration. However, after the game was in a good place, we wanted to make a seperate project that wouldn't have all the residual cruft. In the "Stable Build", we're using much better practices, like implementing complex computations in C++ and using Unreal's Gameplay Ability System.

## Networking, and GAS
Shrineflow is a networked game, as it involves 2 clients communicating over a network. In order to ensure that the game functions as intended over a network, we're implementing Unreal's Gameplay Ability System, including Gameplay Tasks and Cues. It makes replication much easier to manage.

## Abilities
Smoke Bomb
- Originally it was just a see through sphere
- Uses client-side operations to set opacity depending on team
- Uses gameplay cues to start Niagara Particle System to deploy smoke while still using invisible collision
Currently Working On:
- Holding the button will activate pose
- Item Socket on hand for smoke bomb

## Menus
Ability Select Menu
- Uses references to player controllers to apply abilities to characters
- Uses data assets to store/display the name/description/icon of abilities

## Custom Movement Component
I didn't initially create it, but I've been working on it and implementing it for the Kitsune. I'm currently working on tuning the Mantle movement option and removing other bugs and whatnot.