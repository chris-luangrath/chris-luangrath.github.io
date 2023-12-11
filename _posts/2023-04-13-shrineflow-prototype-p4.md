---
layout: post
title:  "Senior Game Project - Perforce"
summary: "Unreal and Perforce"
date:   2023-04-13 00:00:00
preview: /assets/perforce.png
---

<!-- ![Picture 1](/assets/perforce.png) -->
BYU has been making games since 2017, but they didn't start using Perforce until 2023. The senior project games are made in Unreal Engine, and switching to Perforce has made the workflow so much better. In previous years, they used TortoiseSVN and GitLFS, which they also used for their senior film projects, but there were many complications that slowed work, like people accidentally overwriting other people's work. Luckily, Perforce helped with that!

## Installing/Setting Up Perfoce
Before work was started on the project, I installed the Perforce server and fiddled around, though not a lot was making sense. Though, it wasn't until I met up with a Perforce representative at GDC23, who gave me super helpful tips and advice, that I had a better understanding of how to best use it.

## Training 30 Students
To help people to start using this new software, I did several trainings/demonstrations in class and made a quick-start guide for their reference. Work on the game started in April, with about 10 people, but I later had to train an even bigger group of 30 people come fall.

## Setup Scripts
Also, using Perfoce on lab computers is a little awkward because the credentials of the previous person working on a computer would linger, which would complicate things greatly. To make this easier for everyone, I wrote some scripts that would set and fill out a user's p4config file, which avoided this problem.


Also, I think it's funny that everyone calls it Perforce, but Perforce is the name of the company! The software is called Helix Core!