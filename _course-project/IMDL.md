---
title: "IMDL"
excerpt: ""
header:
    teaser: images/imdl/imdl2.jpg
permalink: /course-project/imdl
collection: course-project
sidebar:
    - title: "IMDL1"
      text: "Basic sensors and mechatronics"
    - title: "IMDL2"
      text: "BLDC, EtherCAT, and PCB"
imdl1_gripper:
    - url: "images/imdl/gripper_first.png"
      image_path: "images/imdl/gripper_first.png"
      alt: "First Desgin"
    - url: "images/imdl/gripper.png"
      image_path: "images/imdl/gripper.png"
      alt: "Second Design"
imdl1_robot:
    - url: "images/imdl/imdl1_2.jpg"
      image_path: "images/imdl/imdl1_2.jpg"
      alt: "Final Gripper and Platform"
    - url: "images/imdl/imdl1.jpg"
      image_path: "images/imdl/imdl1.jpg"
      alt: "Final Robot"
imdl2_robot:
    - url: "images/imdl/imdl2_gripper.png"
      image_path: "images/imdl/imdl2_gripper.png"
      alt: "Gripper Design"
    - url: "images/imdl/imdl2_robot.png"
      image_path: "images/imdl/imdl2_robot.png"
      alt: "Robot Design"
---
## Intelligent Machine Design Lab

In this course, we learned how to build a robot.
1. Learn sensors(Datasheet) and code with Microchip(C Language).
2. Mechanical Design for specific parts of a robot.
3. Integrate Hardware, Firmware and high-level Software.
   
   
From IMDL1, we focused on learning sensors with circuit and controlling DC motor.
IR sensor(CNY70, LTH301), Memory(MCP4151-SPI), Motor(FIT0403)


### IMDL1 - Project
{% include figure.html url="true" img="images/imdl/imdl1_project.png" caption="From IMDL1 slides" %}

[](https://ieeexplore.ieee.org/document/1267272)

#### Design a gripper for a mobile robot
{% include gallery id='imdl1_gripper' %}

#### Gripper and Robot
{% include gallery id='imdl1_robot' %}

From IMDL2, we focused on learning EtherCAT, BLDC with hall sensors and PCB Design.

### IMDL2 - Project
{% include figure.html url="true" img="images/imdl/imdl2_project.png" caption="From IMDL2 slides" %}


#### Gripper and Robot
{% include gallery id='imdl2_robot' %}