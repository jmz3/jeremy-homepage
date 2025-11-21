+++
title = "OpenIRIS: Eye Tracking Software for Vestibular and Oculomotor Research"
subtitle = "Software & Open-source"
author = "Jiaming Zhang"

date = "2025-09-01"
weight = 1
categories = ["technical","guide"]
tags = ["ROS","Endoscope","dVRK"]
#draft = "true"
plotly = "true"

[[links]]
label = "Code"
url = "https://github.com/jmz3/OpenIris"

+++

I contributed to the development of [OpenIRIS](https://github.com/jmz3/OpenIris). OpenIris is an adaptable, open-source framework for video-based eye-tracking, developed in C# with a modular design for plugin extension. It supports online and offline recording, binocular pupil tracking, and 3-D eye motion capture.

To be more specific, I added support for USB version of Flir Blackfly cameras, and implemented a online calibration module to calculate the head pose from gravitational vector recorded by an IMU.