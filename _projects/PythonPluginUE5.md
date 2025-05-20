---
layout: page
title: "Unreal Engine Python Runtime Plugin"
description: "A C++ prototype for an Unreal Engine plugin that runs Python scripts at runtime using pybind11."
image: /assets/images/projects/PythonUE5/CppPython.png
permalink: /projects/PythonPluginUE5/
status: prototype
priority: 400
tags:
  - plugin
  - python
  - c++
  - UE5
  - solo project
---

<img src="{{ page.image | relative_url }}" alt="C++ Python UE5" class="project-hero">

This project is a plugin designed to enable the execution of Python scripts at runtime from C++ within Unreal Engine. The system leverages pybind11 to create a bridge between native C++ code and the Python runtime, enabling dynamic interaction between the two languages.

While not yet implemented inside Unreal directly, the core functionality was successfully tested in standalone C++. The long-term goal is to integrate this into Unreal Engine 5 as a plugin, allowing dynamic scripting within the game environment.

Features:
- Python script execution from within a C++ application
- pybind11 bindings for function invocation and data transfer
- Prepared for future integration with Unreal Engine 5

Future Application:
- The plugin is intended for use in a future game where players program virtual robots using Python, allowing them to control movement, perception, and behavior via code. This would create a sandbox environment combining gameplay with real programming concepts.

## Gallery

<div class="project-gallery">
  <img src="{{ '/assets/images/projects/PythonUE5/CppPython.png' | relative_url }}" alt="Scene 1">
</div>