# INFR 3110U: Game Engine Design Tutorial (Week 3)
![[Game Engines Week 2/giphy.gif]]
Presented by Constantine Lucius Pallas for Ontario Tech University, Thursday September 26, 2025

---
# In Today's Tutorial

### Update on In-Lab Assignment 1 Grading <!-- element class="fragment" -->
### Review of DLLs and Plugin development <!-- element class="fragment" -->
### Look ahead: Upcoming content and Lab Assignment 2 Next Week <!-- element class="fragment" -->

 ### Independent Work / Team Support Time <!-- element class="fragment" -->
 
---
# Lab Assignment 1 Grading In Progress
### Expect your grades to be returned by Next Wednesday at the latest<!-- element class="fragment" -->

---
# What is a DLL?
![[giphy.gif]]
## A library is a bank of code which we can reference and make use of in multiple contexts  <!-- element class="fragment" -->
## When we 'include' a library in our code, we are adding 'links' to everything it implements <!-- element class="fragment" -->

## When we use a standard (static) library, the compiler appends the relevant code at build time <!-- element class="fragment" -->

## A dynamically linked library (DLL) is compiled separately from the rest of the code and only appended when it is used (ie: at runtime) <!-- element class="fragment" -->

---
# When should we use a DLL?

## Code which runs simple operations frequently <!-- element class="fragment" -->
C or C++ can execute many operations more efficiently than C# or Unreal Blueprints <!-- element class="fragment" -->
## Anything you want to be easily mutable <!-- element class="fragment" -->
A DLL can be replaced with a modified version, changing functionality <!-- element class="fragment" -->
## Share code between multiple projects <!-- element class="fragment" -->
Using a symbolic link, you can share code between multiple built games  <!-- element class="fragment" -->

---
# When should we *not* use a DLL?

### Not all code needs to be maximally optimized or modular <!-- element class="fragment" -->
Avoid the trap of premature optimization. Implementing a DLL and interface can add logical complexity <!-- element class="fragment" -->
### DLLs do not have perfect compatibility with every build target <!-- element class="fragment" -->
For example, Apple build platforms won't run DLLs created with Visual Studio, and require a separate Objective-C implementation <!-- element class="fragment" -->
### DLLs are often more challenging to debug than native code<!-- element class="fragment" -->
You cannot, for instance, use the Unity debugger within your IDE<!-- element class="fragment" -->

---
# A Small Example DLL
![[thingdoerdll 1.png]]
## Implementations in C++ require extra work, such as configuring the preprocessor, but this is technically all that's strictly required (this would eliminate the performance advantage) 

---
# DLL Usage
![[thingdoercs.png]]

---
# Look ahead

## Next week is Lab Assignment 2 <!-- element class="fragment" -->
## The topic will be one of the Design Patterns already discussed in the Lecture content <!-- element class="fragment" -->

## Similar to last week, we will review both the topic and assignment requirements <!-- element class="fragment" -->
## You are encouraged (but not required) to use Assignment 2 to improve your project from last time <!-- element class="fragment" -->

## Consider how you might implement each of the patterns you've learned thus far <!-- element class="fragment" -->
---
# Team Support Time
### If you do not already have a project group, consider taking this time to form one.

---
# End of Lab Content for Today
#### Be good to each other!