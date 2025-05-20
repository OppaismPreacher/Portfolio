---
layout: page
title: "Blender to YOLOv8 Object Detection Pipeline"
description: "A Python pipeline that renders 3D objects in Blender, extracts bounding boxes, augments data, and trains a YOLOv8 model."
image: /assets/images/projects/YOLOv8/legoDetect.png
permalink: /projects/YOLOv8Pipeline/
status: in-progress
priority: 300
tags:
  - computer graphics
  - computer vision
  - python
  - blender
  - solo project
---

<img src="{{ page.image | relative_url }}" alt="Lego Brick Detection" class="project-hero">

This project is a Python-based pipeline that automates the process of generating training data from 3D models rendered in Blender and trains a YOLOv8 object detection model using the resulting synthetic dataset. It eliminates the need for manual annotation by calculating bounding boxes programmatically and supports optional data augmentation.

Workflow Overview:

1. Render 3D object in Blender
    - A Python script loads a 3D model and renders it in front of a clean background.
    - the model gets rotated multiple times to vary the dataset.
2. Segmentation and bounding box extraction
    - A separate script processes the output image, isolates the object from the background, and computes its bounding box.
    - This step uses masking logic to extract position data automatically.
3. (Optional) Background augmentation
    - To improve training quality and robustness, the pipeline can optionally:
        - Add random noise to the background
        - Overlay a real-world image as a background
        - Apply slight variations in object position
4. Train YOLOv8 model
    - The resulting images and annotation files are passed to Ultralytics’ YOLOv8 training system, producing a fully functional object detection model based on the synthetic dataset.

Tools & Skills Used:
- Blender + Python scripting for procedural rendering
- Custom image processing to detect object boundaries
- YOLOv8 (Ultralytics) for modern object detection training
- Optional data augmentation for better generalization

This project demonstrates how to combine 3D rendering, automation, computer vision, and machine learning into an efficient data generation and training pipeline — ideal for scenarios where real-world data is scarce or hard to annotate.

<div class="project-gallery">
  <img src="{{ '/assets/images/projects/YOLOv8/legoDetect.png' | relative_url }}" alt="Scene 1">
  <img src="{{ '/assets/images/projects/YOLOv8/Renders.png' | relative_url }}" alt="Scene 2">
  <img src="{{ '/assets/images/projects/YOLOv8/segmentation.png' | relative_url }}" alt="Scene 3">
  <img src="{{ '/assets/images/projects/YOLOv8/border.png' | relative_url }}" alt="Scene 4">
  <img src="{{ '/assets/images/projects/YOLOv8/noise.png' | relative_url }}" alt="Scene 5">
</div>