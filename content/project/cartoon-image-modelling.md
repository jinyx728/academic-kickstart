+++
title = "Cartoon Image Modelling"
date = 2018-07-18T21:00:15+08:00
draft = false

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = []

# Project summary to display on homepage.
summary = "An interactive cartoon image modelling system via AR."

# Optional image to display on homepage.
image_preview = "cartoon-model.png"

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
I do this research project at [Digital ART Lab](http://dalab.se.sjtu.edu.cn/www/home/), advised by [Xubo Yang](http://dalab.se.sjtu.edu.cn/www/home/?page_id=17).

Cartoon image modelling is an interesting topic both in academia and industry. Once this technique becomes mature, children can easily model their hand-drawn cartoon character and see their character move and dance vividly via an AR application. However, current modelling method simply dilates the image to a 3D model and adds an NPR shader, which only works on limited cartoon images and requires manual configuration of joints of the character.

We decide to add semantic information to the modelling process. First, we do semantic classification and segmentation to the cartoon image, using a customized deep neural network trained on a dataset we built. Then, we model the image using classification and segmentation information, and generate skeleton (with limbs and joints) automatically. Finally, we attach pre-defined animation and sound to make the character move and dance.

This research project is still in progress. We have built a cartoon image dataset and a DNN-based semantic classification system. See [*ToonNet: A cartoon image dataset and a DNN-based semantic classification system*](/) for detail. we are currently experimenting modelling the cartoon image interactively using classfication and segmentation information.

