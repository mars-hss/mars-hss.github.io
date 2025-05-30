---
title: IMDL
excerpt: ""
header:
    teaser: images/imdl/imdl2.jpg
permalink: /course-project/imdl
collection: course-project
mermaid: true
sidebar:
    - title: MDL1
      text: Basic sensors and mechatronics
    - title: IMDL2
      text: BLDC, EtherCAT, and PCB
imdl1_gripper:
    - url: images/imdl/gripper_first.png
      image_path: images/imdl/gripper_first.png
      alt: First Desgin
    - url: images/imdl/gripper.png
      image_path: images/imdl/gripper.png
      alt: Second Design
imdl1_robot:
    - url: images/imdl/imdl1_2.jpg
      image_path: images/imdl/imdl1_2.jpg
      alt: Final Gripper and Platform
    - url: images/imdl/imdl1.jpg
      image_path: images/imdl/imdl1.jpg
      alt: Final Robot
imdl2_act:
    - url: images/imdl/actuator1.png
      image_path: images/imdl/actuator1.png
      alt: Actuator1
    - url: images/imdl/actuator2.png
      image_path: images/imdl/actuator2.png
      alt: Actuator2
imdl2_pcb:
    - url: images/imdl/pcb1.png
      image_path: images/imdl/pcb1.png
      alt: PCB1
    - url: images/imdl/pcb2.png
      image_path: images/imdl/pcb2.png
      alt: PCB2
imdl2_robot:
    - url: images/imdl/imdl2_gripper.png
      image_path: images/imdl/imdl2_gripper.png
      alt: Gripper Design
    - url: images/imdl/imdl2_robot.png
      image_path: images/imdl/imdl2_robot.png
      alt: Robot Design
---
## Intelligent Machine Design Lab

In this course, we learned how to build a robot.
1. Learn sensors(Datasheet) and code with Microchip(C Language).
2. Mechanical Design for specific parts of a robot.
3. Integrate Hardware, Firmware and high-level Software.
   

**From IMDL1, we focused on learning sensors with circuit and controlling DC motor.**   
IR sensor(CNY70, LTH301), Memory(MCP4151-SPI), Motor(FIT0403)
   

### IMDL1 - Project
{% include figure.html url="true" img="images/imdl/imdl1_project.png" caption="From IMDL1 slides" %}
1. Use sensors, motors, and 3D parts with SAME54 Xplained Pro development board to build mobile platform.
2. High-level board(Intel UP Squared) commumnicate with SAME54 Xplained Pro with sensors' data.
3. IR Localization to use a [method](https://ieeexplore.ieee.org/document/1267272).
4. Use gripper to pick up and down an object.
5. Drive to target point with collision avoidance(Ultrasonic sensors).
   

<div class="mermaid">
stateDiagram
    [*] --> IDLE
    IDLE --> Localization: Command
    Localization --> IDLE: IR_sensor
    IDLE --> Moving: Target_Position
    Moving --> Obstacles: Sonar_sensor
    Obstacles --> Moving: Change_Path
    Moving --> IDLE
    IDLE --> Pick_up: Command
    Pick_up --> IDLE
    IDLE --> Drop_off: Command
    Drop_off --> [*]
</div>

**Design a gripper for a mobile robot**
{% include gallery id='imdl1_gripper' %}
   

**Gripper and Robot**
{% include gallery id='imdl1_robot' %}
   

**From IMDL2, we focused on learning BLDC with hall sensors, EtherCAT, and PCB Design.**
### BLDC with hall sensors
{% include figure.html url="true" img="images/imdl/bldc_structure.png" caption="[ABLIC](https://www.ablic.com/en/semicon/applications/bldc-motor/)" %}

{% include figure.html url="true" img="images/imdl/operating_bldc.gif" caption="[What are Brushless DC Motors - RENESAS](https://www.renesas.com/en/support/engineer-school/brushless-dc-motor-01-overview)" %}
{% include figure.html url="true" img="images/imdl/imdl2_bldc_diagram.avif" caption="[Commutation Logic for BLDC - Microchip](https://microchip.my.site.com/s/article/Commutation-Logic-for-Brushless-DC--BLDC--Motor-Control)" %}

Using above logic, design firmware for BLDC controller. We designed also firmware from understanding CAN bus for EtherCAT using LAN9252.


### IMDL2 - Project
{% include figure.html url="true" img="images/imdl/imdl2_project.png" caption="From IMDL2 slides" %}
1. Design a PCB and solder all electronic parts to operate each actuator.
2. Design a whole frame to build a 2DoF manipulator with gripper.
3. Using protocol EtherCAT to operate the manipulator with simulink.
4. Move an object using a motion planning algorithm(RTT).

**Actuators and PCBs**
<div class="mermaid">
flowchart LR
  A(Joint Design):::white--> B(Configurations):::white
  B --> C(Task Space simulation):::white
  C --> D(Dynamic simulation):::white
  D --> E{Joint torque acceptable?}:::white
  E --> |No| B
  E --> |Yes| F(CAD Design):::white
  classDef white fill: #fff, stroke: #000, stroke-width: 2.5px
</div>
{% include gallery id='imdl2_act' %}
<figcaption>First and Seond joint acturator design from CAD</figcaption>
{% include gallery id='imdl2_pcb' %}
<figcaption>First and Seond PCB design from ECAD</figcaption>
    


**Gripper and Robot**
{% include gallery id='imdl2_robot' %}
<figcaption>End-effector and an assembeled whold robot from CAD</figcaption>

**Result Video**
{% include figure.html url="true" img="images/imdl/imdl2_result.gif" %}
<figcaption>Pick and place an object from cabinet to bottom.</figcaption>