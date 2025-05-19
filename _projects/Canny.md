---
layout: page
title: "Canny Edge Detection Plugin for Krita"
description: "A Krita plugin for customizable Canny edge detection with support for Sobel, Prewitt, and Scharr filters."
image: /assets/images/projects/CannyEdgeDetection/CannyDetection.png
permalink: /projects/Canny/
status: done
priority: 400
tags:
  - plugin
  - python
  - computer graphics
  - solo project
---

This project is a custom plugin for Krita, developed to implement the Canny edge detection algorithm for stylizing and analyzing images. It allows digital artists and designers to apply detailed edge detection on drawings or photos directly within Krita’s UI, using a clean and user-friendly interface.

The plugin integrates seamlessly into Krita under the Tools > Scripts menu. When launched, it opens a control panel where users can fine-tune detection parameters such as thresholds, kernel size, blur intensity, and the gradient calculation method.

Features:
- Adjustable edge detection parameters, including:
    - Lower & upper threshold (0–255)
    - Gaussian blur kernel size and sigma
    - Choice of gradient calculation method: Sobel, Prewitt, or Scharr
- Real-time preview within Krita using custom UI elements
- Clean edge maps for stylization or further processing
- Implemented from scratch in Python using NumPy and Krita’s scripting API

Technical Notes:
- The plugin's edge detection follows all key Canny steps:
    1. Grayscale conversion
    2. Gaussian blur to reduce noise
    3. Gradient calculation using configurable kernels
    4. Non-maximum suppression
    5. Double thresholding and hysteresis to connect weak and strong edges

This plugin was built as part of a graphics programming course and deepened my understanding of image processing algorithms, convolution operations, and UI integration in creative software.