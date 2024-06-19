+++
title = "Robust Realtime Shape Estimation of Deformable Linear Object"
subtitle = "ICRA 2024"
author = "Jiaming Zhang"
paper_author = [{name = "Jiaming Zhang,", me=true},
                {name = "Zhaomeng Zhang,", me=false},
                {name = "Yihao Liu,", me=false},
                {name = "Yaqian Chen,", me=false},
                {name = "Amir Kheradmand,", me=false},
                {name = "and Mehran Armand", me=false}]

date = "2024-05-13"
weight = 1
categories = ["technical","guide"]
tags = ["ICRA 2024","CV","Tracking"]
menu = "main:posts"
#draft = "true"
plotly = "true"
image = "/images/ICRADemo2024.gif"

+++

## Deformable Object Simulation

![Deformable Object Simulation](/images/ICRADemo2024.gif)

 The existing methods of shape estimation of continuum objects create dense point clouds from camera images, and/or use distinguishable markers on a deformable body. They have natural limitations in realtime tracking of large continuum objects/manipulators and the physical occlusion of markers can often compromise accurate shape estimation. We propose a robust method to estimate the shape of linear deformable objects in realtime using scattered and unordered key points. By utilizing a robust probability-based labeling algorithm, our approach identifies the true order of the detected key points and then reconstructs the shape using piecewise spline interpolation. The proposed method is implemented in C++ and integrated with ROS. The code is available [here](https://github.com/jmz3/DeformableEstimation).