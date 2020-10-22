---
title: A Distributed Algorithm for Mapping the Graphical Structure of Complex Environments with a Swarm of Robots 
image: mapping-graph-structure.png
blurb: "This project proposes an algorithm that guarantees each robot’s local graphical map will converge upon the environment's true structure."
type: perception
featured: false
youtube: https://www.youtube.com/watch?v=6bTXm2m0GiM
date: 2017-03-15
---

Distributed algorithms offer several advantages over centralized approaches due to scalability, robustness, and efficiency. To help achieve these benefits, individual robots should be designed with minimalistic capabilities. Mapping an environment is an example of a task that benefits from multi-robot approaches, but requires storing large amounts of data.

This project seeks to uncover the graphical representation of an environment, which is significantly less memory intensive than a metric map. The robots can communicate with each other when within a certain radius, know their own locations, and can detect obstacles only through an extremely short-range sensor (e.g. a bump sensor).

This project proposes an algorithm that guarantees each robot’s local graphical map will converge upon the environment's true structure. To do this the robots follow the perimeters of their islands, merging maps when they come within communication range of other robots. They deviate from their paths when a new robot is within communication range and use a modified bug path following algorithm to determine if the newly discovered robot is on the same island.