---
layout: page
title: "Quadrics Decimation Plugin for Blender"
description: "A Blender plugin implementing quadric mesh decimation with full control over detail, edge preservation, and topology."
image: /assets/images/projects/decimation/decimationDog.png
permalink: /projects/Decimation/
status: done
priority: 400
tags:
  - plugin
  - blender
  - python
  - computer graphics
  - solo project
---

<img src="{{ page.image | relative_url }}" alt="Decimation Dogs" class="project-hero">

This Blender plugin implements a custom quadratic decimation algorithm to reduce the number of faces in 3D models while preserving their overall shape and detail. It was developed from scratch in Python and offers a set of fine-tuned controls that allow artists to optimize their geometry interactively inside Blender.

Features:
- Decimation factor - Control how much of the original mesh is preserved (0.0–1.0)
- Target face count - Override the decimation factor to aim for a specific poly count
- Error tolerance - Define how much geometric deviation is allowed
- Preserve boundaries & sharp edges - Prevents critical topology loss on model borders or corners
- Custom GUI integrated into Blender’s sidebar

Technical Highlights:
- Implements a full quadric error simplification pipeline
- Uses BMesh to handle geometry operations
- Real-time update of decimated meshes without destroying the original
- Full triangulation and contraction-pair logic with priority queues

This plugin was a deep dive into mesh optimization algorithms, 3D geometry processing, and Blender scripting.

## Video

<div class="project-trailer">
  <video class="gallery-video" controls>
    <source src="{{ '/assets/videos/Decimation/DecimationVideo.mp4' | relative_url }}" type="video/mp4">
    Your browser does not support the video tag.
  </video>
</div>

## Gallery

<div class="project-gallery">
  <img src="{{ '/assets/images/projects/decimation/decimationDog.png' | relative_url }}" alt="Scene 1">
  <img src="{{ '/assets/images/projects/decimation/3D_decimation_pure.png' | relative_url }}" alt="Scene 2">
</div>