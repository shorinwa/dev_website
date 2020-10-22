---
title: Virtual Rigid Bodies for Agile Coordination of Quadrotor Swarms and Human-Swarm Teleoperation
image: 
blurb: "We propose  a method for controlling a swarm of quadrotor micro aerial vehicles to perform agile interleaved maneuvers while holding a fixed relative formation, and transitioning between different formations."
type: planning-controls
featured: false
youtube: https://www.youtube.com/watch?v=9hKLZNA5kj4
date: 2015-08-11
---

This article presents a method for controlling a swarm of quadrotor micro aerial vehicles to perform agile interleaved maneuvers while holding a fixed relative formation, and transitioning between different formations. We propose an abstraction, called a Virtual Rigid Body, which allows us to decouple the trajectory of the whole swarm from the trajectories of the individual quadrotors within the swarm. The Virtual Rigid Body provides a way to plan and execute complex interleaved trajectories, and also gives a simple, intuitive interface for a single human user to control an arbitrarily large aerial swarm in real time. The Virtual Rigid Body concept is integrated with differential flatness-based feedback control to give a suite of swarm control tools. The paper also proposes a library architecture for a human operator to select between a number of pre-determined formations for the swarm in real time. Our methods are demonstrated in hardware experiments with a group of three quadrotors controlled autonomously, and five quadrotors teleoperated by a single human user.