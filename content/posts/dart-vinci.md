+++
title = "dARt Vinci: Egocentric Data Collection for Surgical Robot Learning at Scale"
subtitle = "IROS 2025"
author = "Jiaming Zhang"
paper_author = [
    {name = "Yihao Liu,", me=false},
    {name = "Yu-Chun Ku,", me=false},
    {name = "Jiaming Zhang,", me=true},
    {name = "Hao Ding,", me=false},
    {name = "Peter Kazanzides,", me=false},
    {name = "and Mehran Armand", me=false}
]

date = "2025-03-01"
weight = 1
categories = ["technical", "paper"]
tags = ["IROS 2025", "AR", "Da Vinci", "Robot Learning"]
menu = "main:posts"
plotly = "true"
image = "/images/IROS2025.gif"
+++


<div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden;">
  <video autoplay loop style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;">
    <source src="/images/dart-vinci.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
</div>

<div style="margin-top: 1rem; text-align: center;">
  <a href="/pdfs/dart-vinci-paper.pdf" target="_blank">[PDF]</a>
  <a href="https://arxiv.org/abs/your-paper-id" target="_blank">[Arxiv]</a>
  <a href="https://your-project-website.com" target="_blank">[Website]</a>
  <a href="https://github.com/your-github-repo" target="_blank">[GitHub]</a>
</div>

Data scarcity has long been an issue in the robot learning community. Particularly, in safety-critical domains like surgical applications, obtaining high-quality data can be especially difficult. It poses challenges to researchers seeking to exploit recent advancements in reinforcement learning and imitation learning, which have greatly improved generalizability and enabled robots to conduct tasks autonomously. 

In this work, we introduce *dARt Vinci*, a scalable data collection platform for robot learning in surgical settings. The system uses AR hand tracking and a high-fidelity physics engine to capture subtle maneuvers in primitive surgical tasks: By eliminating the need for a physical robot setup and providing flexibility in terms of time, space, and hardware resources-such as multiview sensors and actuators-specialized simulation is a viable alternative. At the same time, AR allows the robot data collection to be more egocentric, supported by its body tracking and content overlaying capabilities. Our user study confirms the proposed system's efficiency and usability, where we use widely-used primitive tasks for training teleoperation with da Vinci surgical robots.

We believe that dARt Vinci can be a valuable tool for researchers to collect data at scale, enabling the development of more robust and generalizable robot learning algorithms.