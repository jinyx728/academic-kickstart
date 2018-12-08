+++
title = "Codimensional Fluid Simulation"
date = 2018-10-08T19:10:00+08:00
draft = false

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = []

# Project summary to display on homepage.
summary = "Codimensional fluid simulation by Closest Point Method."

# Optional image to display on homepage.
image_preview = "codim-fluid.png"

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
I am currently working on this research project advised by [Bo Zhu](http://www.dartmouth.edu/~boolzhu/index.html). This project is towards SIGGRAPH 2019.

We use closest point method (CPM, i.e. extending points on the surface to 3D space) to solve partial differential equation (PDE, like Navier-Stokes equations) on surface. We compute level set function from surface, solve Poisson equation on 3D grid, interpolate pressure and velocity value from closest points on the grid to surface, and calculate advection using particles on the surface. We also adopt non-manifold grid to handle situations where two surfaces are close to each other.

Still in progress ...

**Skills Involved: C++, OpenGL, GLFW, GLSL, Eigen, PDE, Numerical Methods**