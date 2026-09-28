# Game Engines Tutorial 3

INFR 3110U: Game Engine Design & Implementation \
Tutorial #3
## We will begin shortly

![[Fall 2025/Game Engines Week 2/giphy.gif]]

Presented by Constantine Lucius Pallas for Ontario Tech University, Monday September 28, 2025

---


# In Today's Tutorial

### Brief Review of the Singleton Design Pattern <!-- element class="fragment" -->

### Brief Review of the Factory Design Pattern <!-- element class="fragment" -->
### In-Lab Assignment 1<!-- element class="fragment" -->

---
# What is a Singleton?

#### A singleton is a sort of Class with only one single instance<!-- element class="fragment" -->
#### Having only one instance of a class make it easy to find/reference (A Singleton is globally accessible)<!-- element class="fragment" -->

#### A Singleton ensures that it is the only copy of itself<!-- element class="fragment" -->

---
# When should we use a Singleton?

## The Short answer: 'Manager' Scripts<!-- element class="fragment" -->
#### ie: GameManager, AudioManager, SceneMagager, etc<!-- element class="fragment" -->
#### Only one object per scene is of this type, many objects must reference it, and accidently having multiple copies might cause issues.<!-- element class="fragment" -->

---
# When should we * not * use a Singleton?
## The Short answer: Systems which might eventually expand in scope<!-- element class="fragment" -->

### Suppose we used a Singleton to keep track of player data. What would happen if we wanted to add a second player?<!-- element class="fragment" -->

---
# How to implement a singleton
![[Pasted image 20260928131133.png]]

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
# A great example of implementation...

https://learn.unity.com/tutorial/how-to-use-the-factory-pattern-for-object-creation-at-runtime#67a0dba2edbc2a11101f8ddd

---

# In-Lab Assignment 1
## Requirement 1: Create an interactive game project that makes use of the Singleton or Factory Design Pattern <!-- element class="fragment" -->
## Requirement 2: Create a Repo to publish your work, including source files and a build/release <!-- element class="fragment" -->

## Requirement 3: Document your work and answer the reflection questions <!-- element class="fragment" -->

# Exact requirements on Canvas <!-- element class="fragment" -->
# Due 11:59 PM Tonight <!-- element class="fragment" -->

---
# Live Example and Free Work Time 


---
Create an interactive game project that makes use of the Factory OR Singleton Design Pattern
Notes on Grading
- Functionality cannot be graded if a functioning build/release is not included. 
- Implementation cannot be graded if source code is not included. If your source code is not (plain text) visible in your repo (ie: you are using Blueprints), you must include a screenshot of the relevant code in your readme
 

To Submit:

A link to a repository (ie: GitHub) containing:

- A readme file with the following contents:
Your name and student number
- A title of your project, and a brief description of its 'gameplay loop'
- A diagram (ie: Flowchart/Pseudocode/Mermaid/UML or similar) explaining your use of the Command OR Observer Design Pattern
- Answers to the following reflection questions:
  - What element of your game adopts the chosen pattern?
  - Why is this pattern a good choice for the associated    functionality?
  - References to all external assets used
- All Source Files for your project including code and assets. If your project requires any special instructions to open in an editor, include these in your readme file.
- A Release containing a downloadable Windows or Web build of your project (don't rely on a build folder within your repository,)

Grading:
Repo and Release: 10%
Functionality, Interactivity, Expandability: 30%
Use of Design Pattern: 40%
Diagram/Reflection: 20%