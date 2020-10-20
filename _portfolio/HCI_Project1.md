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
<div align="center">
  <img src='/images/hci/brainstorm_group.png'>
</div>

## User Research - Diary Study: Event-Contingent Protocol

### Diary Form Links 

[Student Diary](https://docs.google.com/forms/d/e/1FAIpQLSdBQSXwwy4MeFa6Xqi2hXcXX9tboxZj_UnweTyj3J-ZOMpu9Q/viewform?usp=sf_link)

[Instructor/TA Diary](https://forms.gle/UN4nomS1U2A6ggAM6)

### Target User Demographic

While Zoom is widely used during this COVID-19 era, our primary user demographic are university **students** and **teaching staff**. 

### User Personas

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

From the 18 responses received, all students, and almost all TAs believed that in person office hours are much better than online. 

### Results: Primary Sources of Breakdowns
- Screen sharing is to an entire room, therefore students need to be put into private breakout rooms to share screen 
- Breakout rooms need to be activated, many students and instructors do not know how to use breakout rooms functionality 
- When joining a meeting, TA’s do not know if they have successfully launched the meeting 
- When joining a meeting, students do not know if the TA has joined the Office Hours, if they are in the right office hours, or if the office hours have started/ended 
- Students must use other platforms, e.g. be on phone in addition to joining zoom, if they would like to work with other students while also joining office hours 

## Design Adaptations to Address Breakdowns

### Rooms View 
Current State: Only instructors can setup break out rooms. Many instructors do not know how to setup break out rooms. Leads to breakdown and the instructor ends up keeping all students in the waiting room. Additionally, our user research led us to discover another breakdown surrounding student-student collaboration. Students are currently unable to do so as they are either in the waiting room or listening to the TA answer another student’s question. Many students reported not knowing other students in the class to work through problems and course concepts with, which leads to increased demands on the instructors. Thus to address these breakdowns, we introduced the ability for students to create breakout rooms. 

We have redesigned the Zoom interface to have an interactive “Rooms” tab, where users can more seamlessly view where the TA is and discuss with other students based on topics. The TA has the additional functionality to create private breakout rooms to which users can only be assigned by the TA following the existing break out rooms assignment process. 

Instructor view on the left, student view on the right. Both students and instructors can create breakout rooms. Only instructors can make private break out rooms. 
<div align="center">
  <img src='/images/hci/roomsView.png'>
</div>

###  Pre-Office Hours Questionnaire 

During our user research, we found that TA’s often struggle to address everyone’s questions in the limited amount of time, and often repeat the same recommendation to many students who all have the same question.

To address this breakdown, we propose the Pre-Office Hours Questionnaire. Open for 30 minutes before office hours. Students will be able to submit what homework problems they have issues with as well as the type of question they have. TA’s will view the results when they begin their office hours, and will be able to create break out rooms related to relevant questions. Students can then join these breakout rooms to interact with other students while waiting for help. Additionally, the TA can view the types of questions people have, and structure their time accordingly. Lastly, using state of the art NLP methods, the submitted form will be analyzed and the most common questions/key words from all user submissions will be analyzed to give the TA a summary of topics that they should focus on.            

**Student View:**
<div align="center">
  <img src='/images/hci/formStudentView.png'>
</div>

***Instructor Views - Construct Form: ***
<div align="center">
  <img src='/images/hci/formTAView.png'>
</div>

***Instructor Views - View Form Results:
<div align="center">
  <img src='/images/hci/formResults.png'>
</div>

### Student: Office Hours Status

Surprisingly, we found that both students and TA’s often wonder whether the office hours are active and whether they are on the right link. This leads to a breakdown of closing out of zoom and tracking down the link a second time to confirm they have the right one, or students emailing the TAs to check whether office hours are occurring/in progress. Therefore, after joining the link, we have added a landing page where users can see the status of office hours as well as their place in line if they are a student. 

<div align="center">
  <img src='/images/hci/status.png'>
</div>

### Student Queue for TA

A breakdown we observed is that TA’s lose the order in which students join when they admit students into the meeting. Thus, may TA’s keep students in the waiting room so they can see the order in which they joined. Additionally, TA stated that they spent time with students who were only interested in listening in to the office hours, which increased overhead of the office hour. 

To address this breakdown, we propose an Office Hours Roster/Queue. TAs can view the order in which the students joined, as well as the type of question they have (e.g. 1:1, general, just listening in, etc). Students who are just listening in, will not be included in this schedule view. Only students who have requested 1:1, debugging, or general will be listed. The TA can customize how this is ordered (e.g. general questions first, debugging/1:1 last). 

<div align="center">
  <img src='/images/hci/studentOrder.png'>
</div>

### Share to all students from breakout room

We found that many students attend office hours in order to learn from others. They often stated “you sometimes don’t know what you don’t know, until you hear other student’s questions.” Likewise, TA’s found that they were often answering questions multiple times across students. 

To address these breakdowns we propose the “Share to All” and “Listen In” features. These features allow the TA to share content with the whole office hour session if they decide it may be helpful for everyone. Similar to one person asking a question at in-person office hours and the TA addresses everyone in attendance.

***Instructor View:***
<div align="center">
  <img src='/images/hci/shareToAll.png'>
</div>

***Student View:***                  
The student will be able to decide whether to listen/view the content that the TA is sharing.
<div align="center">
  <img src='/images/hci/listenIn.png'>
</div>

### Whiteboard More Accessible 
Zoom comes with a whiteboard and annotation features. But most users did not know that this feature exists. Therefore, in our redesign we have made it more prominent. In zoom’s current interface, the whiteboard feature can be shared by a user for other users to view and annotate, but when the user switches to sharing a different screen, this whiteboard is no longer visible to other users. This is non-intuitive for a format like office hours where users may want to collaboratively contribute to a derivation or switch between the screen showing the assignment and this whiteboard area. In our redesign, not only is the whiteboard feature now more visible to users, but it also stands on its own, specific to each room in the meeting. This gives users a chance to use a white-board as they may in-person as more of a space to collaborate and share visual ideas that they can easily go back and forth to as they are referencing other views in the meeting. 

<div align="center">
  <img src='/images/hci/whiteboard.png'>
</div>

## Prototype Evaluations
### User 1:
<iframe width="560" height="315" src="https://www.youtube.com/embed/pJs9IxHcEXk" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### User 3: 
<iframe width="560" height="315" src="https://www.youtube.com/embed/78H6idsqfFc" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### Evaluation Tasks

**Student**
Please join a zoom session as you would a student.
Please enter your meeting id and join the meeting.
Please submit some questions for the TA.
Select Problem 3, Lecture Material for topics.
Select Debugging Help and Just listening in for type of question.
Enter information for the corresponding topics you selected and click Done.
Now that the Office Hours is Active, join the session. 
Please join the general discussion room.
Listen in on the breakout room shared by the TA
End your listen in
Navigate back to the rooms overview
Move to the second side room
Open the whiteboard 
Close the whiteboard

**TA**
Please join a zoom session as you would a host.
Since your credentials are already entered, sign in.
Setup the form for your Office Hours session
Click anywhere to setup your form.
Click Publish Form.
Now that it is time to begin your Office Hours, click start.
Choose to open breakout rooms for all questions.
Click Done to open the session to students. 
Join Erica in Breakout Room Q1 to help her with her programming issue. 
You feel the whole class should have an opportunity to see your solution to this common issue. Let the rest of the students have the option to listen in. 
End the Listen In sharing.
Open the Rooms overview.
Open the participants pop up window. 
View the Queue Order.
Sort the roster by Type
Remove the student Erica from the roster since you already helped her. 
Close the roster 
Click and drag Eve from Side Room 1 to Breakout room Q2 to help her with her problem. 

### User Evaluation 

***Positive Feedback***
**User 1:** Found the new prototype to be a significant improvement over the existing platform. He found the overall “rooms” view to be far more interactive, and as a TA appreciated the ability to organize the office hours in cases where there are many students. His favorite part of the new platform was the share screen with everyone feature and is excited to see this implemented in a high fidelity prototype. The user was confused at first by the interaction with the Rooms view, as this has not been a part of video conferencing platforms, but he noted that he has used such interfaces as part of interactive video games, and thinks this is a great addition to a Zoom-like platform. 

**User 3:** User 3 is very familiar with the zoom platform from both a TA and a student perspective. As a student, User 3 is most frustrated by long wait times, and so felt that the pre-office hours form and the ability to meet with other students in the meantime was most helpful. Since user 3 does not know many people in one of her classes, User 3 felt that the topic wise breakout rooms would be a great way to meet other students. Additionally, user 3 loved the ability to return to a whiteboard even once it was closed. As a TA, User 3 felt that the form integrated with the breakout room functionality was the best part of the redesigned platform. However, as discussed below, she also felt that it is still a bit rough. She also felt that the listen in and the share with all features were a great step towards recreating in person office hours.  

**User 4:**User 4 is familiar with the zoom platform from only a student perspective. User 4 thought that although initially a bit overwhelming, the set-up of the rooms interface made a lot of sense and that the circular view of the room was intuitive over some other format. User 4 felt that having used the interface just one of two more times, she would have no issue interacting with this feature to its full extent.

***Areas to improve***
**User 1:**  felt that it was not fully clear how to interact with the new interface and existing zoom functionalities. In a future iteration with a high fidelity prototype, we would look to improve the full extent of the zoom functionality along with the new designs. Additionally, the user felt that the forms view could be more refined to provide more insight to the TA. The user felt that this new interface still does not address the problem of people talking over each other, and it would be great if some type of notification mechanism and pose detection could be used to better understand when individuals want to speak. Additionally, the user felt that the listen in and share with all features could be made more intuitive. As they currently are in the low-fidelity prototype, it is not immediately evident what these functionalities provide. 

**User 3:** User 3 felt that the need to set up a form for every office hour would be very time intensive for the TA/instructor. Though she acknowledges that this form may also save them more time than it would take to set it up. However, given that most assignments are now on Piazza/Gradescope, she said it would be amazing if there was some way these could be integrated in order to make the form generation more seamless. Additionally, she felt that the whiteboard app could be even more prominent within the application.
