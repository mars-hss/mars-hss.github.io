---
title: Learning
excerpt: ""
header:
    teaser: images/learning/arl.gif
permalink: /course-project/learning
collection: course-project
sidebar:
    - title: Overal Learning Method
      text: Biologically-Inspired Learning for Humanoid Robots(BiLHR)
    - title: Reinforcement Learning
      text: Applied Reinforcement Learning(ARL)
learning:
    - url: images/learning/learning.png
      image_path: images/learning/learning.png
      alt: Brain with Learning1
    - url: images/learning/learning2.png
      image_path: images/learning/learning2.png
      alt: Brain with Learning2
arl:
    - url: images/learning/arl_2.jpg
      image_path: images/learning/arl_2.jpg
    - url: images/learning/arl_3.jpg
      image_path: images/learning/arl_3.jpg
    - url: images/learning/arl_4.jpg
      image_path: images/learning/arl_4.jpg
    - url: images/learning/arl_5.jpg
      image_path: images/learning/arl_5.jpg
---

## Biologically-Inspired Learning for Humanoid Robots(BiLHR)
Handle three types of learning via human brain.
- Supervised Learning
- Unsupervised Learning
- Reinforcement Learning
{% include gallery id='learning' caption="From BiLHR slides / Figure1: Neural mechanisms of learning and control(Doya 2001)" %}
   
   
### Supervised Learning
A type of learning is inferring a model from labelled training data. It requires the explicit provision of input-output pairs. Supervised learning occurs by constructing a mapping from input to the output pairs.   

{% include figure.html url="true" img="images/learning/bilhr_nao.gif" caption="2D data supervised learning beteween vision(X, Y) and motors(Sholder)." %}


### Unsupervise Learning
A type of learning refers to the problem of trying to find hidden structure in unlabelled data. It has no concept of target data. Unsupervised learning performs processing only on the input data.   

## Reinforcement Learning
{% include figure.html url="true" img="images/learning/rl_diagram.png" width="100%" %}
A type of learning is considered a hybrid of supervised and unsupervised learning. It simulates the human learning based on trial and error. RL uses a scalar reward signal to evaluate input-output pairs and hence discover, through trial and error, the optimal ouputs for each input.

### Approximate Dynamic Programming and Reinforcement Learning(ADPRL)
The course focused on the theoretical aspects of reinforcement learning. It covered topics ranging from decision-making, deterministic and stochastic processes, and Markov Decision Processes (MDPs) to Bellman Equations and Operators, Dynamic Programming (DP), Q-learning, Monte Carlo methods, and Temporal Difference learning. ADPRL did not include deep learning concepts due to organizational reasons. In essence, deep reinforcement learning (DRL) replaces the mapping from state to action with a neural network. I will explore the theoretical components of reinforcement learning in more detail later.


### Applied Reinforcement Learning(ARL)
ARL focused on the application of reinforcement learning from scratch. Unlike ADPRL, it concentrated on building an RL algorithm based on a game called "Hexball." The use of neural networks was prohibited for this project. Instead, we designed our own reinforcement learning approach, primarily using Q-learning, and implemented it in C++.   
<br/>

{% include figure.html url="true" img="images/learning/arl_1.jpg" %}
{% include gallery id='arl' %}

#### Result Video
{% include figure.html url="true" img="images/learning/arl.gif" %}