+++
title = "Animal Gait Generation"
date = 2018-10-08T19:10:00+08:00
draft = false

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = []

# Project summary to display on homepage.
summary = "Optimal gait and form for animal locomotion."

# Optional image to display on homepage.
image_preview = "animal-gait.png"

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
I did this research project at State Key Lab of CAD/CG, Zhejiang University, advised by Weiwei Xu.

I developed a system that could automatically generate gait and form given an animal skeleton. I referred the method proposed in [Optimal Gait and Form for Animal Locomotion](http://grail.cs.washington.edu/projects/animal-morphology/s2009/). Given the mass of different parts of the animal, I used a objective function as a inner loop and a sample based optimization method as a outer loop. The inner loop penalized joint torque, joint velocity and head motion. I used SQP optimization method to solve this constrained non-linear optimization problem. The outer loop optimized foot contact time. I used basin-CMA to solve this sample based optimization problem.

All the codes are written in C++. I used rigidbody simulation library, SQP library to implement this system. This system is still under developing. I plan to first use automatic differentiation techniques to compute derivatives, then compute derivatives manually.

**Skills involved: C++, Rigidbody Simulation, SQP, Automatic Differentiation**