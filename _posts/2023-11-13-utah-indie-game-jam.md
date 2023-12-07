---
layout: post
title:  "Utah Indie Game Jam 2023"
summary: "Unreal"
date:   2023-11-12 00:00:00
preview: /assets/gj23/preview.png

---
# Aurelius Archibald Astralorn's Traveling Tower
[Link to Itch.io page with video](https://hdeck.itch.io/aurelius-archibald-astralorns-traveling-tower)


[![Video](https://res.cloudinary.com/marcomontalbano/image/upload/v1701933084/video_to_markdown/images/vimeo--883782837-c05b58ac6eb4c4700831b2b3070cd403.jpg)](https://vimeo.com/883782837 "Video")

I worked with some friends to compete in the Utah Indie Game Jam 2023 competition. The theme was "parallel worlds", so we made a game about a wizard that travels between parallel worlds with different elements to solve puzzles.

I did general programming, but the biggest thing that I was proud of was making a persistance system. Throughout the game, the wizard was solving puzzles and leaving and returning. 

In order to keep track of this progress, I created a list of enums that represented things that need to be recorded, like puzzles already solved, keys obtained, and "gates" already unlocked. 
![Picture 2](/assets/gj23/enum.png)

Since enums map directly to integers, I could use a map of integers to booleans to easily record and retrieve the progress of specific puzzles.
![Picture 3](/assets/gj23/make-map.png)

Since I used enums, it made implementing it in other objects super easy!
![Picture 4](/assets/gj23/check-progress.png)

I had no idea how to do this before working on the game, but I really like this system and hope to use it again in some other project.

Also, we named the game "Aurelius Archibald Astralorn's Traveling Tower" because we wanted the announcer to say the full name when we won. We ended up winning "Best Visuals"!
