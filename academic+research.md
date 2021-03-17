---
layout: post
title: Academic and Research Projects 
permalink: /academic+research/
---
### Robotics, Science and Systems
This Spring, I am taking a RSS class where we program a racecar to perform tasks such as parking and wall following to demostrate robotics concepts like controls, path planning, simultaneous localization and mapping, and state estimation. Check out [my team's portfolio](https://github.mit.edu/pages/rss2021-3/website/) to see what we're working on now. 

********

### MIT SparkLab

I am currently working at [MIT SparkLab](http://web.mit.edu/sparklab/) in the AI Innovation Accelerator (AIIA) search-and-rescue intelligence branch as a lab assistant under Professor Luca Carlone.

The initial objective of my summer research was to leverage MaskRCNN for transfer learning in Kimera (an open-source real-time SLAM software) to generate semantic labels from the RGB images simulated through Flightgoggles. Eventually, the aim was to be able to replace Flightgoggles with real world images and get relatively accurate metric-semantic reconstruction.

This has since evolved into speed-testing and latency reduction of Kimera, while also testing different neural networks to find one whoose trainig data best aligns it for use on Flightgoggles simulations.

My action items so far have been:
* Setting up Kimera (Kimera-VIO-ROS + Kimera-Semantics + dependencies) and running Kimera on test datasets
* Getting ground truth per-pixel semantic labelling from Flightgoggles 
* Testing neural networks (eg MaskRCNN) to generate semantic labels from the RGB image
* Adding throttle nodes and reducing resolution of RGB input into Kimera to reduce the time it takes to get a reconstruction
* Integrating Kimera into the broader RL system- involves generalizing topic names and modifying broadcasting rates to account for different input/output buffers


*******

### MIT Aerospace Controls Lab

I worked at [MIT ACL](http://acl.mit.edu) as a lab assistant from January to May 2020 under Professor Jonathan How.

The objective of my research was to conduct testing and debugging of the lab simulator and to help expand it from a quad-rotor to a hex-rotor, which is the lab standard vehicle. I also sought to incorporate wind and air dynamic effects by combining the simulator code with air dynamics code drawn up by another lab member. I also worked on incorporating blade flapping effects into the simulator to factor for the elimination of disymmetry of lift. 

I left my position a lot more comfortable with C++, ROS and Linux systems. I also learnt key logical testing techniques, such as setting checks for variables that might sometimes have null values and are inputs for other functions which would cause unprecedented results down the line.  

A challenge I faced while working on this project was the fact that I was putting together several very independent codebases- the drone simulator code that models flying a quadrotor simulator but does not account for physical properties like wind turbulence and aerodynamic factors that would play a role in real life, and the code that models mathematical Dryden models for turbulence and blade flapping. Working around this involved a lot of debugging in C++ and ROS, and digging into functions to find ways to manipulate them to be more generalizable and easily maintainable in future.

******
-------