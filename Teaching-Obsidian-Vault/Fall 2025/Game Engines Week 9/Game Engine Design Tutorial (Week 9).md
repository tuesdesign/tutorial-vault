# INFR 3110U: Game Engine Design Tutorial (Week 9)
![[Fall 2025/Game Engines Week 2/giphy.gif]]
Presented by Constantine Lucius Pallas for Ontario Tech University, Thursday October 31, 2025

---
# In today's Tutorial

### Written Midterm Review Session

### Brief review of Command and Observer Patterns

### In-Lab Assignment 2

### Independent Work Time

---
# Written Midterm Review Session

### I have graded copies of your Midterms, and an answer key. Let's Go over the answers together.

### Do not take photos of the midterm, and be sure to hand them back when we are finished.

---
# What is a Command?

## It can often be helpful to implement game features in terms of a series of actions.

## These actions might produce different results depending on the context, or we might need to reference previous actions. 

## A command Lets us represent and interface with an action or transformation using code.

---
# A Command Gives us...

## A way to define a given action using data/code
## An interface to invoke (and often also undo) the effects of the action

## A way to store this data, if it is needed

---
# When might we use a Command?

## The player needs to be able to undo an action

## We need to record the 'history' of a certain action (ie: moves on a board game)

## We have an action which can provide a different outcome based on context.
---
## When should we * not * use a Command?

## We just need a way to invoke functionality (use an exposed/public function)

## We need to store data, but that data doesn't represent specific actions (use File I/O, PlayerPrefs, Scriptable Objects, etc)

---
# Examples

## We are making a chess game, and we need to keep track of what each player does on their move.

## We are making a game with a level editor like Mario Maker, and we want the player to be able to undo any mistakes they make.

## We are making a game where the player can give instructions to an NPC. We want them to be able to queue up multiple actions which they should perform in sequence.  

---
# Good References

## Your slides
### Unity Learn
https://learn.unity.com/tutorial/use-the-command-pattern-for-flexible-and-extensible-game-systems?uv=6&projectId=67bc8deaedbc2a23a7389cab

---

# What is an Observer?

---
# An Observer Gives us...

## A way for a given object to broadcast some element(s) of its state (or more generally that something has happened) to other Objects

## A way for other objects to "subscribe" to this effect by defining how they will react when the broadcast is sent


---
# When should we use an Observer?

## When one action requires many objects to react

## Different objects that react will do so in unique ways

## We want to separate code for reactions to an event from the object the event occurs to. (ie: don't call UI functions in the player script) 

---
# When should we * not * use an Observer?

## When it would be simpler to get a reference to the subject

## When we need a higher level implementation, such as a UnityEvent

## When the observing object and the subject need 2-way communication

## We need to maximize performance

---
# Examples

## When we pause the game, we need to notify all the enemies and NPCs in our game to pause their movements and animations, and the audio manager must pause the music.

## When the player falls into a pit of lava, all the enemies should play a victory animation, a sound effect should be played, and the UI should display an 'On Fire' status effect.

---
# Good References

## Your slides
### Unity Learn
https://learn.unity.com/tutorial/create-modular-and-maintainable-code-with-the-observer-pattern?uv=6&projectId=67bc8deaedbc2a23a7389cab
---

# In-Lab Assignment 3

## Goal: Create (or ideally update) a small interactive Project / Game to demonstrate your knowledge of Programming Patterns

## Choose your own adventure! This week, you can implement the Command OR Observer Pattern

---

# In-Lab Assignment 2

## Requirement 1: Create (or ideally update) an interactive game project that makes use of the Command OR Observer Design Pattern <!-- element class="fragment" -->

## Requirement 2: Create (or ideally update) a Repo to publish your work, including source files and a build/release <!-- element class="fragment" -->

## Requirement 3: Document your work and answer the reflection questions <!-- element class="fragment" -->

# Exact requirements on Canvas <!-- element class="fragment" -->
# Due 11:59 PM Tomorrow Night (Sat Nov. 1) <!-- element class="fragment" -->

---
# Notes on Grading

### I cannot grade functionality if a functioning build/release is not included
### I cannot grade implementation if source code is not included
### If your source code is not (plain text) visible in your repo (Ie: Blueprints), you must include a screenshot of the relevant code.

### Thank you all very much for remembering to do this last time!

---

# Independent Work Time
#### I'm happy to help, and I'll be here as long as you are. Feel free to ask me questions or for advice.