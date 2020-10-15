---
title: Intercepting Rogue Robots - An Algorithm for Capturing Multiple Evaders with Multiple Pursuers
image: intercepting-robots.jpg
blurb: "We propose a distributed algorithm for the cooperative pursuit of multiple evaders using multiple pursuers in a bounded, convex environment."
type: planning-controls
featured: true
youtube: https://www.youtube.com/watch?v=70vRPfSbbv0
date: 2016-09-16
---

We propose a distributed algorithm for the cooperative pursuit of multiple evaders using multiple pursuers in a bounded, convex environment. The algorithm is suitable for intercepting rogue drones in protected airspace, among other applications. The pursuers do not know the evaders' policy, but by using a global "area-minimization" strategy based on a Voronoi tessellation of the environment, we guarantee the capture of all evaders in finite time. We present a decentralized version of this policy applicable in 2D and 3D environments, and show in multiple simulations that it outperforms other decentralized multi-pursuer heuristics. Experiments with both autonomous and human-controlled robots were conducted to demonstrate the practicality of the approach. Specifically, human-controlled evaders are not able to avoid capture with the algorithm.