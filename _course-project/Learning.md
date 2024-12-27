---
title: "Learning"
excerpt: ""
header:
    teaser: images/learning/arl.gif
permalink: /course-project/learning
collection: course-project
sidebar:
    - title: "Overal Learning Method"
      text: "Biologically-Inspired Learning for Humanoid Robots(BiLHR)"
    - title: "Reinforcement Learning"
      text: "Applied Reinforcement Learning(ARL)"
learning:
    - url: "images/learning/learning.png"
      image_path: "images/learning/learning.png"
      alt: "Brain with Learning1"
    - url: "images/learning/learning2.png"
      image_path: "images/learning/learning2.png"
      alt: "Brain with Learning2"
---

## Biologically-Inspired Learning for Humanoid Robots
Handle three types of learning via human brain.
- Supervised Learning
- Unsupervised Learning
- Reinforcement Learning
{% include gallery id='learning' caption="From BiLHR slides / Figure 1:Neural mechanisms of learning and control(Doya 2001)" %}
   
   
### Supervised Learning
A type of learning is inferring a model from labelled training data. It requires the explicit provision of input-output pairs. Supervised learning occurs by constructing a mapping from input to the output pairs.   

### Unsupervise Learning
A type of learning refers to the problem of trying to find hidden structure in unlabelled data. It has no concept of target data. Unsupervised learning performs processing only on the input data.   

## Reinforcement Learning
{% include figure.html url="true" img="images/learning/rl_diagram.png" %}
A type of learning is considered a hybrid of supervised and unsupervised learning. It simulates the human learning based on trial and error. RL uses a scalar reward signal to evaluate input-output pairs and hence discover, through trial and error, the optimal ouputs for each input.

### Approximate Dynamic Programming and Reinforcement Learning
$$
Q(s,a) = Q(s,a) + \alpha\big(r(s,a,s') + \gamma^{i}\max_{a}Q(s',a)-Q(s,a)\big)
$$
### Applied Reinforcement Learning
