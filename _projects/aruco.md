---
layout: page
title: "ArUco Marker Augmented Reality Project"
description: "An AR system that detects ArUco markers and projects 3D models onto them using OpenCV and Python."
image: /assets/images/projects/aruco/AR.png
permalink: /projects/aruco/
status: done
priority: 300
tags:
  - python
  - computer vision
  - solo project
---

<img src="{{ page.image | relative_url }}" alt="AR projection" class="project-hero">

This project demonstrates an augmented reality system using ArUco markers to estimate camera pose and overlay 3D models on physical markers in video frames. The pipeline involves:
- Detecting ArUco markers using OpenCV.
- Estimating the camera’s position and orientation relative to each marker.
- Loading and preprocessing 3D models (centering, scaling, and rotating them).
- Projecting the models onto the detected markers using cv2.projectPoints, rendering them as wireframes.
- Processing full videos with frame-by-frame projection and bonus features like 3D axis rendering and trail visualization of marker movement.

This project showcases skills in camera calibration, pose estimation, 3D transformations, and video augmentation using Python.