---
title: Manipulation
excerpt: ""
header:
    teaser: images/manipulation/arcl_panda.gif
permalink: /course-project/manipulation
collection: course-project
sidebar:
    - title: Robothon project
      text: Advanced Robot Control and Learning
    - title: Kinematics and Dynamics
      text: Multi-sensory Based Robot Dynamic manipulation
---

**Both courses dealt with kinematics and dynamics of a robot and control theory.**   

## Advanced Robot Control and Learning(ARCL)   
ARCL handled more theoretical parts with a project at the end.

## Project(ARCL) - Robothon
Robothon had two tasks. First task is self collision and second one is obstacle avoidance. The subtask for me was 'Indentifing and avoiding self-collision from given joint and Cartesian trajectories'. The given task is validating joint configuration and end-effector's homogeneous transformation from home position. I used MoveIt with RRT* from OMPL.   
{% include figure.html url="true" img="images/manipulation/mode3.gif" caption="Joint Configuration" %}
{% include figure.html url="true" img="images/manipulation/mode4.gif" caption="End-Effector pose(HT)" %}
   
## Multi-sensory Based Robot Dynamic manipulation(MSBRDM)
MSBRDM giave more pratical tutorials by each section from homogeneous transform matrix(Rotation and Translation) to dynamics and control.   
The firt part is kinematics. Using homogeneous transfrom, 

{% include figure.html url="true" img="images/manipulation/Tau_0.gif" caption="Tau is zero for UR10" %}
<!-- ## Project(MSBRDM) -  -->