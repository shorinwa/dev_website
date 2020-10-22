---
title: Adaptive Trust in Multi-Robot Coverage Control
image: exp6214_init.jpg
blurb: "We design multi-agent control algorithms that are robust to failures and performance degradation of individual agents, as well as algorithms that are invulnerable to the actions of adversarial agents and hazardous environments."
type: planning-controls
featured: false
youtube: https://www.youtube.com/watch?v=qyYt3frZ7aw
date: 2015-06-18
---

This work aims to design multi-agent control algorithms that are robust to failures and performance degradation of individual agents, as well as to design algorithms that are invulnerable to the actions of adversarial agents and hazardous environments.
 
For example, consider a multi-robot sensing scenario in which robots are controlled to spread out over an environment to sense a field of interest. The robots have some performance variations, and do not know beforehand the relative strengths of their performance compared to the others in the team. We present an algorithm that learns the relative performance variations in a distributed fashion, and automatically compensates by giving the weak robots a smaller portion of the environment, and the stronger robots a larger portion. The key to this algorithm is to quantify inter-agent trust through a "trust weighting," which is adapted on line in response to performance variations among the robots. Using a Lyapunov-type proof, we show the robots converge to locally optimal positions for coverage. We demonstrate our algorithm in both Matlab simulations and experiments with Pololu m3pi mobile robots.
 
The video below is a part of our 2015 ICRA paper on actuation-based performance variations.