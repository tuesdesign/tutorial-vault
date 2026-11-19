# INFR 2350U: Developing (More) Interesting Shaders

![[Pasted image 20260917031942.png | 300]]
## We will begin shortly
Presented by Constantine Lucius Pallas for Ontario Tech University, Thursday Nov 19, 2026

---

# Recap: Last week, we...

## Talked about the compositing process
## Did some creative shader development

---

# Today We Will...

### Make more shaders
### In-Lab Activity 3

---

## Unity held their annual keynote yesterday

### Let's have a look at their new graphics demo
https://www.youtube.com/watch?v=QfXsGwrBgVg

---
### Reflections

![[Pasted image 20261119010142.png]]


---
## Glass Effect
### Receives reflections from a probe
### Transparency and tint
### Diffused specular highlights

![[Pasted image 20261119020521.png]]



---
# Very Basic Implementation
### When we use a Reflection Probe, metallic materials will automatically sample that probe

### This is really barebones though - we'd prbably want to tune it to fit our game's art style

![[Pasted image 20261119015909.png]]

## Play around with which faces are rendered, material modes, blend styles, probe properties and additional textures

---
# A more advanced implementation
## Notice the refraction, depth tint, and glassy surface 
![[-jjQwKIiE-04a0Fw.mp4]]

---

# Water

### Vertex manipulation
### Transparency and Reflections

![[Pasted image 20261119023652.png]]


---
# Very Basic Implementation
## This doesn't do any depth-based colouring

![[Pasted image 20261119023101.png]]

![[Pasted image 20261119023757.png]]

---
# First, subdivide a plane
### The more faces, the better it will look - here I am using ~16k tris

### Of course, balance this to a sensible level depending on the size and importance in the scene

![[Pasted image 20261119021015.png]]


---

# In-Lab Activity 2

### Select one of the effects we looked at today (Water or Glass) and improve the look to fit some art style.

### To Submit: A link to a GitHub Repo containing your source code and a readme file. The readme should contain screenshots of any shader graphs and your finished effect, and the answers to these questions:

### What effect did you choose, and what game did you try to match?
### What new elements have you added?

### Due tonight at 11:59 PM
