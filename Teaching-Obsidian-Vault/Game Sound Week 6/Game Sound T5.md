# INFR 2370U: Game Sound Tutorial
![[giphy (1).gif]]
## We will begin shortly
Presented by Constantine Lucius Pallas for Ontario Tech University, Thursday Oct. 9, 2025

---
# In Today's Session

## Retrospective: The halfway point <!-- element class="fragment" -->
## Look Forward: Small Group Assignment<!-- element class="fragment" -->

## Mini Talk: Overview of Adaptive Music Methods <!-- element class="fragment" -->
## Technical Jam: Let's Make an Audio System! <!-- element class="fragment" -->

---
# The Halfway Point

![[jon-bon-jovi-take-my-hand.gif|300]]

## Time sure does fly! <!-- element class="fragment" -->
## Thank you very much for attending the tutorials! <!-- element class="fragment" -->

---
# The Halfway Point
## I'd really appreciate your feedback  

![[Pasted image 20251008213205.png|300]]

---
# Looking forward: Small Group Assignment

## Full Breakdown in tomorrow's lecture <!-- element class="fragment" -->
## Audio Components <!-- element class="fragment" -->
#### Sound Effects (Interface, In-Game) <!-- element class="fragment" -->
#### Voice-Over <!-- element class="fragment" -->
#### Music Tracks <!-- element class="fragment" -->
#### Optional: Ambient Sounds and Stingers <!-- element class="fragment" -->

---
# Looking forward: Small Group Assignment
## Group Size: 6 to 9 <!-- element class="fragment" -->
## In addition to sound assets, you must pitch your game and implement your assets in-engine <!-- element class="fragment" -->

## Today's tutorial (and next week's) will have sections about this <!-- element class="fragment" -->

---

# Tips for Small Group Assignment

### Unless your whole GDW team is in this class, you should come up with a new idea for the sake of fairness <!-- element class="fragment" -->

### You don't need a fully-fleshed out GDD, just the relevant parts <!-- element class="fragment" -->

### Form a group with people who don't want to do the same task as you (only one person can be assigned to each role) <!-- element class="fragment" -->

### Don't underestimate the value of a great presentation. Practice! <!-- element class="fragment" -->

---
# Mini Talk: How to use audio in your game engine 
![[Pasted image 20251009012249.png]]

---
# Contents
## Overview and basic strategy
## More advanced... Adaptive!
## Native implementation
## Middleware solutions
## Custom solution
---
# Audio Implementation: Overview

### So we've created some great sounds - How do we add them to our game?
![[Pasted image 20251009012842.png|300]]
### Example code and screenshots for Unity (other engines function very similarly in this regard) 

---
# Implementation Level 1 
![[Pasted image 20251009013057.png]] <!-- element class="fragment" -->
## "Somebody else's problem" <!-- element class="fragment" -->
---
# Implementation Level 2

<split even gap="1">
![[Pasted image 20251009013646.png|200]]
![[1_Y8K6OS08ZvL8STnIAAllAw.gif|400]]
</split>

## "The Programmer can figure out the hard stuff"

---
# We can do better than that
![[giphy (2).gif]]
### We will have to get a little more technical, but the rewards are great
### As a side note, *Learn how to use version control.*
---
# Implementation Level 3
![[gsw6ex1.png|500]]

## "The bare minimum"
---
# Implementation Level 4

## Add Features:
- Configurable Master Volume Level
- Pitch/Version Variation for Repeated SFX
- Unified 'Audio Manager'
- Many More!


## "Quality of Life / Juice"

---
# Implementation Level 5
## ₘᵢₙᵢ Mini Talk: Adaptive Audio
### Any audio which is altered depending on in-game variables such as:
- Player state (position, health, movement speed, animation state, score)
- Game state (enemy count, remaining time, puzzle status)
- Literally anything tracked by your game!
 <br />
### Even very simple automations can elevate the gameplay experience 
---
# What's Possible with Adaptive Audio?
### This is just one example, we'll have a look at more next week when we talk more about this
![[stormcastle-tv.gif]]
https://www.youtube.com/watch?v=NkBXgcN3fXo

---
# That looks hard to do!
### There are a number of highly effective ways to implement your game audio

---

# Middleware
![[Pasted image 20251009022437.png|500]]
### Pros: Provides a high-level editor workflow and does not require as much programming as a custom solution. A lot of the 'heavy lifting' is done for you 
### Cons: May be overkill, or might not be well-suited to your workflow. May represent a greater challenge to integrate with your other systems

#### We will discuss these tools at greater length next session. Would you prefer to focus on Fmod/Wwise/Metasounds specifically in that session? Let me know!

---
# Custom Solution
https://www.youtube.com/watch?v=_xs1Iw474iw
### Pros: Much more granular control - Only implement what you need, with the capability to add truly unique functionality

### Cons: Increased time investment, more programming/technical work 

#### If you like, I could also go into more depth about the architecture of my custom interactive audio engine

---
# 5 Minute Break

---

# Technical Jam: Let's Make an Audio System!