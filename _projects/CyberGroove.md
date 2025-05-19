---
layout: page
title: "CyberGroove — Python Rhythm Game"
description: "A Python rhythm game inspired by games like Muse Dash or Piano Tiles."
image: /assets/images/projects/CyberGroove/MainMenu.png
permalink: /projects/CyberGroove/
---

CyberGroove is a rhythm-based game developed in Python using the Pyglet library, created as a semester project. Originally inspired by games like Muse Dash and Piano Tiles, the game evolved into a simplified yet engaging system due to the limitations of working with 2D animations and Python at the time.

The game challenges players to hit notes moving from right to left across three lanes, timing their inputs precisely as the notes cross a white line. Scoring is based on timing accuracy, and missing notes results in point loss or life deduction. Players start with 3 lives, which can regenerate based on performance.

To increase difficulty and variety, the game introduces "errors" — special notes that cause an instant game over if not blocked. Players can activate a shield mechanic to destroy errors, but must be careful as the shield also destroys regular notes, affecting their score.

Key Features:
- 3 unique levels with different music tracks and difficulties
- High score tracking for each level
- Health and regeneration system
- Shield mechanic for error handling
- Custom AI-generated background art
- Practice mode to help players learn the rhythm without penalty
- Dynamic performance graph at the end of a level (via Matplotlib)
- Simple level file format that supports parsing from text files

While the code has some rough edges and most features are hardcoded, CyberGroove was a valuable experience in game logic, audio syncing, event-driven programming, and user interaction in Python. A future version would benefit from a level editor and a scalable song system.