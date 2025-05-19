---
layout: page
title: "Toon Dungeon — Procedural OpenGL Dungeon in C++"
description: "A C++/OpenGL procedural dungeon with toon shading, custom physics, dynamic fractals, and multi-mode camera."
image: /assets/images/projects/OpenGL/openGL.png
permalink: /projects/OpenGL/
status: done
tags:
  - game
  - computer graphics
  - c++
---

Toon Dungeon is a procedurally generated 3D dungeon experience built entirely from scratch in C++ using OpenGL. Designed as a tech demo and experimental rendering engine, it features a rich set of systems including procedural generation, custom shaders, and advanced camera controls.

The project features a distinct toon shading style, giving the dungeon a stylized, hand-drawn aesthetic. Everything in the engine — from rendering and physics to interaction and generation — was built manually without the use of external game engines.

Key Features:
- Procedural generation
    - Rooms and object placements are randomly generated.
    - Generation is both structural (room layout) and decorative (object variety)
- Custom collisions
    - Collision detection was implemented from scratch using linear algebra and C++ math libraries.
- Dynamic fractals
    - Fractal objects are placed in the dungeon.
    - The player can interactively change their iteration depth in real time.
- Rotating hypercube
    - A 4D hypercube (tesseract) is rendered and animated.
    - The player can adjust its visualized dimensionality.
- Custom fog shader
    - A volumetric fog effect was implemented directly in GLSL.
- Three camera modes:
    1. First-person view — player walks through the dungeon.
    2. Free-fly camera — unrestricted exploration of the space.
    3. Orthographic top-down view — interact with the character by dragging them in a "god view."
- Curve systems
    - Implemented NURBS-like curves for object paths.
    - Some in-game objects follow these curves dynamically which makes them look like they are walking through the dungeon.