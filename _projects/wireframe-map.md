---
title: Wireframe Mapping for Resource-Constrained Robots
image: wireframe-map.png
blurb: "How can robots build and store maps well-suited to sparse environments? We propose a distributed algorithm for exploring and mapping a sparse environment under resource constraints."
type: perception
featured: true
date: 2019-11-01
---

We formulated a sparse map representation using an embedded labeled directed graph structure that compactly represents geometry as well as occlusions and frontier information. We tailored the particle filter framework to accommodate this map structure so each robot can incrementally updated and correct errors in its map. Finally, we developed a distributed algorithm to guide the exploration of the environment and enable the robots to verify shared information before it is accepted.
