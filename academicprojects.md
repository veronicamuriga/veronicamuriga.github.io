---
layout: post
title: Academic Projects
permalink: /academicprojects/
---

### MIT SparkLab

I am currently working at [MIT SparkLab](http://web.mit.edu/sparklab/) in the AI Innovation Accelerator (AIIA) search-and-rescue intelligence branch as a lab assistant under Professor Luca Carlone.

The initial objective of my summer research is to leverage MaskRCNN for transfer learning in Kimera (an open-source real-time SLAM software) to generate semantic labels from the RGB images simulated through Flightgoggles. Eventually, I should be able to replace Flightgoggles with real world images and get relatively accurate metric-semantic reconstruction.

This has since evolved into speed-testing and latency reduction of Kimera, while also testing different neural networks to find one whoose trainig data best aligns it for use on Flightgoggles simulations.

My action items so far have been:
* Setting up Kimera (Kimera-VIO-ROS + Kimera-Semantics + dependencies) and running Kimera on test datasets
* Getting ground truth per-pixel semantic labelling from Flightgoggles 
* Testing neural networks (eg MaskRCNN) to generate semantic labels from the RGB image
* Adding throttle nodes and reducing resolution of RGB input into Kimera to reduce the time it takes to get a reconstruction
* Integrating Kimera into the broader RL system- involves generalizing topic names and modifying broadcasting rates to accoount for different input/output buffer


*******

### MIT Aerospace Controls Lab

I worked at [MIT ACL](http://acl.mit.edu) as a lab assistant from January to May 2020 under Professor Jonathan How.

The objective of my research was to conduct testing and debugging of the lab simulator and to help expand it from a quad-rotor to a hex-rotor, which is the lab standard vehicle. I also sought to incorporate wind and air dynamic effects by combining the simulator code with air dynamics code drawn up by another lab member. I also worked on incorporating blade flapping effects into the simulator to factor for the elimination of disymmetry of lift. 

I left my position a lot more comfortable with C++, ROS and Linux systems. I also learnt key logical testing techniques, such as setting checks for variables that might sometimes have null values and are inputs for other functions which would cause unprecedented results down the line.  

A challenge I faced while working on this project was the fact that I was putting together several very independent codebases- the drone simulator code that models flying a quadrotor simulator but does not account for physical properties like wind turbulence and aerodynamic factors that would play a role in real life, and the code that models mathematical Dryden models for turbulence and blade flapping. Working around this involved a lot of debugging in C++ and ROS, and digging into functions to find ways to manipulate them to be more generalizable and easily maintainable in future.

*******

### Interactive Fishing Game Team Project

For my IOT's class final project, my team designed a smart fishing game consisting of a fishing rod, on which was mounted an ESP-32 along with components such as a digital compass for motion sensing, a rotary encoder for a reel, IMU, speaker and buzzer. The user orients themselves towards any given heading and swings the fishing rod. If the line falls within the vicinity of a fish, the user has caught that fish and their points are incremented in a database hosted in a remote server. To communicate with the server, the game was supported by server-side scripts written in Python.

I thoroughly enjoyed he material of the class. I’ve always been really interested in physics and combining it with code to making a product from scratch was amazing. I learnt to navigate team dynamics- how to balance out making people work on things they were already comfortable with doing, with working on something out of one's comfort zone.

******
-------