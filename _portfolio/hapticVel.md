---
title: "Haptic Feedback for Velocity Guidance"
excerpt: "Wearable device prototype to enable motion guidance for rehabilitation through cutaneous haptic feedback.<br/><div align="center"><img src='/images/haptic.png'></div>"
collection: portfolio
---

Current approaches to motion guidance with haptic feedback largely focus on correcting errors in position. Yet, for applications such as rehabilitation, there are advantages to adding velocity guidance. We developed an experimental platform designed to evaluate haptic feedback as a feasible modality for velocity guidance. This wearable platform consists of two vibration motors actuated via a microcontroller in response to changes in angular velocity of a user's upper limb. The system produces vibrotactile stimuli with intensities dependent on the difference between the participant's velocity and a prescribed velocity profile. The observations made through this analysis will enable future studies into the role of haptic feedback in velocity modulation. Coupled with existing work in trajectory guidance, this system holds the potential to enable more robust motion guidance.

## Wearable Device Design
1-DOF wearable haptic guidance device about the shoulder consiting of two vibrotactile actuators controlled by a Raspberry Pi Zero W (RPi) micro-controller. An Adafruit BNO055 inertial measurement unit (IMU) tracks changes in angular velocity and rotational position. The vibrotactile actuators, RPi, and IMU are sewn into an adjustable compression sleeve that can be fit to the lower arm. The vibrotactile actuators are placed such that they lie on opposite sides of the forearm to most closely replicate human touch based guidance.

<div align="center">
  <img src='/images/haptic.png'>
</div>

## Algorithm
![Data Image](/images/hapticData.png)

**Proposing a framework for evaluating haptic feedback as a modality for velocity guidance**    
<ins>Kinjal Shah</ins>, Shweta Ravichandar, Jeremy D. Brown    
*2020 Haptics Symposium - Work-in-Progress Track*     
[Paper](https://kinjmshah.github.io/files/haptics2020_WIP.pdf)         
[Code](https://github.com/kinjmshah/HapticVelocityGuidance)
