---
title: Planning for Human-Robot Interaction
image: human-avoidance.png
blurb: "We combine risk-sensitive optimal control tools with deep generative modeling to enable robotic crowd navigation, and observe diverse interaction behavior by varying the robot's risk sensitivity."
type: planning-control
date: 2020-05-05
---

This work presents a novel online framework for safe crowd-robot interaction based on risk-sensitive stochastic optimal control, wherein the risk is modeled by the entropic risk measure. The control algorithm relies on mode insertion gradient optimization for this risk measure as well as Monte Carlo sampling from Trajectron++, a state-of-the-art generative model that produces multimodal probabilistic trajectory forecasts for multiple interacting agents.

Our modular approach decouples the crowd-robot interaction into learning-based prediction and model-based control, which is advantageous compared to end- to-end policy learning methods in that it allows the robot’s desired behavior to be specified at run time. In particular, we show that the robot exhibits diverse interaction behavior by varying the risk sensitivity parameter.

A simulation study and a real-world experiment show that the proposed online framework can accomplish safe and efficient navigation while avoiding collisions with more than 50 humans in the scene.
