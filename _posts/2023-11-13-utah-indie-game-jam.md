---
layout: post
title:  "Utah Indie Game Jam 2023"
summary: "Unreal"
date:   2023-11-12 00:00:00
preview: /assets/gj23/preview.png

---

![Picture 1](/assets/fullsize.png)
# Aurelius Archibald Astralorn's Traveling Tower

https://hdeck.itch.io/aurelius-archibald-astralorns-traveling-tower

I worked with some friends to compete in the Utah Indie Game Jam 2023 competition. The theme was "parallel worlds", so we made a game about a wizard that travels between parallel worlds with different elements to solve puzzles.

I did general programming, but the biggest thing that I was proud of was making a persistance system. Throughout the game, the wizard was solving puzzles and leaving and returning. 

In order to keep track of this progress, I created a list of enums that represented things that need to be recorded, like puzzles already solved, keys obtained, and "gates" already unlocked. 
I was inspired by this [redit post](https://www.reddit.com/r/unrealengine/comments/6ejnfg/question_in_bp_how_can_i_increment_an_enum_to_its/)
* On game start, creates a map of enum/integer to boolean which stores progress. Objects would get progress by calling a function that returned it's progress, and it would change state accordingly.
