# INFR 2370U: Game Sound Tutorial
## We will begin shortly
Presented by Constantine Lucius Pallas for Ontario Tech University, Thursday September 18, 2025

---
# In Today's Session

## Review from previous lecture <!-- element class="fragment" -->
#### ADSR (Sound Envelope) <!-- element class="fragment" -->
#### Types of Microphones <!-- element class="fragment" -->

#### How to Record Sounds <!-- element class="fragment" -->

## Preparation for Upcoming Test <!-- element class="fragment" -->

## Mini Topic: Stealing Sounds <!-- element class="fragment" -->
####  Sampling <!-- element class="fragment" -->
#### Soundfonts <!-- element class="fragment" -->
#### Granular Synthesis <!-- element class="fragment" -->
## Jam Session <!-- element class="fragment" -->

---
# Sound Envelope

![[Pasted image 20250925020001.png]]

## We'll show a live demo of this during the Mini Topic

---
# Types of Microphones

## Condenser

<split even gap = 3>
![[Pasted image 20250925020453.png|200]]
- **Pictured: Blue Blackout Spark SL**
- High detail, picks up on small sounds
- Requires external 'phantom' power
- More delicate than a dynamic mic
- Great for recording Instruments, vocals
- Best results in a sound-isolated space (picks up on room noise)
</split>

---
# Types of Microphones

## Dynamic

<split even gap = 3>
![[Pasted image 20250925022025.png|200]]
- **Pictured: Shure SM58**
- Does not capture intricate detail as well as a condenser mic
- Does not require external 'phantom' power
- Extremely durable compared to other mic types
- A sound-isolated space is less necessary
- Arguably the least fussy
</split>

---
# Types of Microphones

## Shotgun

<split even gap = 3>
![[Pasted image 20250925022925.png|200]]
- **Pictured: Rode NTG2**
- Extremely directional
- Ideal Use: Capture audio emanating from a specific point
- Example: Use multiple to capture a live conversation with minimal crosstalk
- Example: Capture foley sounds of a small object while minimizing background noise
</split>

---
# Types of Microphones

## Ribbon

<split even gap = 3>
![[Pasted image 20250925023805.png]]
- **Pictured: RCA 44-BX**
- Unique sound which is often described as 'warm' or 'smooth'
- Often extremely expensive
- Durability of a wet napkin
- Very mechanically simple
- Often used for studio vocals
</split>

---
# Types of Microphones

## Plate / Boundary

<split even gap = 3>
![[Pasted image 20250925024730.png|200]]
- **Pictured: Sennheiser E901**
- Attaches to a wall or other surface, records sound that hits that surface
- Can be used to capture a reverb profile of a space
- Secretly a condenser mic in a flat rectangular trenchcoat  
</split>

---
# Types of Microphones

## Lavalier

<split even gap = 3>
![[Pasted image 20250925025309.png|200]]
- **Pictured: DJI Mic**
- Extremely portable, often wireless
- Not great quality, but can be easily attached to nearly anything
- The best mic is the one you have, and this is better than a cell phone
- Not many uses for game audio
- Gen Z holds them in a strange way 
</split>

---
# How to Record Sounds

## 1.  Remember to preconfigure your target sample rate and bit depth
## 2. Record in a space with as little background noise as possible
## 3. Be aware of gain levels, avoid going into the red and 'clipping'  

## 4. Organize your files! label, sort, and make backups

---
# Upcoming Test

## 1. Don't be stressed about this one
## 2. Review slides with a focus on the 'technical' (Terms and their definitions, examples given during the lectures.) 

## 3. Everything is True/False or Multiple Choice/Association

## 4. Take your time and don't panic

---
# 5 Minute Break
### When We Return- Mini Topic: Stealing Sounds and Jam Session

---

# Mini Topic: Stealing Sounds

---
# Sampling
![[Fall 2025/Game Sound Week 4/giphy.gif]]
#### Re-Using a (usually small) piece of audio in something else
#### Advantage: draw from existing musical phrases and auditory canon
#### Disadvantage: Not legal unless you attain express permission and licencing from the original copyright holder
---

# Sampling Examples

https://www.youtube.com/watch?v=5AqHSvR9bqs

https://www.youtube.com/watch?v=Y9uDl6IwHWQ

---

# Soundfonts

![[Pasted image 20250925143644.png]]
### The earliest game systems could only produce sound using programmable Duty Chips which make primitive sound waves (sine, square, saw, etc)

#### They either did not support arbitrary sounds (ie: waveform) due to size constraints and hardware limitations

---
![[Pasted image 20250925143948.png]]
### The next generation of systems could play any sounds, but were still restricted by file size

#### A 3 minute WAV file can be ~30MB, the maximum ROM file size for a SNES game is 6MB (including sound, art, code, and everything else)

## How can we play back full-quality songs without storing them?
---
# The Sound Font
![[Pasted image 20250925144116.png]]
## Save a very small WAV of each note played by each instrument and write the songs as a MIDI track

## Implement a Sample instrument to recreate your music at runtime

# This cuts down our file size massively!

---
# Why do we care about this today?

![[Pasted image 20250925144652.png]]

## You can use these Soundfont files with a modern sampler VST program to use these sounds in your own music

## Famously, Toby Fox used soundfonts, such as the one from EarthBound for much of the Undertale soundtrack

## This is also a legal grey area. I personally wouldn't want to pick a legal battle with Nintendo

---
# Granular Synthesis

![[Pasted image 20250925150608.png]]
## What if we take a similar idea to the extreme?

## In this model, we call the shortest unit of sound a Grain 

### We loop through or sample this 'grain' many times per second and apply synth effects to it (ADSR Envelope, Reverb, Filters, etc)

# Live demo?
---

# Jam Session