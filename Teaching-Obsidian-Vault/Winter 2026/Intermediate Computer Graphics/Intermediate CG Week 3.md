# INFR 2350U 
### Intermediate Computer Graphics

### Tutorial 3 (cameras cont'd)
### We will begin shortly.
#### Tutorial Presented by Constantine Pallas

---

# On the Agenda today
### Lab Activity 1 requirements and Overview
### Overview of Cinemachine, Animators
### Interpolation & Animation curves
### Independent work time - Lab Activity 1

---

# Lab Activity 1

## In short
### Make a 10-15 second video
### min. 5 shots of varying types
### Use cinemachine features (ie: blends, tracking)
### Due midnight tonight, full details on canvas

---
# Advice

## 1. Develop a storyboard and source 3D assets.
## 2. Blockout camera positions and scenes
## 3. Create a 'simple pass' using the timeline
### Populate scenes with in-frame details, add camera transitions
## 4. Add 'Juice'
### Dynamic focus/fov, Post-Processing Effects, Shaders, etc
### Approach each addition as an opportunity to make a new pass

---
# Submission Requirements

## Unity Project Files (Do not submit a build or zipped project folder, upload your project to version control ie GitHub).
## Video (Include an unlisted YouTube Link in your GitHub ReadMe file or in your submission textbox)
## Shot List (you can use my template as a base).

---

# What is Cinemachine?

---
# The built-in Unity camera can be restrictive. 

![[Pasted image 20260202021123.png]]

---
# Especially when we have multiple perspectives 
## There's no built-in way to switch between them - other than a hard cut.

![[Pasted image 20260202021239.png]]

---
# Reasons why we might want a more elaborate camera solution

---
# Smooth transition to alternate viewpoint 
![[Pasted image 20260202021511.png]]

---
# Cutscenes

![[Pasted image 20260202021930.png]]

---
# Algorithmic, dynamic, or gameplay-driven camera targets 
![[Pasted image 20260202022035.png]]

---
# Cinemachine gives us some additional tools
## Multiple 'virtual' Cameras and a central 'brain'

<split even gap=0>
![[Pasted image 20260202022203.png | 300]]
![[Pasted image 20260202022209.png| 300]]
</split>

---
# About Cinemachine Brain and Cameras
https://youtu.be/P_ibDJhFVMU?si=Lgqz_GoxOK-Br5Pz&t=87

# How to use Cinemachine with a Timeline
https://youtu.be/Px_H1oyZgGY?si=arkapOIOC8-ebstz&t=82

---
# Let's talk about Easing and Interpolation
![[Pasted image 20260202023638.png]]

---
![[Pasted image 20260202023825.png]]
## When we drag two clips together in a Cinemachine Timeline, we can edit the manner in which we move from one to another.

## You may recognize the 'Curve' data type that defines this.

---
## We call the motion between these cameras 'easing' or interpolation.
![[Pasted image 20260202023929.png]]
## There are many types of easing patterns.
---
# Core Concept - Interpolation
### Here, we are interpolating between two positions (3D vectors) across time (single axis)
![[Pasted image 20260202024207.png | 400]]
## In the future, we might apply a similar technique to select between colours, which are also 3D vectors.

## We can think of interpolation patterns as virtual sliders that define how we switch from one thing to another 

---
# Extra Tips

## Try customizing the skybox and view fog.
## Try adding built-in Render features such as screen-space Ambient Occlusion
## Try using (or even animating) the built-in post-processing effects.
![[Pasted image 20260202024900.png| 300]]
![[Pasted image 20260202023457.png | 300]]
![[Pasted image 20260202024824.png | 300]]