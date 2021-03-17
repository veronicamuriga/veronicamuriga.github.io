---
layout: post
title: Research Projects
permalink: /researchprojects/
---

### MIT SparkLab

During summer 2020, I worked at [MIT SparkLab](http://web.mit.edu/sparklab/) in the AI Innovation Accelerator (AIIA) search-and-rescue intelligence branch as a lab assistant under Professor Luca Carlone.

The initial objective of [my summer research](https://docs.google.com/presentation/d/1a6QX4ZsGHbm3dHmvRBnj5FmknGqfRi2brFXyT2fudUc/edit?usp=sharing) was to leverage MaskRCNN for transfer learning in Kimera (an open-source real-time SLAM software) to generate semantic labels from the RGB images simulated through Flightgoggles. The aim is to replace Flightgoggles with real world images and get relatively accurate metric-semantic reconstruction.

This evolved into speed-testing and latency reduction of Kimera, while also testing different neural networks to find one whose trainig data best aligns it for use on Flightgoggles simulations.

My action items were:
* Setting up Kimera (Kimera-VIO-ROS + Kimera-Semantics + dependencies) and running Kimera on test datasets
* Getting ground truth per-pixel semantic labelling from Flightgoggles 
* Testing neural networks (eg MaskRCNN) to generate semantic labels from the RGB image
* Adding throttle nodes and reducing resolution of RGB input into Kimera to reduce the time it takes to get a reconstruction
* Integrating Kimera into the broader RL system- involves generalizing topic names and modifying broadcasting rates to account for different input/output buffers


*******

### MIT Aerospace Controls Lab

I worked at [MIT ACL](http://acl.mit.edu) as a lab assistant from January to May 2020 under Professor Jonathan How.

My research involved:
- Conducting testing and debugging of the lab simulator and expand it from a quad-rotor to a hex-rotor, which is the lab standard vehicle 
- Incorporating [wind and air dynamics](https://docs.google.com/presentation/d/19Kbac-fTL5wLGF808WAbKQIAuRLFzwZiIPuHjMd7ino/edit?usp=sharing) by combining the simulator code with air dynamics code drawn up by another lab member 
- Incorporating [blade flapping effects](https://docs.google.com/presentation/d/1yYXDTJ7G_zLPxQvvDlohSAqE3KK49iFHhipkQPyv9fQ/edit?usp=sharing) into the simulator to factor for the elimination of disymmetry of lift. 

I left my position a lot more comfortable with C++, ROS and Linux systems. I also learnt key logical testing techniques, such as setting checks for variables that might sometimes have null values and are inputs for other functions which would cause unprecedented results down the line.  

A challenge I faced while working on this project was the fact that I was putting together several very independent codebases- the drone simulator code that models flying a quadrotor simulator but does not account for physical properties like wind turbulence and aerodynamic factors that would play a role in real life, and the code that models mathematical Dryden models for turbulence and blade flapping. Working around this involved a lot of debugging in C++ and ROS, and digging into functions to find ways to manipulate them to be more generalizable and easily maintainable in future.

******
-------