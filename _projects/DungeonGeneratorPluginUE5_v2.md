---
layout: page
title: "Procedural 3D Dungeon Generator (UE5 plugin)"
description: "An Unreal plugin for generating 3D dungeons using 3D Delaunay tetrahedralization, MSTs, and a custom A* pathfinding algorithm"
image: /assets/images/projects/dungeonGenerator/dungeon3D.png
permalink: /projects/DungeonGeneratorPluginUE5_v2/
status: prototype
priority: 400
tags:
  - plugin
  - UE5
  - c++
  - solo project
---

<img src="{{ page.image | relative_url }}" alt="Dungeon Generator 3D" class="project-hero">

This plugin builds on the ideas of my earlier 2D dungeon generator, expanding it into three dimensions with full vertical connectivity and customizable modular design. Created as a plugin for Unreal Engine, the system allows users to build complex, interconnected dungeon layouts using a graph-based generation system.

The generator supports both horizontal and vertical level construction using pre-made room and hallway assets, with full control over room shapes, doorway positions, and vertical transitions.

Key Features:
1. Custom Room Modules
    - Users can define rooms with arbitrary shapes and specify door locations manually.
2. Modular Hallway Tiles for Vertical Connectivity
    - Vertical movement is handled using custom hallway tiles (e.g. staircases, elevators) that connect specific doors on different levels.
    - Each hallway prefab includes exactly two doors and acts as a “vertical edge” in the graph.
3. Delaunay Tetrahedralization
    - Instead of 2D Delaunay triangulation, the system uses 3D Delaunay tetrahedralization to determine optimal room-to-room connections.
4. Graph + A*
    - A minimum spanning tree is created to ensure connectivity.
    - A custom 3D A* implementation attempts to route valid hallway paths, using hallway tiles as weighted “steps” in the algorithm.
5. Blueprit Node System
    - The system operates through a network of customizable Blueprint nodes, providing users with greater control and flexibility over the dungeon generation process.

This project remains a prototype, as the custom 3D A* algorithm occasionally becomes unstable or gets stuck in edge cases. Despite these issues, the core system laid the foundation for a powerful and flexible dungeon generation tool that I may return to and refine in the future.

## Gallery

<div class="project-gallery">
  <img src="{{ '/assets/images/projects/dungeonGenerator/dungeon3D.png' | relative_url }}" alt="Scene 1">
</div>