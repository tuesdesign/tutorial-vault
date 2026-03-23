### Intermediate Computer Graphics

### Tutorial 9 (Scaling and sampling)
### We will begin shortly.
#### Tutorial Presented by Constantine Pallas

---

# Today We Will...

### An activity about computation time
### Discuss the progression of rendering technologies
### Preview of Lab activity 3
### Brief demo of VFX Graph

---
# How hard is it to compute a single pixel?
### In today's activity, we will be doing the job of a (fragment?) shader
![[Pasted image 20260323120725.png]]

---
# Choose X value between 0 and 70, and a Y value between 0 and 39

## Then follow the worksheet

### for an extra challenge, try to get your final answer without using a calculator
---
# When we write a fragment shader, how many times does it run per second?

![[Pasted image 20260323114954.png]]

---
# With every major screen resolution increase, pixel density increases at a geometric rate

#### At 4k, over 8 million pixels must be computed per frame
#### At 60 fps, over 497 million pixels must be computed per second!

![[Pasted image 20260323115724.png]]

---
# What are some shortcuts?
### We could render the game at a lower resolution and upscale it
### Using traditional methods, our result would be blurrier and/or less detailed than if we had rendered it at full resolution

![[Pasted image 20260323123320.png]]

---
# DLSS (and FSR, XeSS, etc)
### Use a machine learning technique to produce more detailed upscaled frames  

![[Pasted image 20260323125424.png]]

---
# Modern Implementations

### Modern versions of supersamplers support frame generation, which generates multiple consecutive frames from a single low-resolution render
### In its default profile, DLSS 4.5 fabricates 24 pixels for every one pixel rendered

![[Pasted image 20260323130313.png]]

---
# If the machine learning model is trained on extremely high resolution images, it is (technically) possible for these generated frames to be "better" than the natively rendered ones

### (based on diff scoring from a 'ground truth' image)
![[Pasted image 20260323130610.png]]

---
# We can push this technique very far!

https://youtu.be/DKCyk3CeUFY?si=ENJJ9Jw_pHqE8kJ4&t=177

---

![[Pasted image 20260323130847.png]]

---
# DLSS 5 takes that idea even further, using AI image generation to 'improve' frames

## NVIDIA CEO Jensen Huang says that in the future, 100% of pixels will be generated instead of rendered 

### What do you think?

https://www.youtube.com/watch?v=dJACkKbN-Eo

---
# This is not an entirely new idea

https://www.youtube.com/watch?v=yF1bZiH-wJQ

### In 2019, this idea seemed much more exciting 

---
# Discussion

### What do you think the future will hold?

---
# Lab Activity 3
## Due Mar 30th (next week) at 11:59 PM 
## Let's have a look at what will be required

---

# Brief live demo