---
layout: page
title: About this Demo
subtitle: Browser is what you need
---

# What is a monocular depth network?

A monocular depth network is (generally) a CNN able to infer 
the depth of the scene from a single image. We use a CNN because of the
complexity of this task.

# Why depth is important?
We can use depth information in many applications, such as Augmented Reality (AR),
3D Reconstruction, Collision Avoidance and many others.
We can obtain these data using *active sensors*, such as LiDAR or ToF, but also with passive ones like
stereo cameras. However, many devices do not have multiple cameras or active sensors, so monocular depth estimation
is attractive since it requires just a single camera. For many of these, (near) real time performances are necessary.

# What do I need to run a monocular depth network?
In general, you may need high performance devices, like a GPU, because many state-of-the-art networks
leverage million of parameters (eg 50 M, or even 100M). This means that they are not able to run with high FPS
on mobile or embedded devices. On the contrary, in this project we deploy a lightweight network, called **PyDNet** [avilable here](https://arxiv.org/pdf/1806.11430.pdf)
that is able to run directly on mobile devices.
We both developed a mobile application (for Android and iOS devices), but they have to been installed. Instead, in this demo, you can run the network on your device just using your
browser. Indeed, using [TensorFlow JS](https://www.tensorflow.org/js) the network runs inside the client device, and not in the remote server
