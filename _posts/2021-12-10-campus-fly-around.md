---
layout: post
title:  "Fly Around BYU's Campus in Unreal!"
summary: "Unreal - Programming"
date:   2021-12-10 00:00:00
preview: /assets/byu-model.png
---

![Picture 1](/assets/byu-model.png)

In 2020, a BYU grad student, Bryce E. Berrett, flew drones all over BYU's campus to [create a 3d photogrammetric model.](https://magazine.byu.edu/article/3d-byu-campus-tour/)

Then, in 2021, me and my coworker were tasked with making an interactive experience where people could view the model. We worked together to create "Fly Around BYU" in Unreal 5! 

Footron, the interactive display (we made this the year before) cycles through sever

My one of my biggest contributions to the project was 

Flying around the BYU model was easy enough, but the experience also needed to accommodate both active and passive interaction. To solve this, I implemented the auto-play track and designing/implementing the target/trigger system.

If no input has been given, the camera will travel along a spline track. This solved movement, but we needed the camera to focus on key landmarks, like specific buildings or the clock tower, and we needed to be able to switch between different targets and the the track. The solution ended up being relatively simple:

- View Targets: Placed around the world to give the camera something to focus on.
- Triggers: Placed along the track. When the camera/drone overlaps with the trigger, the trigger gives the camera data, specifically the travel speed and the new view target.
- When the camera recieves a new view target, it stores the previous view target and lerps between the two to smoothly transition to the next target.

If the use starts using the controller, the auto play stops and the user is free to fly around. If there's 30 seconds of inactivity, it returns to the track.

Fly Around BYU is available to the public in the lobby of the James E. Talmage building at Brigham Young University.