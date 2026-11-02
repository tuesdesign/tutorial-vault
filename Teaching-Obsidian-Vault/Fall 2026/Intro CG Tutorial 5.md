
# INFR 2350U: Midterm Review and interpolation

![[Pasted image 20260917031942.png | 300]]
## We will begin shortly
Presented by Constantine Lucius Pallas for Ontario Tech University, Thursday Oct 22, 2026

---


# In Today's Tutorial

## Extended Review of Midterm
### Theoretical - Q&A, Question by Question Breakdown
### Practical - Live Demo
### Interpolation
### Detail Maps

### Independent work time

---
# How did it go?
### Did you feel prepared?
### What took you for surprise?

---
# Theoretical Component

### Grade Check

---
# Theoretical Component
## Breakdown on Canvas

---
# Practical Component
## Extended Live Demo
---
# What to do going forward

## The final exam will follow a similar format
## Practice similar high-speed development (do game jams!) 

---
# Interpolation



![[Pasted image 20261022100015.png]]

---
# Lerp
### Linear Interpolation

---
# We have been using this function often to make shaders - what does it do?

![[Pasted image 20261022110509.png]]

---
## Think of it like a sliding light switch
#### Terms A and B represent the possible states (lights on or off), and the control (usually 't') is a value between 0 and 1 describing which is active (ie: switching between them).
![[Pasted image 20261022110738.png]]
---
# We can interpolate anything...

### Position in 3D space

![[interpolate-1.gif]]

---
# We can interpolate anything...
### Colour

![[df9dda246147c93608a923cbdf9c5d4ced9c12ef.gif]]

---
# There's more than just Lerp
![[Pasted image 20261022110320.png]]

---
# Detail Maps
#### We can use the color of each pixel in an image as a unique control

#### We could control up to three things with a single image by using the different colour channels (or four, if we also use the alpha/transparency channel)

![[Pasted image 20261022095816.png]]

---
# Let's look at some PBR materials and break down how these work

---
# Independent Work Time