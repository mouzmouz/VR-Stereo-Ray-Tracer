# Stereoscopic Ray Tracer with Barrel Distortion

## Overview
This project implements a stereoscopic ray tracer using the Rayground platform. It generates stereoscopic images by rendering the scene from two slightly offset cameras, simulating human vision. Barrel distortion is applied to the final output for VR compatibility.

## Features
- **Stereoscopic Rendering**:
  - Two cameras with horizontal offsets simulate binocular vision.
  - Split-screen output displays left-eye and right-eye views side by side.

- **Barrel Distortion**:
  - Corrects VR lens distortions using a radial distortion formula:
    \[
    r' = r \times (1 + k_1 \times r^2)
    \]
  - Negative `k1` values create the outward distortion effect.

- **Ray Tracing**:
  - Calculates direct and indirect illumination for photorealistic rendering.
  - Includes objects like a teapot and a rectangular cuboid illuminated by a single light source.

## Language Used
This project is written in **GLSL (OpenGL Shading Language)**, used for ray tracing and rendering shaders.
