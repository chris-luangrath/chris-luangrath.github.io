---
layout: post
title:  "Senior Game Project - Pipeline"
summary: "Unreal and Python Material Script"
date:   2023-11-13 00:00:00
preview: /assets/postpreview.png
---

<!-- ![Picture 1](/assets/fullsize.png) -->

I worked on the animation department's senior game project in a pipeline role. So far, my biggest contributions have been:
* Setting up Perforce, training others how to use it, and helping troubleshoot.
* Creating a mesh-material generator to assist artists importing their models into Unreal

[Here's a link to my page talking about Perforce](https://chris-luangrath.github.io/2023/04/13/shrineflow-prototype-p4/)

## Material Tool
Most of the modeling team hadn't worked extensively in Unreal, so we needed a way to help them import their models into Unreal with efficient materials, specifically we wanted to use material instances instead of materials.

To do this, I wrote a tool in Unreal's Python API to automatically generate materials and material instances.
For every mesh, the tool:
1. Determines what parent material(s) it needs (a category, like wood, paint, stone, etc.)
2. Create a correlating material instance (if there isn't one already, else it grabs an existing one)
3. Applies textures to correlating parameters to the material instance (after checking each texture to ensure it's not too detailed/big, for reduce game size)

I worked with the Environment Lead to set up a file structure and naming convention to best organize assets (inspired by the UE5 style guide). This will make it easier for artists to transition their work into Unreal as assets optimized for performance.
