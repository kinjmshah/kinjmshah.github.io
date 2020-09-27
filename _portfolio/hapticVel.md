---
title: "Haptic Feedback for Velocity Guidance"
excerpt: "Wearable device prototype to enable motion guidance for rehabilitation through cutaneous haptic feedback.<br/><img src='/images/haptic.png'>"
collection: portfolio
---

Current approaches to motion guidance with haptic feedback largely focus on correcting errors in position. Yet, for applications such as rehabilitation, there are advantages to adding velocity guidance. We developed an experimental platform designed to evaluate haptic feedback as a feasible modality for velocity guidance. This wearable platform consists of two vibration motors actuated via a microcontroller in response to changes in angular velocity of a user's upper limb. The system produces vibrotactile stimuli with intensities dependent on the difference between the participant's velocity and a prescribed velocity profile. The observations made through this analysis will enable future studies into the role of haptic feedback in velocity modulation. Coupled with existing work in trajectory guidance, this system holds the potential to enable more robust motion guidance.

## Wearable Device Design
1-DOF wearable haptic guidance device about the shoulder consiting of two vibrotactile actuators controlled by a Raspberry Pi Zero W (RPi) micro-controller. An Adafruit BNO055 inertial measurement unit (IMU) tracks changes in angular velocity and rotational position. The vibrotactile actuators, RPi, and IMU are sewn into an adjustable compression sleeve that can be fit to the lower arm. The vibrotactile actuators are placed such that they lie on opposite sides of the forearm to most closely replicate human touch based guidance.

<div align="center">
  <img src='/images/haptic.png'>
</div>

## Guidance System
1. Initialization: Arm held parallel to ground to allow for IMU calibration.
2. Range of Motion: User moves arms in full vertical range of motion to establish "safe motion" limits.
3. Velocity Measurement: Angular velocity and Euler angle position data recieved from the IMU at a frequency of 100 Hz. A 3-sample moving average filter is applied to the IMU readings to smooth the velocity signal and remove noise.
4. Vibrotactile Stimuli: Repulsive vibrotactile cues administered in response to the deviation of the participant's velocity from the desired velocity using pulse-width modulation commands. Intensity of stimulus is dependent on Weber fraction for just noticeable difference (JND) for vibration perception.     

*Further details available in [paper](https://kinjmshah.github.io/files/haptics2020_WIP.pdf)  

## Results
Device performance was evaluated under constant and varying desired velocities. The device is able to accurately track the participant's angular velocity in 1-DOF about the shoulder joint and output vibrotactile cues in response to the difference between the participant's velocity and the desired velocity. The left image displays the system's performance with respect to a constant desired velocity while the right displays the performance with respect to a variable velocity profile. The top half of the figure displays the participant's measured velocity over time as compared to the desired velocity while the bottom half displays the activation frequencies of the vibrotactile motors. As shown, when the participant moves at velocities outside of the desired range, the system produces a stimulus in real-time, that increases and decreases in accordance with Weber's Law of Just Noticeable Difference. 
<div align="center">
  <img src='/images/hapticData.png'>
</div>

**Proposing a framework for evaluating haptic feedback as a modality for velocity guidance**    
<ins>Kinjal Shah</ins>, Shweta Ravichandar, Jeremy D. Brown    
*2020 Haptics Symposium - Work-in-Progress Track*     
[Paper](https://kinjmshah.github.io/files/haptics2020_WIP.pdf)         
[Code](https://github.com/kinjmshah/HapticVelocityGuidance)
