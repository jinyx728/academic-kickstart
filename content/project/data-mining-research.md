+++
title = "Data Mining Research"
date = 2018-07-18T19:45:05+08:00
draft = false

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = []

# Project summary to display on homepage.
summary = "Data mining related research projects."

# Optional image to display on homepage.
image_preview = "data-mining.png"

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
I have several research experiences on data mining, which will be described below in detail.

## **Morphological Classification of Amazon Rainforest via Satellite Data**

I did this online research project of [School of Information](https://www.ischool.berkeley.edu), [UC Berkeley](https://www.berkeley.edu), advised by [Mike Tamir](https://www.ischool.berkeley.edu/people/mike-tamir). 

Around 30% of surface of Earth is covered by forests but many of them are suffering from deforestation which raises the concerns about forest, especially rainforest. As deforestations are mostly concentrated in rainforest, understanding the condition of rainforest is a global issue and a common way to monitor rainforest is remote sensing. In this project, images of Amazon rainforest captured by Planet company are used and our group chose the 3 band images to process. After building simple baseline model to analyse the result, directions for data preprocess and augmentation became clear. Then VGG-16 was chosen to perform and produce the final test score based on F2 evaluation.

In terms of technical details, we first conducted data pre-processing, including haze removal and data augmentation. Then we implemented data set extension, image contrast optimization and dimensionality reduction. After that, we compared the multi-label classification outcomes processed by MLP, shallow CNN and VGG-16 Network, and chose VGG-16 Network as the main classification method. Finally, we improved the VGG-16 Network details and achieved the F2 score of 0.90254 (world highest 0.93317 on Kaggle).

**Skills involved: Python, Numpy, Pandas, Keras, OpenCV**

## **Text Data Mining and Analysis of Enron Corporation Emails**

I did this research project at [Institute of Computing Technology](http://english.ict.cas.cn), [Chinese Academy of Sciences](http://english.cas.cn), advised by Ning Li.

The Enron Corporation is an American energy company, whose bankruptcy was caused by the Enron Scandal. Some of its mails, which are good materials for Text Mining, were made public by Federal Energy Regulatory Commission (FERC). In this project, we chose Python as the programming language, NLTK as the word segmentation tool, TF-IDF as the form of document vector, LDA and KMeans as clustering methods, and Gephi as the visualization tool. Through the above methods, we analyze the mail content of the main months of Enron Scandal, and we get some high frequency topics of every month. Successfully, we find that some topics and Enron Scandal itself are linked. Finally, by the form of pictures, we show the staff mail messaging relationship of high-frequency topics above.

In terms of technical details, we first conducted word splitting, lexical reduction of email title/body parts and converted all participles to the TF-IDF vectors. we then realized vectors clustering via LDA and K-means. Finally we plotted the relationship networks of senders and recipients via Gephi based on the email contents and clustering results.

**Skills involved: Python/JAVA, Numpy, Pandas, NLTK, Sklearn, Gephi**
