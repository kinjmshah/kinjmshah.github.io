---
title: "6-DOF robot manipulation using inverse kinematics, resolved rate, and gradient control methods"
permalink: /portfolio/rdkdc
---

Developed manipulation algorithms in MATLAB to perform pick and place with intention and writing tasks using a UR5 robot.          
*Additional details are available in the attached [report](https://www.kinjshah.com/files/RDKDCFinalProject.pdf)

## Written Task
<div align="center">
  <img src='/images/rdkdc.png'>
</div>
Implemented inverse kinematics control method to achieve task of writing RDKDC (acronym for course Robot Devices, Dynamics, Kinematics, and Controls) at any orientation once the robot is told the location of the top right corner of the page. 

The primary challenge for this task was to establish the local coordinate frame of the paper and the written letters. To achieve this goal, our team established the process below:
1. "Teach" the robot the keypoints of the written letters (robot manually moved to each of the 27 points shown in the figure)
2. Collect joint angles of the UR5 at each of the 27 points 
3. Collect joint angles for the 4 corners of the paper 
4. From the joint angles, calculate the transformation matrices 
5. Store all transformation matrices offline 
6. Establish local coordinate frame of paper 
7. Move robot arm to top right corner and initialize writing process 

### [Task Performance Video](https://www.youtube.com/watch?v=aduOeCUExFI&t=16s)

## Place and Mark with Intention Task
<div align="center">
  <img src='/images/homeandintent.png'>
</div>
Implemented forward kinematics, inverse kinematics, and resolved rate control methods to achieve following steps: 
1. “Teach” the robot: Use UR5 interface to manually position the robot 
2. Establish new home: Establish configuration that avoids the singularities met by the ur5 home position 
3. Intention Pose: Display direction “intention” by establishing intention pose (home to intent pose shown in figure above) 
4. Perform control trajectory: Inverse Kinematics, Resolved Rate Control, Gradient Control         

### [Task Performance Video](https://www.youtube.com/watch?v=9ZHz0VcOGyU)

