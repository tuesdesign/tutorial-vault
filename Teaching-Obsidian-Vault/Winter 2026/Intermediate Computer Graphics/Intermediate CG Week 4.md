# INFR 2350U 
### Intermediate Computer Graphics

### Tutorial 4 (Lighting)
### We will begin shortly.
#### Tutorial Presented by Constantine Pallas

---

# On the Agenda today
### Lab Activity 1 Grading Update
### Review: All about lights
#### How do lights work in games?
#### Intro to Normals
#### Baked vs Dynamic Lighting
### Tips to improve lighting
### Independent work / Q&A Time

---

# Lab Activity 1
## Update on Grading

#### Excellent work on Activity 1
#### Please remember to follow the submission guidelines stated in class (ie: file types)

### Expect grades over the upcoming weekend.

---
# How Do lights work in games?

![[Pasted image 20260209014151.png]]

---
# Light is as important as color to a sense of 'realism'

![[Pasted image 20260209014444.png]]

---
# Nearly all modern lighting works by lightening or darkening our textures
![[Pasted image 20260209015141.png]]
### The transformation to the color of each pixel is determined by the lighting model it uses. 
### This happens at different points in the rendering pipeline depending on what lighting technology is used. 

---
# Physics of Light
## A normal is a line perpendicular to a face
## A ray of light can be approximated by a line originating from a source point 
## When this line intersects with a face, it is reflected about the normal of the face.

![[Pasted image 20260209014707.png]]

---
# Types of local shading
## The most basic type of shading (flat) calculates one light color per face
## More advanced shading models approximate the continuous change in received light along a smooth surface
## There are a number of ways of doing this, such as by interpolating the values from every face that shares a vertex (gouraud) or by calculating light per fragment (phong)

![[Pasted image 20260209014301.png]]

---
# Global Illumination
### Modern lighting systems also include global illumination, which allows reflected rays to contribute light to other objects (indirect lighting)

![[Pasted image 20260209022641.png]]

### This can be achieved in a number of ways. It can be approximated or simulated, using baked lights, dynamic lights, or a combination of both.
---
# Baked lights

### It can be too computationally expensive to calculate lighting values every frame - and if our objects never move, that effort will be wasted.  

### We can 'bake' lights by calculating lighting values for every surface ahead of runtime and saving them in a (often very large) texture called a lightmap

![[Pasted image 20260209014919.png | 400]]
 ## Advantages: Fast/cheap at runtime, high resolution ceiling
 ## Disadvantages: lights and objects must be static, large overhead at compile-time 

---
# Even though it is an old technique, baked lighting can produce beautiful results
![[Pasted image 20260209021600.png]]

---
# Dynamic lights

### Dynamic lighting encompasses techniques which are more expensive at runtime but can support moving objects

![[Pasted image 20260209021825.png]]

### We'll learn more about dynamic lights when we discuss ray tracing

---

# How can you improve lighting in your games?
## To demonstrate, I have constructed a small scene in Unity

![[Pasted image 20260209024542.png]]
## Here, we are using the default URP settings and no shadows

---
## First, we will change some camera settings under the 'renderer' tab of our camera   
![[Pasted image 20260209024907.png]]

---
# This image is better (especially if we zoom in), but we have mostly just made it darker

![[Pasted image 20260209024952.png]]

---
# Since this scene is static, we can add an Area Light to a model in the scene
![[Pasted image 20260209025753.png]]

## We'll also enable the SSAO renderer feature

![[Pasted image 20260209031343.png]]

---
# Already, we have a much better-looking result

![[Pasted image 20260209025638.png]]

---
# Our scene is indoors, so we can disable the default directional light (sun), and change some environment settings until they look right

![[Pasted image 20260209030506.png | 400]]

---
# The result looks more natural

![[Pasted image 20260209030326.png]]

---
# We'll add some post-processing effects

![[Pasted image 20260209032353.png]]

---
# Before and after

<split even gap=0>
![[Pasted image 20260209024542.png | 450]]
![[Pasted image 20260209032353.png | 450]]
</split>

## Lighting (and associated effects) can make a big difference!

---
# Independent work / Q&A Time 