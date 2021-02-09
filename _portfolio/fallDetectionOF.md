---
title: "OptiTrip: Motion Tracking in Video via Optical Flow and Human Pose Estimation"
permalink: /portfolio/fallDetectionOF
---

*Code coming soon* 

We aim to use optical flow and human pose tracking to localize falls from standard RGB video feed. We performed our analysis with videos from a simulated falls database labeled with fall onset and offset, and our a self generated dataset of simulated falls.

<div align="center">
  <img src='/images/dl2020/dl2020_storyBoard.png' width="600px"/>
</div>

## Approach: 3D-CNNs       
The availability of fall datasets is extremely limited. Existing simulated datasets do not accurately capture falls *"in-the-wild"* as falls are unexpected actions and therefore difficult to simulate. However, action recognition is a well studied field with many open-sourced datasets. Therefore, we implemented a transfer learning approach using a [3D-ResNet architecture](https://github.com/kenshohara/3D-ResNets-PyTorch) pretrained on the Kinetics-700 action recognition dataset and performed supervised fine-tuning on fall datasets.         

### Demo
A demo of our model performance can be seen below. The outer border represents the label (Fall vs. No Fall) at each timestep while the inner border represents our prediction (Green = No Fall, Red = Fall). 

<div align="center">
  <img src='/images/dl2020/dl2020_oopsGif.gif' width="600px"/>
</div>

<!-- ### Datasets
Simulated Falls: [URFD](http://fenix.univ.rzeszow.pl/~mkepski/ds/uf.html)
Real-World Falls: Using post processing of the recently released [Oops! dataset](https://oops.cs.columbia.edu/) we were able to extract a small dataset of real-world falls -->

## Awards

<div>
<head>
<style>
.hide {
  display: none;
}
.seenText { font-size: 1.2em;
  font-weight: bold;}
.seenText:hover + .hide {
  display: block;
}
</style>
</head>
<body>
<div class="seenText" align="center">Intuitive Surgical Best Project Award</div>
  <div class="hide" align="center">
    <img src='/images/dl2020/award.png' width="600px"/>
  </div>
</body>
</div>


<!-- <div align="center">
  <img src='/images/dl2020/award.png' width="600px"/>
</div> -->



