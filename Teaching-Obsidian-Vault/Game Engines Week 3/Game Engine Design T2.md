# INFR 3110U: Game Engine Design Tutorial (Week 3)
![[Game Engines Week 2/giphy.gif]]
Presented by Constantine Lucius Pallas for Ontario Tech University, Thursday September 19, 2025

---

# In Today's Tutorial

### Brief Review of the Singleton Design Pattern <!-- element class="fragment" -->
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

# In-Lab Assignment 1

## Primary Goal: Create a small interactive Project / Game to demonstrate your knowledge of Programming Patterns
#### Think of the In-Lab assignments together as a mini Game Jam<!-- element class="fragment" -->

## Secondary Goals: <!-- element class="fragment" -->

#### Don't Overscope: You don't need to make an entire game, only a prototype with limited features <!-- element class="fragment" -->
#### Plan Ahead: Consider that you will need to  4 Programming Patterns in total. You should be able to adapt your idea to create features which showcase each one. <!-- element class="fragment" -->

#### Get practice: Being able to quickly implement Programming Patterns won't only prepare you for assessments in this course, it will also make you better at fast-paced game development. <!-- element class="fragment" -->

#### Please Note- You'll be iterating on this project in future in-lab assignments <!-- element class="fragment" -->
---
# In-Lab Assignment 1
## Requirement 1: Create an interactive game project that makes use of the Singleton Design Pattern <!-- element class="fragment" -->
## Requirement 2: Create a Repo to publish your work, including source files and a build/release <!-- element class="fragment" -->

## Requirement 3: Document your work and answer the reflection questions <!-- element class="fragment" -->

# Exact requirements on Canvas <!-- element class="fragment" -->
# Due 11:59 PM Tonight <!-- element class="fragment" -->

---
# Live Example and Free Work Time 