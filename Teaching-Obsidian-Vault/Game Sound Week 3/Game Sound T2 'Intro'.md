# INFR 2370U: Game Sound Tutorial
# 'Introduction'
![[Game Engines Week 2/giphy.gif]]
## We will begin shortly
Presented by Constantine Lucius Pallas for Ontario Tech University, Thursday September 18, 2025

---
# Review Session

#### Exporting Audio <!-- element class="fragment" -->
#### Everything you need to know about sine waves <!-- element class="fragment" -->

---
# Exporting Audio

### Ideal Properties:
### Waveform (WAV) Format <!-- element class="fragment" -->
- Uncompressed (no loss in quality due to file compression) <!-- element class="fragment" -->
- Easily processed by the game engine compared to compressed formats <!-- element class="fragment" -->

### 48kHz Sample Rate <!-- element class="fragment" -->
- ~2x the range of ordinary human hearing <!-- element class="fragment" -->
- Can be perfectly synchronized to video at a multiple of 24 OR 30 FPS <!-- element class="fragment" -->
- Good compromise between file size and quality <!-- element class="fragment" -->
- We will cover what sample rate means later today <!-- element class="fragment" -->

### 24 Bits per Sample <!-- element class="fragment" -->
- At any instant, the volume of the sound is represented by 24 binary digits (1 or 0) <!-- element class="fragment" -->
- Sound can be at any of 8,338,608 unique 'volume levels' at any point in time (144 dB of dynamic range) <!-- element class="fragment" -->
- Floating point arithmetic becomes limiting factor: 24bit is arguably overkill for real-world audio equipment and human ears <!-- element class="fragment" -->
---
# Exporting Audio <!-- element class="fragment" -->
## When to deviate from these options <!-- element class="fragment" -->

### The only reason I can think of: you need to optimize for file size <!-- element class="fragment" -->
- Use a compressed format like Vorbis/OGG, FLAC, or MP3(avoid if possible) <!-- element class="fragment" -->
- Key Tradeoff: Smaller Size = Worse quality and/or more processing power needed to uncompress <!-- element class="fragment" -->
- On Mobile platforms especially, read the build documentation to find out the best format (IOS and Android may mess things up) <!-- element class="fragment" -->

---
# Help with Sine Waves
### Everything you need to know and hopefully enough to make you curious
---
# Desmos Demo
https://www.desmos.com/calculator/ybpsfn8py7

![[Pasted image 20250918133530.png|300]]
---
# Video: "Every Sound is SINE" by Posy
![[stormcastle-tv 1.gif]]
https://www.youtube.com/watch?v=UrBZsUBibtk

---
# Mini Topic Vote 

<split even>
![[Pasted image 20250911013310.png | 300]]
![[Pasted image 20250918130524.png | 700]]
</split>

## The first Mini Topic will be next week

---
# Let's take a 10 minute break 
---
# Jam Session

## Let's make something together
#### Equipment: Microphone, MIDI Controller, Audio Interface