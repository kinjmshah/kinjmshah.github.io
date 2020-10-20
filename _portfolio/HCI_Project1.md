---
title: "Human-Computer Interaction: Project 1 - Design Remote Interactions"
permalink: /portfolio/HCIDesignRemoteInteractions
---

Kinjal Shah, Kaiyu Shi, Erica Tevere

# Proposed Platform Redesign: Zoom for Office Hours

Zoom has become a major video conferencing platform for universities around the globe for facilitating remote instruction. While Zoom has begun to cater to the needs of remote instruction via additions such as breakout rooms, whiteboards, etc., it still falls severely short of student and instructor needs.

## Brainstorming

<div align="center">
  <img src='/images/hci/brainstorm_officeHours.png'>
</div>
<div align="center">
  <img src='/images/hci/brainstorm_tinderNetworking.png'>
</div>
<div align="center">
  <img src='/images/hci/brainstorm_contentViewing.png'>
</div>

## User Research - Diary Study: Event-Contingent Protocol

### Diary Form Links 

[Student Diary](https://docs.google.com/forms/d/e/1FAIpQLSdBQSXwwy4MeFa6Xqi2hXcXX9tboxZj_UnweTyj3J-ZOMpu9Q/viewform?usp=sf_link)

[Instructor/TA Diary]

### Target User Demographic

While Zoom is widely used during this COVID-19 era, our primary user demographic are university **students** and **teaching staff**. 

### Prototype Evaluation Users

*User 1*
Age: 26     
Gender: Male       
Occupation: 5th year PhD student in Computer Science                   
Level of platform use: High, daily use 
User Role: Student, TA 

*User 2*      
Age: 25
Gender: Male
Occupation: 4th year PhD student in Mechanical Engineering
Level of platform use: High, daily use 
User Role: TA 

*User 3*
Age: 26     
Gender: Female       
Occupation: 2nd year Masters Student                  
Level of platform use: High, daily use 
User Role: Student, TA 



### Rationale

In order to evaluate Zoom for Office Hour use, we needed to evaluate user experience during real office hours. Since office hours are relatively spontaneous events, and are individualized per class, it is not possible for us to observe users interacting with the interface without causing a disruption to the event. Furthermore, we did not necessarily need to observe how a user performed a given list of tasks, but rather we needed to understand how the user interacts with the platform to communicate with others. Therefore, the flexibility of the diary method enabled us to receive input from both teaching staff and student users.                     

*Key interactions for TA:*               
- Start a meeting
- Speak individually with students 
- Answer common questions 
- Breakout rooms facilitation 
- Whiteboard                      

*Key interactions for Student:*                  
- Join a meeting
- Share screen with TA 
- Share screen with another user
- Discuss class material/problems with other students 
- Join rooms 

### Results: Flow Model

We chose to use a Flow Model to interpret our results from the diary study as the Zoom platform is primarily a communication tool. Therefore, we needed to better understand how communications of different forms happen in order to understand how to best improve the application. For this reason, a flow model was more appropriate for our evaluation than a sequential model. 

### Results: Primary Sources of Breakdowns
- Screen sharing is to an entire room, therefore students need to be put into private breakout rooms to share screen 
- Breakout rooms need to be activated, many students and instructors do not know how to use breakout rooms functionality 
- When joining a meeting, TA’s do not know if they have successfully launched the meeting 
- When joining a meeting, students do not know if the TA has joined the Office Hours, if they are in the right office hours, or if the office hours have started/ended 
- Students must use other platforms, e.g. be on phone in addition to joining zoom, if they would like to work with other students while also joining office hours 

## Design Adaptations to Address Breakdowns

### Rooms View 
Current State: Only instructor can setup break out rooms. Many instructors do not know how to setup break out rooms. Leads to breakdown and the instructor ends up keeping all students in the waiting room. Additionally, our user research led us to discover another breakdown surrounding student-student collaboration. Students are currently unable to do so as they are either in the waiting room or listening to the TA answer another student’s question. Many students reported not knowing other students in the class to work through problems and course concepts with, which leads to increased demands on the instructors. Thus to address these breakdowns, we introduced the ability for students to create breakout rooms. 

We have redesigned the Zoom interface to have an interactive “Rooms” tab, where users can more seamlessly view where the TA is and discuss with other students based on topics. The TA has the additional functionality to create private breakout rooms to which users can only be assigned by the TA following the existing break out rooms assignment process. 

Instructor view on the left, student view on the right. Both students and instructors can create breakout rooms. Only instructors can make private break out rooms. 
<div align="center">
  <img src='/images/hci/roomsView.png'>
</div>

###  Pre-Office Hours Questionnaire 

During our user research, we found that TA’s often struggle to address everyone’s questions in the limited amount of time, and often repeat the same recommendation to many students who all have the same question.

To address this breakdown, we propose the Pre-Office Hours Questionnaire. Open for 30 minutes before office hours. Students will be able to submit what homework problems they have issues with as well as the type of question they have. TA’s will view the results when they begin their office hours, and will be able to create break out rooms related to relevant questions. Students can then join these breakout rooms to interact with other students while waiting for help. Additionally, the TA can view the types of questions people have, and structure their time accordingly.           

Student View:
<div align="center">
  <img src='/images/hci/formStudentView.png'>
</div>

Instructor Views: 

Fill out form 
<div align="center">
  <img src='/images/hci/formTAView.png'>
</div>

View form results
<div align="center">
  <img src='/images/hci/formResults.png'>
</div>

### Student: Office Hours Status

Surprisingly, we found that both students and TA’s often wonder whether the office hours are active and whether they are on the right link. This leads to a breakdown of closing out of zoom and tracking down the link a second time to confirm they have the right one, or students emailing the TAs to check whether office hours are occurring/in progress. Therefore, after joining the link, we have added a landing page where users can see the status of office hours as well as their place in line if they are a student. 

<div align="center">
  <img src='/images/hci/status.png'>
</div>

### Instructor: Student Queue for TA

A breakdown we observed is that TA’s lose the order in which students join when they admit students into the meeting. Thus, may TA’s keep students in the waiting room so they can see the order in which they joined. Additionally, TA stated that they spent time with students who were only interested in listening in to the office hours, which increased overhead of the office hour. 

To address this breakdown, we propose an Office Hours Roster/Queue. TAs can view the order in which the students joined, as well as the type of question they have (e.g. 1:1, general, just listening in, etc). Students who are just listening in, will not be included in this schedule view. Only students who have requested 1:1, debugging, or general will be listed. The TA can customize how this is ordered (e.g. general questions first, debugging/1:1 last). 

<div align="center">
  <img src='/images/hci/studentOrder.png'>
</div>

### Instructor/TA: Share to all students from breakout room

We found that many students attend office hours in order to learn from others. They often stated “you sometimes don’t know what you don’t know, until you hear other student’s questions.” Likewise, TA’s found that they were often answering questions multiple times across students. 

To address these breakdowns we propose the “Share to All” and “Listen In” features. These features allow the TA to share content with the whole office hour session if they decide it may be helpful for everyone. Similar to one person asking a question at in-person office hours and the TA addresses everyone in attendance.

<div align="center">
  <img src='/images/hci/shareToAll.png'>
</div>

The student will be able to decide whether to listen/view the content that the TA is sharing.
<div align="center">
  <img src='/images/hci/listenIn.png'>
</div>
