---
layout: page
title: "VR Fractal Viewer (Unreal Engine 5 + Blender)"
description: "A VR fractal viewer combining Blender geometry nodes with interactive scanning in UE5."
image: /assets/images/projects/FractalVR/Mandelbrot.png
permalink: /projects/FractalsVR/
status: done
priority: 500
tags:
  - blender
  - UE5
  - computer graphics
  - solo project
---

<img src="{{ page.image | relative_url }}" alt="Fractal" class="project-hero">

This project is a virtual reality exploration experience built in Unreal Engine 5, designed as an interactive fractal viewer. It allows the player to walk through a virtual space and interact with procedurally generated 3D fractals created in Blender using Geometry Nodes.

The VR scene takes place in a simple, darkened room, where the player can:
- Move freely around the space using VR locomotion
- Toggle the environment lighting using a physical button in the center of the room
- Pick up small "toy" fractals (low-iteration versions of the 3D fractals) from a table using their virtual hands
- Place the toy fractals into a scanner, which detects the specific model and displays a high-iteration version of that fractal in the main viewing area

The project includes four unique fractal forms, each modeled procedurally in Blender, then imported and optimized for use in UE5. The scanner logic was built to recognize each fractal and trigger the correct full-detail model dynamically.

This project gave me hands-on experience combining:
- Procedural modeling in Blender (Geometry Nodes)
- VR interactions and hand tracking in UE5
- Object detection and event-based behavior in a 3D environment
- Import/export workflows between Blender and Unreal

It serves more as an interactive tech art installation than a traditional game, and was a great exercise in combining creative procedural visuals with immersive VR controls.

## Gallery

### Fractal Cannopy
<div class="project-gallery">
  <img src="{{ '/assets/images/projects/FractalVR/Canopy.png' | relative_url }}" alt="Scene 1">
  <img src="{{ '/assets/images/projects/FractalVR/Tree_GN_Group.png' | relative_url }}" alt="Scene 2">
  <img src="{{ '/assets/images/projects/FractalVR/Tree_GN.png' | relative_url }}" alt="Scene 3">
</div>

### 3D Snow Flake
<div class="project-gallery">
  <img src="{{ '/assets/images/projects/FractalVR/SnowFlake.png' | relative_url }}" alt="Scene 4">
  <img src="{{ '/assets/images/projects/FractalVR/Snowflake_GN.png' | relative_url }}" alt="Scene 5">
</div>

### Menger sponge
<div class="project-gallery">
  <img src="{{ '/assets/images/projects/FractalVR/Sponge.png' | relative_url }}" alt="Scene 6">
  <img src="{{ '/assets/images/projects/FractalVR/Sponge_GN_Group.png' | relative_url }}" alt="Scene 7">
  <img src="{{ '/assets/images/projects/FractalVR/Sponge_GN.png' | relative_url }}" alt="Scene 8">
</div>

### Mandelbrot set 3D
<div class="project-gallery">
  <img src="{{ '/assets/images/projects/FractalVR/Mandelbrot.png' | relative_url }}" alt="Scene 9">
  <img src="{{ '/assets/images/projects/FractalVR/MB_GN_Group.png' | relative_url }}" alt="Scene 10">
  <img src="{{ '/assets/images/projects/FractalVR/MB_GN.png' | relative_url }}" alt="Scene 11">
</div>
