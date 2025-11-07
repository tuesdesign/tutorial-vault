# INFR 3110U: Game Engine Design Tutorial (Week 9)
![[Game Engines Week 2/giphy.gif]]
Presented by Constantine Lucius Pallas for Ontario Tech University, Thursday October 31, 2025

---
# In today's Tutorial 

## Update on grading <!-- element class="fragment" -->

## Review of profiling and optimization <!-- element class="fragment" -->
## Independent Work / Team Support Time<!-- element class="fragment" -->

---

# Update on Grading

### Midterms and course project progression now should be returned

### In-Lab Assignment 3 will be returned next week, prior to Assignment 4.

---
# Let's talk about performance!
![[622130c23d21c3873ad2c9ea6fcbb80e.gif]]

---
# The Problem™ 
### "I made the game, and it works, but It doesn't run well!"
![[giphy.gif]]

---
# A worse version of The Problem™
![[Pasted image 20251107035535.png]]

---
# How can we make our games run well?

## Get good.

![[twitter-gif-1762506801206.gif]]
---
# It is possible to over-optimize a game

![[Pasted image 20251107035026.png]]

---
# My argument: 

### (here, I'm counting 'performance' as any desirable optimization - but usually file size, load times, and FPS)
![[Pasted image 20251107040518.png]]
#### Pictured: Sigmoid curve between getting clowned on and never shipping

---
# Areas to engoodify your real projects

## 1. Minimize what is loaded at any time
## 2. Make files included in a build as small as they can be without compromising on quality
## 3. Make use of appropriate programming patterns

## 4. Be a programming magician

---

# Minimize what is loaded at any time
![[source.gif|500]]
## Whenever something is offscreen, don't render it.
## You can achieve this with techniques such as frustum culling, additive scene loading, and chunking.

---

# Make files included in a build as small as they can be without compromising on quality
![[Pasted image 20251107043109.png]]
## Often, perceived quality of an artifact and its cost to performance scale at different rates

## The cost of more detailed 3D models, higher sample rate audio, higher resolution textures, or more frequently polled physics systems may scale linearly or even exponentially

## At the same time, the differences may become imperceptible  

---
## Side Note: The previous picture, while illustrative, was not fully accurate!
![[Pasted image 20251107043239.png]]
## Things that have a high cost to the game's performance are not necessarily valuable, but they can be.

---
# Make use of appropriate programming patterns
![[z3GRJx.gif]]
## Remember that there is always a tradeoff between development time, performance, and features

## Using the tools you've learned, you can avoid the pitfalls of 'junk food': Easy but inefficient code.

---

# Be a programming magician
![[Pasted image 20251107044400.jpg]]
### Photo from Kaze Emanuar on YouTube (This guy is a wizard for sure)

## As programmers, we don't have to adhere to strict rules - As long as it works!

---
# Check out this video!

https://www.youtube.com/watch?v=tKbV6BpH-C8

---
# How do we debug performance?
## Modern game engines have tools called Profilers
## Using these tools, we can see exactly what is taking up time, from rendering or physics to specific functions in our scripts
![[Pasted image 20251107045326.png]]
## We will cover how to read and use the profiler next week

---
# Team Support Time
