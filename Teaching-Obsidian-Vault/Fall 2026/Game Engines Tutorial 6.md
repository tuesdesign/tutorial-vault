 Game Engines Tutorial 6

INFR 3110U: Game Engine Design & Implementation
Tutorial #5
## We will begin shortly

![[Fall 2025/Game Engines Week 2/giphy.gif]]

Presented by Constantine Lucius Pallas for Ontario Tech University, Monday November 2, 2026

---

# In Today's Tutorial

## Review of Libraries
## Review of Extensions
## Independent Work Time

---

# What are libraries?
![[Enchanted_Book.gif]]
### Think back to the concept of abstraction. 
### Oftentimes, we have sections of code that we'd like to re-use or build on.

---
## Within our codebase, we would do this by getting a reference to or inheriting from existing classes.

![[Pasted image 20261102122235.png]]

## The behavior of one piece of code is dependent on another. In this way, we 'link' these pieces of code together

---
# What usually happens
### Although our code might be written in many separate files, during the build process, they are assembled and linked together into a single file called a binary.

![[Pasted image 20261102123903.png]]


---
# Dynamically Linked Libraries
## Suppose we told our game to look for a library in a separate file to our binary. We could switch it out, and it could change the functionality of the program without having to recompile it.

![[Pasted image 20261102121925.png]]

---
# What can we do with this?

![[Pasted image 20261102124256.png]]

---

# What can we do with this?

![[Pasted image 20261102124452.png]]

---

# Extensions

## It's often the case that some functionality written for one game could be useful for another

![[Pasted image 20261102124921.png | 400]]

### Engines give us a useful way to do this

---
# Packages
### Packages are a method to bundle code, assets, and editor functionality into re-usable libraries

### Most engines have a similar concept 

![[Pasted image 20261102125053.png]]

---
# Editor Scripts
### We'll talk more about these next week, but they're an excellent use case for this.

### Here's a simple one that can help us to see trigger colliders

![[Pasted image 20261102125823.png]]

---

# Live Demo
### Let's make a package