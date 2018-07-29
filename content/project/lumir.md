+++
title = "Lumir"
date = 2018-07-18T19:40:33+08:00
draft = false

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = []

# Project summary to display on homepage.
summary = "A software that provides numerous image processing algorithms."

# Optional image to display on homepage.
image_preview = "lumir.png"

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
Lumir is the course project of *SE342-Computer Vision*. It is written in C++, using Qt framework.

Lumir provides various image processing algorithms. **All of the algorithms are written by myself**, without using libraries like OpenCV. Supported algorithms are listed below:

* RGB channel seperation
* RGB to GRAY
* Hue/Saturation/Value adjustment
* Binarization (Otsu algorithm or double threshold)
* Rotation/Scaling (nearest neighbor interpolation or bilinear interpolation)
* Image add/minus/multiply operation
* Clipping
* Contrast adjustment (piecewise linear, exponent, logarithm or histogram equalization)
* Smoothing filter (mean filter, gaussian filter or median filter)
* Edge detection (Sobel operator, Laplace operator or Canny operator)
* Hough transform (detect line or circle)
* Binary morphology (dilation, erosion, open, close, thinning, thickening)
* Distance transform
* Skeleton extraction and reconstruction
* Grayscale morphology (dilation, erosion, open, close)
* Watershed algorithm

[Github link](https://github.com/jinyx728/SE342-Computer-Vision) for source code.

**Skills involved: C++, Qt, OpenCV(no algorithms used)**