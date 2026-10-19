# INFR 2350U: Intro to Computer Graphics Tutorial 4
# More Lighting

![[Pasted image 20260917031942.png | 300]]
## We will begin shortly
Presented by Constantine Lucius Pallas for Ontario Tech University, Thursday Oct 8, 2026

---
# Today we will...

## Discuss reflections
## Implement Lighting models
## Prepare for the Midterm
## In-lab Activity 1

---
# In a previous Lab...
## We talked about different lighting models
![[Pasted image 20261008082648.png]]
## How do they work?

---
# Flat shading

## Lighting Calculation: Per-face
## Can be interpolated or 'smoothed out'

![[Pasted image 20261008101504.png]]

---
# Gouraud shading

## Lighting Calculation: Per-face
## We actually calculate the light value in the vertex shader

 ![[Pasted image 20261008102119.png]]


---
# Phong Shading

## Adds Specular highlights
![[Pasted image 20261008102812.png]]

---
# Specular
## Has the material properties of a mirror (ie: reflectiveness)
![[Pasted image 20261008102914.png]]

---
# Specular highlights
## A basic form of reflection we expect to see in somewhat shiny objects is a specular
![[Pasted image 20261008082936.png]]

https://www.youtube.com/watch?v=JmfQLHMw7N8

---
# Reflection

## This is a subset of reflective properties

https://www.youtube.com/watch?v=hk6c15z63x4

---
# Review for Midterm

# Theoretical Component
### Short, Multiple choice based
### Review Lecture slides and previous assessments, these questions are very similar
### Be sure to leave enough time for the practical component

---
# Review for Midterm
## Practical Component 

### Longer, more involved
### Create an interactive project that makes use of several of the techniques and patterns you've learned thus far

### You will likely need to recreate a scene and/or specific behaviors, and add some of your own

### You will need to articulate your ideas effectively in a reflection

### You will be under a tight time constraint, divide your time effectively between tasks
 
### Advice: Setup a repo and empty project first, push often.

---
# 10 Minute Break
---
# In-Lab Assignment 1

## Your goal: Create two shader effects with interesting effects

## Vertex Shader
## Fragment Shader

## Use some of the following effects

Reflections
Lighting continued
implementing vertex lighting
implementing smooth lighting
adding specular highlights
In-lab make a cool shader