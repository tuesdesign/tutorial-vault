# INFR 3380U 
### Industrial Design for Game Hardware

### Tutorial 3 (microcontrollers)
### We will begin shortly.
#### Tutorial Presented by Constantine Pallas

---

# Today We Will...

### Review Lecture Content
### Choosing a microcontroller for your project
### Basic microcontroller communication
### Continuing our keyboard demo
### Independent Work / Q&A Support Time: Activities

---
# Review Lecture Content



---
## Sensors
### In the case of this light sensor, we need an analog pin and a 5v vcc pin. 
![[Pasted image 20260212154256.png]]

---
## Potentiometers
### Here, we would need a 5v vcc pin, and an analog pin
![[Pasted image 20260212154058.png]]

---
## Joysticks
### Here, we would need a 5v vcc pin, a digital pin for the button, and two analog pins for the x and y axis potentiometers
![[Pasted image 20260212153848.png]]


---
## Button Matrices
### Here, we would need 20 digital pins (5 rows x 15 columns)
![[Pasted image 20260212153643.png]]

---

## LED
### A simple LED can be added using only a single digital pin (ie:  Arduino blink example diagrams)

### We can use Pulse Width Modulation (PWM) to control the brightness of the LED using only a digital pin.

![[Pasted image 20260212154531.png]]

---

## RGB LED

### An RGB LED actually contains three LEDs, one of each color.
### Each color requires its own digital pin
![[Pasted image 20260212154552.png]]

---
# If we were trying to recreate a GameCube controller, how many of each type of pin would we need?

![[Pasted image 20260212154956.png]]

---
# Basic introduction to Firmware

### How can we communicate with our controller?

---

# Firmware
## Firmware is software that runs on hardware such as game controllers that allows for communication between that hardware and software (such as games) 
![[Pasted image 20260212155704.png]]


---
# Ardity

![[Pasted image 20260212160203.png]]

### Arduinos and compatible microcontrollers are capable of emitting data in a serial format (ie: a direct stream of binary data)

### Computer programs can listen for serial data across a COM port (ie: USB ports on your computer)

### Ardity is an extension for Unity which allows us to read this data to a string in a C# script - we can use this to approximate HID syscalls (ie: pressing buttons)

## We'll talk more about Ardity later.
---
# Xinput for Arduino

### Sends signals interpreted as an Xbox controller

### Only compatible with a few Arduinos

---

# Mechanical keyboard firmware

### Sends keycodes, interpreted as keyboard across operating systems

### Some include support for additional features such as rotary encoders, mouse pointers, and LEDs

### Heavily limits your choices in terms of microcontrollers

---
  

# Choosing a Microcontroller

## First, determine the number of pins you need

## Consider additional features such as Bluetooth/battery support, type of USB connector used, size, compatibility with firmware options, and ability to find production files

---

# BBC Microbit
![[Pasted image 20260212172306.png]]
### Simplest to use

### Built in sensors and LED array
### Very few pins

---

# Arduino Uno
![[Pasted image 20260212172247.png]]
### Easy compatibility with breadboards

### Many examples will use these

### Many knock-offs are available

  
---
# Arduino Pro Micro

![[Pasted image 20260212172209.png]]

### Similar feature set to Uno in a smaller package

### Many other microcontrollers will use the same shape and pinout

---

# Seeed Xiao

![[Pasted image 20260212172052.png]]

### Small form factor

### Few pins

### Available with a variety of skus to match project needs

  
---

# If you are planning on making a PCB

### Make sure that you can find a footprint and layout for your exact microcontroller! 

---
# Demo: continuing with our keyboard 

---
# Demo: Ardity

---
# Independent Work / Q&A Support Time