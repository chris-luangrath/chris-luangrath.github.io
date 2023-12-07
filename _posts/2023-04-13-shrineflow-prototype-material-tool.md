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
We needed a way to help artists to import their models into Unreal with efficient materials. To do this, we needed to implement materials and material instances. 

* Worked together with Environments to make a tool that helps artists import meshes into Unreal with good materials
* It checks the meshes in a folder, either creates a correlating parent material or finds it, then either creates a correlating material instance more finds it, then adds correlating textures. 
* Worked with environment to set up a file structure and naming convention to organize assets.
