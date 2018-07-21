+++
title = "NPR Shader and Filter"
date = 2018-07-18T20:40:11+08:00
draft = false

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = []

# Project summary to display on homepage.
summary = "Non-Photorealistic Rendering shader and filter to create hand-drawn style image."

# Optional image to display on homepage.
image_preview = "shader.jpg"

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

This project includes an NPR shader and an NPR filer. These two algorithms developed by myself are directly used to augment the *ToonNet* dataset.

The NPR shader consists of two steps. First, it applies a shader similar to Blinn-Phong to the model. The shader calculates the ambient and diffuse color, and apply Half Lambert to the diffuse term. It also samples a 1D ramp texture using diffuse color, and multiply the sampled grayscale color to the output. Then, the shader postprocesses the shaded model using Sobel operator, which depicts the contour and makes the final image more realistic.

The NPR filter can change a common cartoon image to a hand-drawn style image. First it apply pencil or crayon textures to the grayscale cartoon image using [Lu's method](http://www.cse.cuhk.edu.hk/leojia/projects/pencilsketch/pencil_drawing.htm). Then it maps the color back using a certain equation. After mapping, the grayscale texture can be directly applied to the cartoon image
according to the color.

These two algorithms are successful to augment the *ToonNet* dataset. To learn these algorithms further, see [*ToonNet: A cartoon image dataset and a DNN-based semantic classification system*](/).