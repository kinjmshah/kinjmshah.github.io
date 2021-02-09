---
title: "OptiTrip: Motion Tracking in Video via Optical Flow and Human Pose Estimation"
permalink: /portfolio/fallDetectionOF
---

*Code coming soon* 

We aim to use optical flow and human pose tracking to localize falls from standard RGB video feed. We performed our analysis with videos from a simulated falls database labeled with fall onset and offset, and our a self generated dataset of simulated falls. Our implemetation approach leveraged OpenCV and FacebookAI's Detectron2 libraries. An overview of our approach can be seen below, further details can be found in the attached report and presentation. 

[OptiTrip Report]()

<div align="center">
  <img src='/images/cv2020/processOverview.png' width="600px"/>
</div>

## Presentation
<iframe src="https://onedrive.live.com/embed?cid=6CC13FE5E023D836&amp;resid=6CC13FE5E023D836%21107&amp;authkey=AP8Tlq8Wt064RTg&amp;em=2&amp;wdAr=1.7777777777777777" width="610px" height="367px" frameborder="0">This is an embedded <a target="_blank" href="https://office.com">Microsoft Office</a> presentation, powered by <a target="_blank" href="https://office.com/webapps">Office</a>.</iframe>

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



