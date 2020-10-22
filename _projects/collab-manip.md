---
title: Adaptive Control for Collaborative Manipulation
image: collab-manip.png
blurb: "How can robots work together to move unknown payloads? Using tools from adaptive control, we develop a distributed algorithm for collaborative manipulation without prior payload knowledge."
type: planning-control, perception
date: 2020-05-01
youtube: https://www.youtube.com/watch?v=qRoCpjAW5NY
---

Collaborative manipulation remains one of the most important problems in multi-agent systems. Using teams of robots to manipulate large or heavy payloads promises many advantages over single-agent manipulators, including flexibility, scalability, and robustness to individual agent failures. However, current strategies for manipulation often require exact knowledge of the payload and agents' attachment positions, which limits the applicability of these systems to real-world manipulation tasks.

In this work, we leverage adaptive control theory to design decentralized controllers for a team of robots performing collaborative manipulation. We formulate the dynamics for collaborative manipulation tasks in 2D and 3D, and develop control and adaptation laws that guarantee the stability and tracking of the payload's velocities. We verify these controllers both experimentally (using a team of ground robots) and in simulation.
