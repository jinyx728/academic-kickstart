+++
title = "Human Shape and Pose Modelling"
date = 2018-07-18T19:43:12+08:00
draft = false

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = []

# Project summary to display on homepage.
summary = "Simultaneous visual recovery of 3D human pose and shape."

# Optional image to display on homepage.
image_preview = "human-shape.png"

# Optional external URL for project (replaces project detail page).
external_link = ""

# Does the project detail page use math formatting?
math = false

# Does the project detail page use source code highlighting?
highlight = true

# Featured image
# Place your image in the `static/img/` folder and reference its filename below, e.g. `image = "example.jpg"`.
[header]
image = ""
caption = ""

+++
This research project is the PRP research project of [Shanghai Jiao Tong University](http://en.sjtu.edu.cn). I did this project at [VisionLab](http://www.visionlab.sjtu.edu.cn), advised by [Xu Zhao](http://www.automation.sjtu.edu.cn/en/ShowPeople.aspx?info_id=505&info_lb=326&flag=224).

We developed a system that automatically generate a 3D human model with pose and shape from a single RGB image. We then used this technique to develop an application: automatically measure the BWH of a person from a photo. Detailed procedure is:

* Capture the photo of a person with a plotting scale.
* Use the method describe in [*Realtime Multi-Person 2D Pose Estimation using Part Affinity Fields*](http://openaccess.thecvf.com/content_cvpr_2017/html/Cao_Realtime_Multi-Person_2D_CVPR_2017_paper.html) to extract the 2D human pose in real-time.
* Use the method describe in [*Keep it SMPL: Automatic Estimation of 3D Human Pose and Shape from a Single Image*](https://link.springer.com/chapter/10.1007/978-3-319-46454-1_34) to fit a 3D human model with pose and shape to the 2D pose.
* measure the BWH of the human model, and calculate the BWH of the person using the plotting scale.

I am the **team leader** of this project.

**Skills involved: Python, Caffe, OpenPose, SMPLify**