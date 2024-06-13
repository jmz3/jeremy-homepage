+++
title = "About"
author = "Jiaming Zhang"
date = "2023-01-22"

+++

<!-- description = ""
aliases = ["about", "contact"]
slug = "contact" -->

# Bio

<img src="/images/IMG_0804.JPG" data-canonical-src="/images/IMG_0804.JPG" width="200"  align="right" style="padding-left: 40px; margin-bottom: 30px; margin-top: 30px; border-radius: 50%"/>

<!-- <img src="/images/IMG_0804.JPG" data-canonical-src="/images/IMG_0804.JPG" width="200"  align="right" style="margin-bottom: 30px; margin-top: 30px; border-radius: 50%"/> -->

Hello! My name is Jiaming (Jeremy) Zhang. I am a first-year Ph.D. student in Computer Sciecne at [The Johns Hopkins University](https://www.jhu.edu/). My reasearch focuses on the application of robotics in medical scenarios. Prior joining in Hopkins, I received my Bachelor degree in Mechanical Engineering from [Huazhong University of Science and Technology](https://www.hust.edu.cn/), where I graduated with honors. Afterwards, I obtained my Master's degree in Robotics at Hopkins. I was an intern engineer at Narwal Robotics and HUST-Wuxi Research Institute. During my leisure time, I enjoy playing tennis, cooking and reading. 


# Research Interest and Experience
As a robotics enthusiast with a strong interest in visual perception, motion planning, and medical robots, I have conducted research in various areas such as hand-eye calibration, LiDAR-based SLAM, exoskeleton design and analysis, AI-based medical image analysis, and medical robots. Thess experiences equip me with solid foundation for Mathematics, ROS development, Robot Hardware Design and the state-of-the-art Computer Vision models.

# Ongoing Project

Currently, I'm working as a research assisant in [BIOMECHANICAL AND IMAGE GUIDED SURGICAL SYSTEMS (BIGSS)](https://bigss.lcsr.jhu.edu/) laboratory under the supervision of [Prof. Mehran Armand](https://scholar.google.com/citations?user=0jQj6m4AAAAJ&hl=en), [Prof. Amir Kheradmand](), and [Prof. Alejandro Martin-Gomez](https://engineering.jhu.edu/faculty/alejandro-martin-gomez/). Here are the projects that I'm carrying out.

- [Deformable Object Simulation](#deformable-object-simulation)
- [Robot TMS](#robot-tms)
- [Position-based Visual Servoing](#position-based-visual-servoing)
- [Learning-based 2D/3D Fluoroscopic Image Registration](#learning-based-2d/3d-fluoroscopic-image-registration)
- [3D Slicer Integration with Segment Anything Model, aka SAMM (Segment Any Medical Model)](#samm)

## Deformable Object Simulation

![Deformable Object Simulation](/images/ICRADemo2024.gif)

 The existing methods of shape estimation of continuum objects create dense point clouds from camera images, and/or use distinguishable markers on a deformable body. They have natural limitations in realtime tracking of large continuum objects/manipulators and the physical occlusion of markers can often compromise accurate shape estimation. We propose a robust method to estimate the shape of linear deformable objects in realtime using scattered and unordered key points. By utilizing a robust probability-based labeling algorithm, our approach identifies the true order of the detected key points and then reconstructs the shape using piecewise spline interpolation. The proposed method is implemented in C++ and integrated with ROS. The code is available [here](https://github.com/jmz3/DeformableEstimation).

## Robot TMS

<img src="/images/rotms.jpeg" data-canonical-src="/images/samme.png" alt="Robot TMS" align="right" style="width: 60%; padding-left: 50px; margin-bottom: 30px; margin-top: 0px"/>

With our advanced robotic system, surgeons can easily and accurately deliver non-invasive stimulations to the cortical area of the brain. The system is designed to be easy to use and can be operated by a single person. The system is currently being tested in a clinical trial at the Johns Hopkins Hospital. 

## Position-based Visual Servoing

## Learning-based 2D/3D Fluoroscopic Image Registration
We developed and maintained an open-source python package [xregi](https://github.com/jeremyzz830/xregi/tree/master) that is used to compute the projection matrix between 2D x-ray images and 3D CT scans. This process is also called as 2D/3D fluoroscopic image registration problem. The package is now available on Pypi. Install the pacakge through `pip install xregi` to try out!


## SAMM: Segment Any Medical Model

<img src="/images/samme.png" data-canonical-src="/images/samme.png" width="350"  align="left" style="padding-right: 40px; margin-bottom: 10px; margin-top: 10px"/>


I'm excited to announce that our project [SAMM](https://github.com/bingogome/samm) has received many attentions from all over the world! Please reach out if you want to collaborate. SAMM allows users to directly leverage the powerful Segment Anything Model (SAM) to segment medical images (including CT, MR, Ultrasound, and more) in 3D Slicer. 

<!-- <br></br> -->

## PoseHub: Surgical Tool Tracking with AR Headset
We are developing a surgical tool tracking system that can be used with augmented reality headsets. The system is designed to provide real-time feedback to the surgeon about the location of the surgical tool. The system has a scene-graph structure that allows for easy integration with different tracking devices and visualization tools. A synthetic dataset is generated in ROS to test the system. The code is available [here](https://github.com/jmz3/PoseHub.git)