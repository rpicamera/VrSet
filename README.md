# Dual Pi Camera Vr Set
This project was inspired by a video I watched on Youtube: https://www.youtube.com/watch?v=z9gSZwVMybc. I did some improvements. This project is based on html, so any smart phone can control it.

## Hardware list
1.  Raspberry Pi 3B
2.  Raspberry Pi Zero V1.3
3.  Picon  https://4tronix.co.uk/blog/?p=1224
4.  Two servos and pan & tilt kit
5.  VR camera kit
6.  Two raspberry pi camera module. 
7.  One soft usb->usb mini cable (25cm in length, the softer the better)

## Hardware Setup

## System design
This system is based on the html. A nodejs server will run on RPi 3B, and rpi-cam-web-interface (http://elinux.org/RPi-Cam-Web-Interface) is required. 

Basically, the nodejs server received the requires from the smart phone, which is pan & tilt angle. Then this server passes these data to the picon (I wrote an I2C driver in js for this device.) The servos pan & tilt kit would then move based on these data. On html, the live stream will be shown from two cameras which one connected to RPi 3B and the other one connected to the pi zero. Pi zero act as a USB ethernet gadget to the RPi 3B. So, the communication speed between pi zero and RPi 3B is good enough for the live stream. Since the smart phone connected to the server from RPi 3B, then mount it on a VR headset like google cardboard VR, it would be good to go.  

## Software setup steps

### RPi-cam-web-interface

### Pi zero USB gadget setup

### Setup RPi 3B as USB gadget master

### Nodejs 

### Setup my code and test

## Ending
