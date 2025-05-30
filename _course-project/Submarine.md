---
title: Submarine
excerpt: ""
header:
    teaser: images/submarine/submarine_teaser.jpg
permalink: /course-project/submarine
collection: course-project
sidebar:
    - title: Robotics
      text: Visiting Student in Taltech
---

## Control of UCAT(Submarine Robot)
The course handled basics of robotics with an application.
   
### PID Control
PID(Proportional - Integral - Derivative)   
$$ u(t) = K_p e(t) + K_i \int e(t) dt + K_d \frac{de(t)}{dt} $$   
$$ u(t) $$: Input of control, $$ e(t) $$: Error between current and desired value(current - desired)

Using PID control, I control a depth of a submarine robot.
{% include figure.html url="true" img="images/submarine/depth_control.gif" %}

### Tracking an object
Using yolo, we can recognize a diver in a camera image.
{% include figure.html url="true" img="images/submarine/diver_detection.png" %}

### Fuzzy Logic Control
{% include figure.html url="true" img="images/submarine/fuzzy_logic.png" caption="[Wikipeida Fuzzy control system](https://en.wikipedia.org/wiki/Fuzzy_control_system)" %}


### Kalman Filter
{% include figure.html url="true" img="images/submarine/Basic_concept_of_Kalman_filtering.svg" caption="[Wikipeida Kalman filter](https://en.wikipedia.org/wiki/Kalman_filter)" %}

Implementing the theory above, sensor fusion between vision and sonar to track the diver.
