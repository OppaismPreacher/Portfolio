---
layout: page
title: "Thermal Camera Image Processing & Fusion"
description: "Image processing pipeline for thermal cameras: alignment, segmentation, and temperature overlay using OpenCV."
image: /assets/images/projects/ThermalCamera/OverlayedImage.png
permalink: /projects/ThermalCamera/
status: done
tags:
  - computer vision
  - python
  - solo project
---

This project involved analyzing and enhancing thermal data from a thermographic sensor by aligning it with RGB images, extracting temperature data, segmenting hot regions, and calculating the surface area of heat-emitting components.

The workflow combines real thermal camera data with RGB imagery, using Python and OpenCV to normalize, map, and overlay data in a meaningful visual format.

Key Steps:
1. Data loading & normalization
    - Loaded temperature data from a CSV file and corresponding RGB image.
    - Normalized the thermal data to visualize and prepare it for overlaying.
2. Temperature mapping to RGB image
    - Selected matching points in both the thermal and RGB images.
    - Used cv2.getPerspectiveTransform() and cv2.warpPerspective() to align the thermal data with the RGB image.
3. Binary segmentation of hot regions
    - Applied threshold-based segmentation to isolate areas within a critical temperature range (e.g., 36–50 °C).
    - Removed outliers (like a USB resistor) that distorted thermal analysis.
4. Color overlay
    - Mapped thermal intensities to a colormap (e.g., JET) and overlaid it onto the original RGB image with alpha blending.
    - Resulted in a composite thermal-RGB visualization.
5. Surface area calculation
    - Converted selected thermal blobs (microchips) into real-world units (cm²).
    - Calculated the heating surface areas of each hotspot using calibration and geometry.

Technologies & Tools:
- Python, NumPy, Matplotlib
- OpenCV (image transforms, overlays, segmentation)
- CSV-based temperature data with camera calibration

This project bridges hardware data interpretation and image analysis, and demonstrates practical computer vision applications for diagnostics or inspection.
