---
title: Manipulation
excerpt: ""
header:
    teaser: images/manipulation/arcl_panda.gif
permalink: /course-project/manipulation
collection: course-project
sidebar:
    - title: Advanced Robot Control and Learning
      text: Robothon project 
    - title: Multi-sensory Based Robot Dynamic manipulation
      text: Kinematics and Dynamics
msbrdm_space:
    - url: images/manipulation/ur10_taskspace.png
      image_path: images/manipulation/ur10_taskspace.png
      alt: Taskspace
    - url: images/manipulation/ur10_singularity.png
      image_path: images/manipulation/ur10_singularity.png
      alt: Singularity
msbrdm_ellipsoid:
    - url: images/manipulation/control_ellipsoid.png
      image_path: images/manipulation/control_ellipsoid.png
      alt: Normal Control
    - url: images/manipulation/control_singularity.png
      image_path: images/manipulation/control_singularity.png
      alt: Singularity
msbrdm_OpTask:
    - url: images/manipulation/OpTask.png
      image_path: images/manipulation/OpTask.png
      alt: Trajectory of end-effector
    - url: images/manipulation/OpTask.gif
      image_path: images/manipulation/OpTask.gif
      alt: Rviz video

---

**Both courses dealt with kinematics and dynamics of a robot and control theory.**   

## Advanced Robot Control and Learning(ARCL)   
ARCL handled more theoretical parts with a project at the end.

## Project(ARCL) - Robothon
Robothon had two tasks. First task is self collision and second one is obstacle avoidance. The subtask for me was 'Indentifing and avoiding self-collision from given joint and Cartesian trajectories'. The given task is validating joint configuration and end-effector's homogeneous transformation from home position. I used MoveIt with RRT* from OMPL.   
{% include figure.html url="true" img="images/manipulation/mode3.gif" caption="Joint Configuration(From Home poistion to target joints)" width="90%" %}
{% include figure.html url="true" img="images/manipulation/mode4.gif" caption="End-Effector pose(Linear movement from home to a target point)" width="90%" %}
   
## Multi-sensory Based Robot Dynamic manipulation(MSBRDM)
MSBRDM giave more pratical tutorials by each section from homogeneous transform matrix(Rotation and Translation) to dynamics and control.   
   
**The first part is kinematics.**   
Using homogeneous transfrom, publish TF for UR10 from DH parameters(3 DoFs from 6 DoFs).   

{% include gallery id='msbrdm_space' %}
<figcaption>Task space and Singularities for UR10 from MSBRDM tutorial slide</figcaption>
{% include gallery id='msbrdm_ellipsoid' %}
<figcaption>Manipulability Ellipsoid from MSBRDM tutorial slide</figcaption>

**The second part is dynamics.**   
Formulate a dynamic equation from centor of Mass and lengths of links for each joint(3 DoFs).
{% include figure.html url="true" img="images/manipulation/Tau_0.gif" caption="Tau is zero for UR10" %}

{% include gallery id='msbrdm_OpTask' %}
<!-- ## Project(MSBRDM) -  -->