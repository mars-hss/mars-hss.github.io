---
title: Navigation
excerpt: ""
header:
    teaser: images/navigation/tas_main.jpg
permalink: /course-project/navigation
collection: course-project
sidebar:
    - title: Introduction to Autonomous System
      text: How to use Navigation Stack
    - title: Multi-robots Navigation System
      text: How to expand nav2 for more robots
nav_robots:
    - url: images/navigation/turtlebot.jpg
      image_path: images/navigation/turtlebot.jpg
    - url: images/navigation/robotino.jpg
      image_path: images/navigation/robotino.jpg
nav_multi:
    - url: images/navigation/t4_nav_num.png
      image_path: images/navigation/t4_nav_num.png
    - url: images/navigation/t1r1_obs.png
      image_path: images/navigation/t1r1_obs.png
---

## Navigation Stack
{% include figure.html url="true" img="images/navigation/nav2_concept.png" caption="Concept of Nav 2" %}


## Implement Reachablable sets for montionb planning
Our team tried to implement a motion planning algorithm in navigation stack.
[Using Reachable Sets for Trajectory Planning of Automated Vehicles](https://mediatum.ub.tum.de/doc/1616878/zgez7fijmubink9ouhet3vqbs.2021_07_11_Paper_Sampling_Reachable_Sets_final_submission.pdf)

{% include figure.html url="true" img="images/navigation/tas_video.gif" caption="Final Result" %}

## Multi-robots Navigation
From Fraunhofer IKS, I implemented Nav2 with Webot.

{% include gallery id='nav_robots' %}
<figcaption>Turtulebot v4 / Robotino</figcaption>


{% include gallery id='nav_multi' %}
<figcaption> 4 robots / 2 robot with obstacles</figcaption>