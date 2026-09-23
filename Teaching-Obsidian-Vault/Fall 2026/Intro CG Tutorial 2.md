# INFR 2350U: Intro to Computer Graphics Tutorial 2
# Intro to Shader Development
![[Pasted image 20260917031942.png | 300]]
## We will begin shortly
Presented by Constantine Lucius Pallas for Ontario Tech University, Thursday September 24, 2026

---
# Recap: Last week, we...

## Introduced the rendering pipeline
## Created a primitive shader using HLSL and Shader Graph
## We even computed a "fragment shader" by hand! 

---
# Today we will...

## Learn more about the rendering pipeline
## Develop more interesting vertex and fragment shaders

---
# Steps of the Rendering Pipeline
## This diagram represents each major step in the rendering process, from raw data to screen colours.

![[Pasted image 20260923012954.png]]

## What do each of these steps do?

---
# We start off with raw data representing a series of points...

![[Pasted image 20260923013727.png]]

---
# By bridging these points with edges/faces, they can represent a 3D object.

![[Pasted image 20260923014332.png]]

---
# Processing Vertices

### The purpose of this step is to transform this 3D information into 2D positions relative to how they should appear on screen

---
# How they should appear depends on the way we do that projection.

#### There are two common types of virtual cameras:
## Perspective and Isometric
<split even gap=3>
![[Pasted image 20260126123244.png | 400]]
![[Pasted image 20260126123517.png | 400]]
</split>

---
# It's all about depth
## With a perspective camera, objects that are far away look smaller
![[Pasted image 20260126123708.png]]
## This is analogous to how the human eye (and real cameras) perceive depth.

---
# Perspective projection is often used in 3D games
![[Pasted image 20260126124029.png]]

---
# Isometric/Orthogonal projection is most often used in 2D games.

![[Pasted image 20260126123916.png]]

---

# How does a perspective camera work in-engine?
### We define a perspective camera by marking an origin point and creating a pyramid with its peak at that point. 
![[Pasted image 20260126124338.png]]
## We slice this pyramid along two planes (one near the point, and one far from the point) to create a shape called a *frustum*.

## Anything between the two planes is in view of the camera - we call this region Clip Space.

---
# Vertex Shaders

![[Pasted image 20260923015300.png]]

### The vertex processing step also allows us to define custom behavior in the form of programmable shaders. For example, in a simple water shader, we might change the height of each vertex over time to form waves.

---
# Rasterizing

## While our models are comprised of continuous edges and faces between their points, there are no guarantees these will align with our finite grid of pixels

![[Pasted image 20260923015659.png]]

---
# By rasterizing, we can transform object vertices into a series of "fragments", which represent a unit of screen space

![[Pasted image 20260923020228.png]]

---
# Fragment Processing
## Of course, we still need to figure out what colours occupy each fragment

![[Pasted image 20260923020709.png]]

## To do this, we will use another type of programmable shader - the Fragment Shader

---
# Fragment Shading

## We can do a whole lot with fragment shaders.

![[Pasted image 20260923021022.png]]

## From lighting and texture sampling to bespoke effects like posterization and toon shading, we have many tools at our disposal to create interesting effects.

---

# Many  interesting effects are possible with shaders.

 
 ![[Pasted image 20260923022339.png]]
## In future weeks, we'll cover many specific techniques and topics in greater detail.

---

# Live Demo

---

NOTES

TO COVER IN LIVE DEMO

- sampling textures
- lighting and shadows
- properties
- making materials from shaders
- The depth map / z buffer
- transparency / alpha channel