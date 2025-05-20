---
layout: page
title: "Cell Shader Plugin for Blender (Toon Shader)"
description: "A Blender plugin for quick creation of stylized cell-shaded materials with outlines using EEVEE and Grease Pencil."
image: /assets/images/projects/CellShaderBlender/toon_couch.png
permalink: /projects/CellShaderBlender/
status: done
priority: 400
tags:
  - python
  - blender
  - plugin
  - computer graphics
  - solo project
---

<img src="{{ page.image | relative_url }}" alt="Cell Shader Couch" class="project-hero">

This plugin enables quick and easy creation of cell-shaded (toon-style) materials in Blender. Designed for EEVEE, it automates the setup of stylized materials and outlines to create a hand-drawn, comic-book-like aesthetic.

Ideal for creating stylized renders, the plugin uses custom node groups and Grease Pencil modifiers to apply shadows and outlines in a fully non-destructive way.

Features:
- Set light and dark colors for shading bands
- Control the number of shading steps for soft or hard style transitions
- Enable and customize outline thickness and color
- Works directly within Blender's sidebar panel
- Uses Grease Pencil + Line Art modifier to generate outlines

Under the Hood:
- Builds node groups dynamically with proper reuse if one already exists
- Adds Grease Pencil strokes automatically for outlines
- Compatible with multiple objects and reusable across scenes

This project was an exploration of shader node manipulation, real-time render stylization, and UI scripting in Blender.

## Video

<div class="project-trailer">
  <video class="gallery-video" controls>
    <source src="{{ '/assets/videos/CellShader/CellshaderVideo.mp4' | relative_url }}" type="video/mp4">
    Your browser does not support the video tag.
  </video>
</div>

## Gallery

<div class="project-gallery">
  <img src="{{ '/assets/images/projects/CellShaderBlender/toon_couch.png' | relative_url }}" alt="Scene 1">
</div>