---
title: "Early fall detection from video using 3D-CNNs"
permalink: /portfolio/detectaTrip
---

*Code and initial results coming soon*            

According to the CDC, along with the aging population in the United States, the fall related fatality rate is increasing - up 30% from 2007 to 2016. Over 3 million elderly people are treated in emergency departments each year as a result of fall related injuries. Accurate and real-time detection of falls is vital to timely intervention and minimization of long term effects. Current state-of-the-art focuses on video- and sensor-based detection systems. Video based monitoring is ubiquitous in hospitals and elderly care homes where fall detection applications can be most helpful. Our work aims to localize falls in RGB video feed. 

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

## Presentation


<div align="center">
  <iframe src="https://onedrive.live.com/embed?cid=6CC13FE5E023D836&amp;resid=6CC13FE5E023D836%21112&amp;authkey=AJSHOkE_-oQlk3Y&amp;em=2&amp;wdAr=1.7777777777777777" width="610px" height="367px" frameborder="0">This is an embedded <a target="_blank" href="https://office.com">Microsoft Office</a> presentation, powered by <a target="_blank" href="https://office.com/webapps">Office</a>.</iframe>
</div>


