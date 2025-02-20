
As part of my internship at VSD Squadron Mini, where I am working with the CH32V003F4U6, a 32-bit RISC-V microcontroller. VSD Squadron Mini focuses on RISC-V development, embedded systems, and low-level programming,
providing hands-on experience with microcontroller interfacing and software-hardware integration. In this repository, I document my work on various embedded system projects, showcasing the practical application of RISC-V architecture and its integration into real-world solutions.

![1](https://github.com/user-attachments/assets/da2d91b1-2fb9-486e-88f1-5a26d50d373c)

# PROJECT SMARTDOOR


### OVERVIEW OF THE PROJECT
This project is used to give an idea to make a automatic door.

### Key Features 
Fully Automated Door – Uses an ultrasonic sensor to detect movement and opens/closes the door via a servo motor.

Precise Distance Sensing – The HC-SR04 ultrasonic sensor ensures accurate detection of objects within a specific range.

CH32V003F4U6 Microcontroller Powered – Runs on a 32-bit RISC-V core, offering fast processing and low power consumption.

Secure & Hands-Free – Eliminates the need for physical contact, making it hygienic and safe.

Adjustable Sensitivity & Delay – Users can fine-tune the detection distance and door closing delay for customized automation.

Compact & Low-Cost – Uses minimal hardware while delivering smart automation, making it ideal for DIY home automation projects.

Expandable & Upgradable – Can integrate with RFID, facial recognition, or IoT for enhanced security and smart home connectivity.

# Why This Matters 

Scalable and Cost-Effective
Scalable – Perfect for small to medium-sized solar installations, with the flexibility to expand as energy demands grow.
Low Maintenance
This design minimizes manual intervention, reducing the need for frequent adjustments and lowering long-term labor costs.
# How It Works
*  Sensors detect the distance
* Servo motors adjust their  position accprding to it
* Microcontroller processes feedback and ensures alignment
***
# Required component:
* VSD SQUADRON MINI
* ULTRASONIC SENSOR
* LED
* Bread board
***



## PINLAYOUT
The board is powered by USB type

| COMPONENT               | LABLE  |   PINOUT |
|-----------------------|-------------|--------|
| ULTRASONIC SENSOR | GND|GND OF VSD|
||VCC|+5 OF VSD|
||ECHO|PD5|
||TRG|PD2|
| Servo motor |VCC|+5 OF VSD|
||GND|GND OF VSD|
||PWM|PC0|

### DIAGRAM 

![413534824-79d7bfdf-f695-4f3a-8015-ca0068845237](https://github.com/user-attachments/assets/b8c14cda-d033-4344-a62a-629bce622440)

 
