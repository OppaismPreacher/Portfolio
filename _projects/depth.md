---
layout: page
title: "Body Measurement and BMI Estimation Using Depth Camera"
description: "Used a depth camera and skeleton data to estimate height, limb size, weight, and BMI using OpenCV and Python."
image: /assets/images/projects/depth/depth.png
permalink: /projects/depth/
status: done
priority: 300
tags:
  - python
  - computer vision
  - solo project
---
<img src="{{ page.image | relative_url }}" alt="Depth Camera Segmentation" class="project-hero">

This project focused on extracting human body measurements from a depth map and skeleton metadata captured with a Kinect depth camera. The goal was to estimate the subject’s height, limb dimensions, body mass, and BMI using computer vision techniques and a predefined body model.

Key Steps:
1. Data Acquisition
  - Loaded a 16-bit depth image and associated metadata (skeleton keypoints and scaling constant k in cm/pixel).
2. Skeleton Visualization
  - Displayed 20 keypoints of the detected skeleton and connected them with lines to form a simplified body structure.
3. Height Estimation
  - Estimated total height using the skeleton points for head and feet, adjusted using anthropometric proportions.
4. Body Segmentation
  - Segmented the person from the depth image using thresholding around the known distance (296 cm from the sensor).
5. Limb Measurement and Contour Analysis
  - Calculated distances like thigh and upper arm length.
  - Found normal intersections on the body contour at specific points to measure widths (e.g. thigh, calf, waist, arm).
6. Circumference and Volume Approximation
  - Modeled limbs as cylinders to compute circumferences.
  - Used these values to estimate body mass with a biometric formula from academic literature.
7. BMI Calculation
  - Derived the Body Mass Index (BMI) from the estimated height and weight.

This project showcases practical applications of depth sensing, geometric analysis, and biomedical estimation using Python and OpenCV.