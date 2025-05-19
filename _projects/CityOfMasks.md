---
layout: page
title: "City of Masks — Detective Time Loop Game (UE5)"
description: "A UE5 detective game with time loops, fingerprint analysis, NPC schedules, and a custom clue board system."
image: /assets/images/projects/CityOfMasks/MainMenu.png
permalink: /projects/CityOfMasks/
status: done
priority: 500
tags:
  - game
  - c++
  - UE5
  - team project
---

City of Masks is a narrative-driven third-person detective game developed in Unreal Engine 5 as a semester group project by a team of five. The player takes on the role of a masked detective investigating a bomb threat in a stylized city where everyone wears a mask — but only some masks matter.

To prevent the bombing, the player must uncover the name and fingerprint of the culprit before the day ends. If they fail, the bomb explodes — and the detective is transported back to the start of the day with all their knowledge intact. Through repeated loops, the player pieces together clues by talking to NPCs, collecting evidence, and connecting information in a unique, story-driven environment.

Game World Overview:
- 4 interconnected locations:
    - The Square – where a political rally is held (and the bomb is hidden under the podium)
    - Poor Street – home to a factory and local workers
    - Rich Street – site of a mansion party
    - The Bridge – a quieter area with a riverside diner
- Each scene contains points of interest, unique NPCs with animations, and various interactive objects.
- All characters wear masks; story-relevant NPCs have distinct mask designs, while background characters wear plain ones.
- Noone will speak to the detective untill he finds a mask.

Gameplay & Features:
- Time loop mechanics — restart the day with retained knowledge if the bomb detonates.
- Dynamic NPC behavior — certain NPCs move between scenes based on a day schedule.
- Custom bulletin board inventory — players store collected evidence (fingerprints, photos) and connect clues with lines and sticky notes.
- Interactive object inspection — players can pick up and rotate objects in 3D to search for clues like fingerprints.
- Fingerprint collection system — integrated with object inspection, letting players extract prints and store them.
- Photo acquisition — a photographer NPC provides pictures of other characters or locations when asked.

# My Contributions:
- Lead programmer for the project
- Designed and implemented the entire bulletin board inventory system
- Developed the custom 3D object inspection system for interacting with clue-bearing objects
- Handled all character animations and cutscenes
- Made the time system
- Built the complex branching dialogue system (see separate project)
- Provided support with materials, textures, and model integration across the team

This project combined investigative gameplay, narrative design, system programming, and teamwork, culminating in a technically complex and immersive experience.