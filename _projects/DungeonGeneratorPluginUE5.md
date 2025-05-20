---
layout: page
title: "Procedural 2D Dungeon Generator (UE5 plugin)"
description: "An Unreal plugin for generating 2D dungeons using Delaunay triangulation, MSTs, and A* pathfinding."
image: /assets/images/projects/dungeonGenerator/dungeon2D.png
permalink: /projects/DungeonGeneratorPluginUE5/
status: abandoned
priority: 400
tags:
  - plugin
  - UE5
  - c++
  - solo project
---

<img src="{{ page.image | relative_url }}" alt="Dungeon Generator 2D" class="project-hero">

This Unreal Engine plugin generates procedurally built 2D dungeon layouts by placing and connecting rooms using a combination of computational geometry and pathfinding algorithms. Designed for flat (non-elevated) dungeon maps, it creates navigable, non-linear environments suitable for roguelikes or exploration-based games.

The generation process is entirely algorithmic and extensible, allowing for custom control over room density, spacing, and connectivity.

Algorithm Overview:
1. Room Placement 
    - Rooms are randomly placed on a 2D plane with spatial constraints (no overlaps).
2. Delaunay Triangulation
    - The room centers are passed through a Delaunay triangulation to determine optimal potential connections.
3. Graph Construction with Loops
    - A minimum spanning tree (MST) is extracted from the triangulation to ensure all rooms are connected.
    - Some extra edges from the triangulation are randomly preserved to introduce loops for non-linear gameplay.
4. A Pathfinding*
    - For each edge in the final graph, an A* path is calculated to carve corridors through the map grid between rooms.

This project is abandoned, as I’ve moved on to a more advanced version — a fully procedural 3D dungeon generator with elevation, and vertical connectivity.