# INFR 2350U 
### Intermediate Computer Graphics

### Tutorial 2 (Cameras)
### We will begin shortly.
#### Tutorial Presented by Constantine Pallas

---

# In today's tutorial...

## 1. Review of lecture content
## 2. Live Demo
## 3. Lab Activity 1
## 4. Independent Work Time

---

# How does a virtual camera work?

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
## This is analogous to the human eye (and real cameras) perceive depth.

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

## Anything between the two planes is in view of the camera.

---

# Cinematography


https://www.youtube.com/watch?v=MYlgj1hwcYw

---
# How to find cinematic references
https://film-grab.com/
![[Pasted image 20260126124651.png]]

---
# How to find models: Unity Asset Store
![[Pasted image 20260126130745.png | 300]]

---
# How to find models (and animations): Mixamo
![[Pasted image 20260126130837.png]]

---
# Lab Activity 1

## Available from now until next week at midnight.

## Next week, we will discuss Cinemachine and the Animator, which are required for this activity.

## I Recommend you acquire models and assemble a scene during the lab today.

---
# Independent Work Time
## Thank you for coming to the lab!