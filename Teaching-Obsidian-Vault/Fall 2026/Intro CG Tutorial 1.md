# INFR 2350U: Intro to Computer Graphics Tutorial 1
# Introduction
![[Pasted image 20260917031942.png | 300]]
## We will begin shortly
Presented by Constantine Lucius Pallas for Ontario Tech University, Thursday September 17, 2026

---
# So... Who is this guy?

<split even gap=3>
![[Pasted image 20250910211644.png|300]]
- My name is Constantine Lucius Pallas
- 2025 Graduate of Ontario Tech Game Development and Interactive Media Program
- Graduate Student (Master's Computer Science, Digital Media)
- TA for Game Engines, Game Sound, Computer Graphics, Game Hardware 
- Interests: Game Development, Music, Technology
- Areas of Research: Virtual Reality, Human Interface Devices, Training Software 
- I have taken this course, and I previously taught the intermediate level graphics course.
</split>

---
# What is this course?

---
# Primary Topics

## Understanding how computers render graphics
## Developing shaders to produce various effects
## Creating unique visual styles using graphics techniques

---

# How can you succeed in this course?

### 1. Be sure to submit assignments before the deadline
### 2. Use the assignments as an opportunity to make your GDW game better
### 3. Experiment with each new technique - Always be making things  

---
# Tools used
## Engine
![[Unity1.png| 200]]
## Version Control
![[Github.png| 250]]
### Unless otherwise stated, all demo projects will use the Universal Render Pipeline (URP)
## 2D Image Editor: Aseprite (LibreSprite is a free alternitive)
## 3D Editor: Blender (Latest version via Steam)

---
# Lab Assignments
### Format: Create and share an interactive project demonstrating understanding of the course topic(s) 
### Guidelines and requirements will be posted during labs
### Lab Evaluations will take place roughly every two weeks, starting next week 
### You will be given time during the lab to complete these tasks

---
# Important things to know

### In every submission, all code and other relevant materials must be visible in your repository or readme. Notably, if you are using Shader Graph, please include high-resolution screenshots of each graph and sub-graph in your readme.


### If you have any questions, please contact me using Discord.

---
# AI Policy
#### From the Lecture 1 Slides

### The use of generative AI is allowed under the following conditions:
-  The assignment clearly indicates where and how AI was used.
- It clearly states how you enhanced and built upon what was provided by
generative AI. 
- Citations of generative AI are provided in the read me file, and a
disclaimer is added to the video report.

### Failure to meet the generative AI conditions will result in zero marks

---
# Let's talk about AI...
### Please keep the discussion civil and respectful to your peers, even if you do not agree 

---
# Today we will...

### Introduce shaders
### Learn how to implement a shading program:
#### - By hand 
#### - In code, using CG
#### - Visually, using Shader Graph

---
# Introduction to the graphics pipeline
### A series of steps that your program/computer follows to go from raw data to pixel colours on your screen  
![[Pasted image 20260119021615.png]]
### Some of these steps are programmable. We call those programs "Shaders"

---
# Shaders

![[Pasted image 20260917041345.png]]
#

---
# Vertex Shaders
### i.e. a program to control position 
![[Pasted image 20260917041512.png | 300]]
### Vertex shaders run once per frame for each vertex of each 3D model

---
# Fragment Shaders
### i.e. a program to control colour
![[Pasted image 20260917042030.png | 300]]
### Fragment shaders run once per frame for each screen pixel taken up by an object

---
# In essence: 
### To abstract the idea of a shader, we can think of it as a function
### It takes in data, processes it according to steps we define, and returns new (useful) data 
![[Pasted image 20260917043038.png]]

---
# Activity: Human Shader
### To illustrate that point, we can manually do the steps that a fragment shader could perform to compute this image!
![[Pasted image 20260917043519.png | 400]]
### Inputs: X, Y (2D coordinates)
### Outputs: R, G, B (Colour)

---
# Activity: Human Shader
### Note that the * symbol is used for multiplication
![[humanshader.png]]

---
# "Hello World" of graphics - smallest URP shader 

![[Pasted image 20260917040505.png]]

---
# In Engine
![[Pasted image 20260917040708.png]]
![[Pasted image 20260917040733.png | 300]]
### As you can see, this only gives us one solid colour

---
# Let's implement the same thing in Shader Graph!

![[Pasted image 20260917050030.png]]

---
# Free Work Time: Group Formation
### It's suggested that you form a course project group as soon as possible
### If possible, GDW groups are a great option.
### Max Group Size: 3
### You may form a group with students from the other tutorial section

---

# Thank you for coming to the tutorial!