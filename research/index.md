[**Home**](../index.md){:style="margin-right: 10px;"}
|
[**About Me**](../aboutMe/index.md){:style="margin-right: 10px;margin-left: 10px;"}
|
**Research**{:style="margin-right: 10px;margin-left: 10px;"}
|
[**Industry Experience**](../industryExperience/index.md){:style="margin-right: 10px;margin-left: 10px"}
|
[**Projects**](../projects/index.md){:style="margin-right: 10px;margin-left: 10px"}
|
[**Hobbies**](../hobbies/index.md){:style="margin-right: 10px;margin-left: 10px"}
|
[**Travel**](../travel/index.md){:style="margin-left: 10px"}

___

# Research

## Table of contents:

- [Tele-operated Palpation Robot](#tele-operated-palpation-robot-in-progress) ***(In progress!)***
- [PediaCORE ADAPT System](#pediacore-adapt-system-in-progress) ***(In progress!)***
- [Fetal-Maternal Dual Heart Monitoring System](#fetal-maternal-dual-heart-monitoring-system)

___

## Tele-operated Palpation Robot ***(In progress!)***

[Return to Table of Contents](#table-of-contents)

<p align="center">
<img width="595" height="250" src="../pics/HonorsInstrumentation.png">
</p>

This project was completed for the Honors Instrumentation course under Dr. Nitish Thakor at JHU. The aim of the project was to utilize the UR5 robot arm for tele-operated palpation tasks. To accomplish this, me and my project team built a wireless arm tracker which could estimate the user's wrist position relative to their shoulder over time, utilizing the Madgwick sensor fusion algorithm on a pair of 9-DOF IMU sensors. This wrist position is then sent to the UR5 over bluetooth, where it is used as input to the inverse kinematics for control over the UR5. The UR5 then moves to achieve the same end-effector position as the user's wrist, running at a sampling rate of ~20 Hz. For the palpation side of the project, we built a tactile sensing palpation probe that attaches to the end-effector of the UR5. Using a grid array of piezoelectric fabric strips as well as a pair of thermistors, we are able to sense pressure and temperature information from the skin of the patient. This information is then fed back to the user in two different forms of feedback. A GUI heat map demonstrates visually the levels of pressure for each segment of the grid array and the relative temperature of the two thermistors, while buzzer motors in a glove worn by the user provides haptic feedback of the level of pressure felt by the probe.

***Current improvements*** to the project include the following:
- Comparison of the estimation results and computational efficiency of using a Kalman filter in place of the Madgwick algorithm
- Implementation of the MoveIt! motion planning service to increase the efficiency of the inverse kinematics
- Implementing object avoidance using optimal control techniques

**Topics of interest:**
- Medical Robotics
- ROS / Gazebo Simulation
- Robot Kinematics
- Robot Sensors & Actuators
- MATLAB Programming
- Arduino Programming

***Stay tuned, more to come soon!***

___

## PediaCORE ADAPT System ***(In progress!)***

[Return to Table of Contents](#table-of-contents)

<img align="right" width="450" height="300" src="../pics/DesignTeam.jpg">{:style="margin-left: 10px;"}
PediaCORE is a former JHU BME Design Team turned independent research group now housed within the Kennedy Krieger Institute (KKI). Sponsored by Dr. Amy Bastian, Chief Science Officer of KKI, PediaCORE initially formed in the spring of 2018, with the goal of making physical therapy more engaging for children with motor disabilities. Since then, we have developed the ADAPT system, specifically with this goal in mind. As one of the original founders of the team, I have recently taken over the role of Lead Project Manager, and have been in this new leadership position since May 2020. I have since led our team of 12, consisting of undergraduate students, graduate students, and young professionals, through our ongoing first round of clinical studies. We are actively engaging and collaborating with Physical Therapists, Neuroscience experts, and Child Behavioral Psychologists to ensure the ADAPT system is a success. We look forward to seeing what the ADAPT system can accomplish, and sharing more details soon!

**Topics of interest:**
- Medical Device Start-up
- Prototype Research & Development
- Physical Therapy Data Analysis
- Unity Game Development

***Stay tuned, more to come soon!***

___

## Fetal-Maternal Dual Heart Monitoring System

[Return to Table of Contents](#table-of-contents)

<img align="right" width="341" height="400" src="../pics/RobustICA.jpg">{:style="margin-left: 10px;"}
This project was completed through the REU program at University of Washington, Bothell. I worked under Dr. Hung Cao and Dr. Tadesse Ghirmai to develop an algorithm that could take abdominal ECG (aECG) data from a pregnant mother, extract out the separate fetal ECG (fECG) and maternal ECG (mECG) signals, while simultaneously removing any motion artifacts present in the signal. This algorithm utilizes Independent Component Analysis (ICA), and an analysis was done comparing results from using FastICA vs. RobustICA.

**Topics of interest:**
- Wearable Medical Devices
- Digital Signal Processing
- MATLAB Programming
- C++ Programming

***Stay tuned, more to come soon!***