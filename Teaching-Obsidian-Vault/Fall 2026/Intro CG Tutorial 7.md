# INFR 2350U: Developing Interesting Shaders

![[Pasted image 20260917031942.png | 300]]
## We will begin shortly
Presented by Constantine Lucius Pallas for Ontario Tech University, Thursday Nov 12, 2026

---

# Today We Will...

### Review:  Developing interesting shaders using compositing techniques

### In-Lab Activity 2

### Independent work time

---
# Compositing

![[Pasted image 20261112021551.png]]

---
# Alpha

### When we combine images together, we need an associated image called a mask, which allows us to separate an image into two parts

### In the era of film, these were often simple or hand-drawn, and used in a lithographic process to either cover (mask) or expose photosensitive film to light.

![[Pasted image 20261112020251.png]]

---
# Single colour 'key' screens are often used to make that process easier

![[Pasted image 20261112020431.png]]

---
# These days, we usually use an extra channel in our image data to contain mask data.

### In that case, we can store information about transparency alongside colour.

![[Pasted image 20261112020546.png]]

---
![[bill-nye-bill-nye-the-science-guy.gif]]

https://www.youtube.com/watch?v=XobSAXZaKJ8

---
# Blend Modes

![[Pasted image 20261112021517.png]]

---
# Decals
### "If you shoot at a wall, there have to be decals" - Gabe Newell

![[Pasted image 20261112022000.png]]

---
# Decals

![[Pasted image 20261112022909.png]]
![[Pasted image 20261112022919.png]]
![[Pasted image 20261112022925.png]]

---
# Decals
![[Pasted image 20261112022938.png]]

---
# The Stencil Buffer

![[Pasted image 20261112022042.png]]
https://www.youtube.com/watch?v=-NB2TR8IjE8

---
## Read Stencil
![[Pasted image 20261112022816.png]]
## Write Stencil
![[Pasted image 20261112022823.png]]

---
# Fresnel Effect 

![[Pasted image 20261112022155.png | 300]]

![[Pasted image 20261112022112.png | 300]]

---
# Creating a Hologram Effect

![[Pasted image 20261112023110.png]]
![[Pasted image 20261112023102.png]]

---
# Creating a Hologram Effect 

![[Pasted image 20261112023010.png]]

---

# In-Lab Activity 2

### Select one of the effects we looked at today (Hologram/Fresnel, Cutout/Stencil, or Decal/Blend) and improve it in some way to make an interesting visual effect

### To Submit: A link to a GitHub Repo containing your source code and a readme file. The readme should contain screenshots of any shader graphs and your finished effect, and the answers to these questions:

### What effect did you choose?
### What new elements have you added?

### How could you use this shader in a game to improve the gameplay?

### Due tonight at 11:59 PM

---
