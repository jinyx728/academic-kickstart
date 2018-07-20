+++
title = "Neuron Simulation Engine"
date = 2018-07-18T19:20:06+08:00
draft = false

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = []

# Project summary to display on homepage.
summary = "An interactive VR application that simulates nerve impulse and inhibition."

# Optional image to display on homepage.
image_preview = "neuron-simulation.png"

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
Neuron simulation engine is the course project of *SE341-Game Designing and Programming*. We develop this engine using Unity and C# language.

This simulation engine allows user to create and delete neurons and build a neural network via HTC Vive headset. It can also simulate the process of nerve impulse and inhibition. Detailed features are listed below:

* Provides basic structures including sensors, effectors, excitatory neurons and inhibitory neurons. Users can customize the number of incoming and outgoing channels of neurons, such as the number of peripheral branches and the number of side branches.
* Allows users to build a neural network by freely choosing and moving different basic structures.
* Allows the user to set neuron parameters such as nerve impulse conduction time (from neuronal cell body to axon tip), neurotransmitter transmission time (from axon tip to next neuron cell body), nerve excitation/inhibition duration.
* Correctly simulates the effects of any neural networks in real-time, such as which effectors or neurons are excited and which are not. The conduction process of nerve impulses is visualized during the simulation.
* Allows real-time magnification observation of a neuron's axons, using particles to simulate the microscopic process of axons' nerve impulse conduction (substance exchange of sodium and potassium ions after nerve impulses pass).
* Allows real-time magnification observation of the peripheral branches/lateral branches of a neuron, using particles to simulate the microscopic processes of neurotransmitter transmission (neurotransmitters are produced from the peripheral branches/lateral branches, diffuse and bind to the next neuron)