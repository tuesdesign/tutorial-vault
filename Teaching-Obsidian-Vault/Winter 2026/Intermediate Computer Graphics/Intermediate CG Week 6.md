# INFR 2350U 
### Intermediate Computer Graphics

### Tutorial 4 (Introduction to image processing)
### We will begin shortly.
#### Tutorial Presented by Constantine Pallas

---
# Questions we will answer today?

### What is an image?
### What is sampling?
### How can an image be manipulated? 
### What is a convolution?
### How do post-processing effects work?
### How can I make post-processing effects?

---
# What is an image?

![[Pasted image 20260223011036.png]]

---
# What happens when we zoom in?

![[spy-kids-lemme-zoom-in-on-that.gif | 400]]

---
# Digital images are made up of pixels

![[Pasted image 20260223011521.png]]

---
# Film cameras work at a chemical level, pixel-based resolution isn't the best comparison 
![[Pasted image 20260223013101.png]]

---
# What happens when we zoom in *more*?

![[spy-kids-lemme-zoom-in-on-that.gif | 400]]

---
# Image pixels are usually scaled to multiple display pixels
# Display pixels are composed of sub-pixels
![[Pasted image 20260223070705.png]]

---
# Subpixels control the colour of each pixel by changing the color of red, green, and blue lights.

![[Pasted image 20260223013353.png]]

---
# Modern display technologies (such as OLED or Quantum Dot displays) employ interesting patterns

![[Pasted image 20260223013303.png]]

---
# We often use RGB to describe the colour of a pixel.

### Each value describes how bright the corresponding subpixel is
### The values range from 0 to 255 (the maximum fidelity of an 1byte/8bit unsigned integer)
### Including the alpha channel, that means we can describe a pixel using 4 bytes of data

![[Pasted image 20260223013730.png]]


---
# Small tangent

### Let's consider that number with more context
### A bitmap image (no compression) with a resolution of 1920x1080 pixels is ~8 megabytes of data

###  Modern GPUs are extremely good at processing images (i.e.  we can use multiple such images to do things hundreds of times per second)

---
# Each pixel is represented by three numbers associated with red, green, and blue. 

## That seems familiar...

![[Pasted image 20260223015533.png]]

---
# We could think about a pixel as a Vector3
## Albeit, one with 1/3rd of the precision
## We can use this idea to trick the GPU into doing useful things. 

![[Pasted image 20260223015628.png]]

### A Normal Map *samples* each pixel of an image to describe a direction and magnitude in 3D space, which is applied to geometry to add fine detail without a massively detailed mesh   

---

# What is sampling?
![[Pasted image 20260223020255.png]]
### Surprisingly, sampling an image and a music track are similar concepts

---

# Here, we have the function y = sin(x)
### To sample the function, we plug in an x value of 2.44 and evaluate it to be ~0.65

![[Pasted image 20260223020612.png]]

### (bonus: all sound waves can be expressed as a sum of sine waves, doing this to a sound wave is where the term 'sampling' in music comes from as well)
---
# Here, we have the cat picture
### To sample this function, we have two inputs and three outputs 
### We plug in an (600, 575) and evaluate it to be (195, 153, 155) 

![[Pasted image 20260223020900.png]]

---
# What can we do with this?
### If we think of images as functions, we can change them in precise ways

![[Pasted image 20260223022148.png]]

---
# We can encode useful data in a texture, sampling allows us to read that data

## This is a depth buffer (or z-buffer). Each pixel is shaded according to how far away it is from the camera

# How might we use this?
![[Pasted image 20260223135408.png]]

---
# In Silent Hill, depth fog was used to hide the game's short render depth

### Nowadays, we might use a similar effect as a creative choice.

![[Pasted image 20260223135633.png]]

---
# Another example is water
### We expect water to look darker with more depth

![[Pasted image 20260223135839.png]]

---
# What is convolution?

## This mathematical operation powers visual effects, data storage, and even AI models.

![[Pasted image 20260223141331.png]]

---

## Similar to addition or multiplication, it is a type of transformation we can use to apply one function to another.

![[Pasted image 20260223022422.png]]

---
# Let's see how we might use that on an image!

![[bill-nye-bill-nye-the-science-guy.gif]]
https://youtu.be/KuXjwB4LzSA?si=6pqsUE6nZLNOoZDy&t=537

---
# We can make some simple effects using only this technique
### e.g. edge detection, various blurs, sharpening, emboss

![[Pasted image 20260223024533.png]]

---
## These transformations can act as building blocks towards interesting art styles

![[Pasted image 20260223024913.png]]

---
# What is post-processing?

### After everything else in the rendering pipeline, post-processing effects are transformations applied to the final rasterized image.   

![[Pasted image 20260223025225.png]]

### These effects could include colour grading, tone mapping, adding bloom or vignette, and many more.

---
# Let's show an example of how we can use a post-processing effect to colour grade a game

![[Pasted image 20260223030028.png]]

---
# Our scene from two weeks ago looks good, but it isn't very distinct

![[Pasted image 20260223030147.png]]

---
# We can create an image called a 'lookup table' to describe what we want any possible colour to become.

![[Pasted image 20260223030258.png]]


---
# Here are some examples of LUTs I have made
![[Pasted image 20260223030806.png]]
![[Pasted image 20260223030737.png]]

---
![[splendorLUT.png]]
![[Pasted image 20260223031127.png]]

---
![[negativeLUT.png]]
![[Pasted image 20260223031158.png]]

---

# Demo: creating a LUT using Aseprite
![[identityLUT.png]]

---
# Some custom post-processing effects

https://www.youtube.com/watch?v=EzjWBmhO_1E
https://www.youtube.com/watch?v=k9g2LaBrirI

---

# Next week

### We will discuss programming your own post-processing effects
## Would you like to go deeper into any of our topics today (displays, sampling, lookup tables, convolution, etc)?