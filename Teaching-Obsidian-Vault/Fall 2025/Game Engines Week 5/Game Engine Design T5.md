# INFR 3110U: Game Engine Design Tutorial (Week 3)
![[Fall 2025/Game Engines Week 2/giphy.gif]]
Presented by Constantine Lucius Pallas for Ontario Tech University, Friday Oct 3, 2025

---
# In today's Lab...
## Brief Review of the Factory Design Pattern <!-- element class="fragment" -->
## Mid-Term Review <!-- element class="fragment" -->
## In-Lab Assignment 2 <!-- element class="fragment" -->

---
# Aside: You should be doing game jams 
![[Pasted image 20251002123454.png|300]]

---

# What is a Factory?

## We often write code that creates objects with certain properties <!-- element class="fragment" -->

## When we have few distinct objects, we can hard-code the spawning logic (ie: with prefabs and the Instantiate function) <!-- element class="fragment" -->

## When we have many types of objects, or when their features are procedurally generated, this won't work. <!-- element class="fragment" -->

---
# A factory gives us...
### A way to spawn objects (an abstract parent class or an Interface) <!-- element class="fragment" -->
### A way to inherit from the above to change how or what gets spawned (ie: a child class which uses prefabs/arguments or a ScriptableObject to define object properties and spawning behaviour) <!-- element class="fragment" -->
### A method to trigger the spawning behavior from anywhere it is needed <!-- element class="fragment" -->

---

# When should we use a Factory?

## We have many instances of a type of object which share common features (ie: deriving from the same parent class) <!-- element class="fragment" -->

## We want a convenient way to spawn objects that vary in definable ways  <!-- element class="fragment" -->

## We want to implement object pooling later to improve performance <!-- element class="fragment" -->

---
# When should we * not * use a Factory?

## We want to spawn many identical objects (use object pooling on its own) <!-- element class="fragment" -->

## We want to spawn an object one time, or other cases where regular Instantiation would be functionally identical (and simpler) <!-- element class="fragment" -->
---
# Examples
## You're making an action roguelike where the player can upgrade their bullets with a number of properties, you're using a ScriptableObject to update these properties, and you  want to keep your upgrade logic separate from your spawning logic <!-- element class="fragment" -->
## Your game's dialogue system spawns a UI popup with unique properties (font, color, border) depending on which character it is associated with, and you don't want extra bloat in your dialogue code <!-- element class="fragment" -->
---
# Good references
## Your Lecture slides 3.6, 3.7 <!-- element class="fragment" -->
## https://learn.unity.com/tutorial/how-to-use-the-factory-pattern-for-object-creation-at-runtime#67a0dba2edbc2a11101f8ddd <!-- element class="fragment" -->

---
# Review for Midterm

# Theoretical Component
### Short, Multiple choice based <!-- element class="fragment" -->
### Review Lecture slides and previous assessments, these questions are very similar <!-- element class="fragment" -->
### Be sure to leave enough time for the practical component <!-- element class="fragment" -->

---
# Review for Midterm
## Practical Component 

### Longer, more involved <!-- element class="fragment" -->
### Create an interactive project that makes use of several of the techniques and patterns you've learned thus far <!-- element class="fragment" -->

### You will likely need to recreate a scene and/or specific behaviors, and add some of your own <!-- element class="fragment" -->

### You will need to articulate your ideas effectively in a reflection <!-- element class="fragment" -->

### You will be under a tight time constraint, divide your time effectively between tasks <!-- element class="fragment" -->
 
### Advice: Setup a repo and empty project first, push often. <!-- element class="fragment" -->
---
# 5 Minute Break
---
# In-Lab Assignment 2

## Goal: Create (or ideally update) a small interactive Project / Game to demonstrate your knowledge of Programming Patterns

---
# In-Lab Assignment 2

## Requirement 1: Create (or ideally update) an interactive game project that makes use of the Factory Design Pattern <!-- element class="fragment" -->

## Requirement 2: Create (or ideally update) a Repo to publish your work, including source files and a build/release <!-- element class="fragment" -->

## Requirement 3: Document your work and answer the reflection questions <!-- element class="fragment" -->

# Exact requirements on Canvas <!-- element class="fragment" -->
# Due 11:59 PM Tonight <!-- element class="fragment" -->

---

# Notes on Grading

### I cannot grade functionality if a functioning build/release is not included
### I cannot grade implementation if source code is not included
### If your source code is not (plain text) visible in your repo (Ie: Blueprints), you must include a screenshot of the relevant code