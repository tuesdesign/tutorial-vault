 Game Engines Tutorial 8

INFR 3110U: Game Engine Design & Implementation
Tutorial #8
## We will begin shortly

![[Fall 2025/Game Engines Week 2/giphy.gif]]

Presented by Constantine Lucius Pallas for Ontario Tech University, Monday November 16, 2026

---
# In Today's Tutorial

## Optimizing Games, Part Two

![[Pasted image 20261109020731.png]]

---
# Last week...
### We talked about the goals of optimizing games and common improvements
### We briefly looked at some profiling tools

---
# This week...
### Using the Profiler to measure performance
### In-Lab Activity 2
---
# The Profiler
![[Pasted image 20261116124230.png]]
### Live Demo Later

---
# How can you use design patterns to improve performance?

---
# Scenario 1:
### You have many instances of objects in your scene, each with their own logic.
![[Pasted image 20261116140419.png]]
## You could...
### Use object pooling to reduce memory allocation spikes
### Use a factory pattern to decouple instantiation logic from each instance
### Use static references to a singleton instead of each instance gathering its own references

---
# Scenario 2:
### Many objects in your scene reference a handful of scripts, like a game manager or the player controller.
![[Pasted image 20261116140748.png]]
## You could...
### Convert those scripts to singletons where possible
### Use command/observer patterns to reduce the number ofreferences references needed
### Otherwise reduce the complexity of commonly used methods

---
# Scenario 3:
### You have an expensive operation - Whenever a bunch of objects perform that operation, it causes a lag spike.
![[Pasted image 20261116141229.png]]
## You could...
### Use a C++ DLL (if C# performs worse at that operation)
### Reduce the frequency with which that operation is performed, such as by introducing a tick system, or by handling it for every object using a single manager script.

---
# In-Lab Activity 2

## Your Task: Use the profiler to measure an improvement in your game's performance.

### Requirement 1: Create an interactive scene with a performance bottleneck. Use the profiler to measure its performance 

### Requirement 2: Implement design patterns to improve performance. Use the profile to determine if this was effective.
### Requirement 3: Document your work and answer the reflection questions 

## Exact requirements on Canvas
## Due 11:59 PM Tonight

---
Create interactive game project, or select one you have previously made. Improve its performance using programming patterns. Measure its performance before and after implementing the design patterns. 

Notes on Grading
- Functionality cannot be graded if a functioning build/release is not included. 
- Implementation cannot be graded if source code is not included. If your source code is not (plain text) visible in your repo (ie: you are using Blueprints), you must include a screenshot of any relevant code in your readme

---

To Submit:

A link to a repository (ie: GitHub) containing:

- A readme file with the following contents:
Your name and student number
- A title of your project, and a brief description of its 'gameplay loop'
- Screenshots from the profiler before and after implementing design patterns
- Answers to the following reflection questions:
	- What did you notice was impacting the performance of your project?
	- Which pattern(s) did you implement, and what behavior did they replace?
	- Do your patterns / technique implementations improve performance? Why or why not?
	- Can you demonstrate what the profiling process revealed?
- All Source Files for your project including code and assets. If your project requires any special instructions to open in an editor, include these in your readme file.
- A Release containing a downloadable Windows or Web build of your project (don't rely on a build folder within your repository,)

Grading:
Repo and Release: 10%
Reflection Questions: 20%
Usage of Profiler: 30%
Performance Improvement Measured: 20%
Implementation of Design Pattern(s): 20%
