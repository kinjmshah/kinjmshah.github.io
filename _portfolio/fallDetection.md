---
title: "Early fall detection from video using 3D-CNNs"
permalink: /portfolio/fallDetection
---

*Code and initial results coming soon*            

Along with the aging population in the United States the fall related fatality rate is increasing - up 30% from 2007 to 2016 [1]. Every year, over 3 million elderly people are treated in emergency departments as a result of fall related injuries [1]. Accurate and real-time detection of falls is vital to timely intervention and minimization of long term effects. Current state-of-the-art focuses on video- and sensor-based detection systems. Video based monitoring is ubiquitous in hospitals and elderly care homes where fall detection applications can be most helpful. Our work aims to recognize and detect onset of falls from the video. 

<div align="center">
  <img src='/images/dl2020/dl2020_storyBoard.png' width="600px"/>
</div>

## Approach       
The availability of fall datasets is extremely limited. Existing simulated datasets do not accurately capture falls *"in-the-wild"* as falls are unexpected actions and therefore difficult to simulate. However, action recognition is a well studied field with many open-sourced datasets. Therefore, we implemented a transfer learning approach using a [3D-ResNet architecture](https://github.com/kenshohara/3D-ResNets-PyTorch) pretrained on the Kinetics-700 action recognition dataset and performed supervised fine-tuning on fall datasets.

### Demo
A demo of our model performance can be seen below. The outer border represents the label (fall vs. no fall) at each timestep while the inner border represents our prediction (Red = No Fall, Green = Fall). 

<div align="center">
  <img src='/images/dl2020/dl2020_oopsGif.gif'>
</div>

<!-- ### Datasets
Simulated Falls: [URFD](http://fenix.univ.rzeszow.pl/~mkepski/ds/uf.html)
Real-World Falls: Using post processing of the recently released [Oops! dataset](https://oops.cs.columbia.edu/) we were able to extract a small dataset of real-world falls -->


