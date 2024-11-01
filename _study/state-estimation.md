---
title: "State Estimation"
collection: study
excerpt: "State Estimation for legged systems"
permalink: /study/state-estimation
tags:
    - state estimation
---

### 1. Linear Kalman Filter
[Experimental Evaluation of Simple Estimators for Humanoid Robots](https://hal.science/hal-01574819v2/document)
[Reference_Repo](https://github.com/qiayuanl/legged_control/tree/master/legged_estimation)

#### Method
State $X = \{ Base_{pos}, Base_{vel\_lin}, P_1, P_{n}, ... \}$
Base position and linear velocity and Contact positions (Humanoid: 2, Quadruped: 4)

Measurement $Y = \{P_1, P_2, ... , V_1, V_2, ..., H_1, ..., \}$
P : Position vector for each foot.
V : Velocity vector for each foot.
H : Height of foot.

Update $F, G, Q$ from time.
Prediction
$\hat{X}_0 = X_{init}$
$X' = F\hat{X}_n + Gu_n$
$P' = FP_nF^{\top} + Q$

Update $H_n, R, Y$ from pinocchio.
Update section
$Y_{error} = Y - H_nX'^{\top}$
$S_n = H_nP'H_n^{\top} + R$
$G_{kalman} = P'H_n^{\top}S_n^{-1}$

$\hat{X}_{n+1} = \hat{X}_n + G_{kalman}Y_{error}$
$P_{n+1} = (I-G_{kalman}H_n)P'$
$P_{n+1} = \frac{P_{n+1} + P_{n+1}^{\top} }{2}$



### 2. Extended Kalman Filter
[State Estimation for Legged Robots - Consistent Fusion of Leg Kinematics and IMU](https://roboticsproceedings.org/rss08/p03.pdf)

[State estimation and localization of legged robots : a tightly-coupled approach based on a-posteriorimaximization](https://theses.hal.science/tel-03715727)