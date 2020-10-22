---
title: Game of Drones Competition 2019
image: game-of-drones.png
blurb: "A competition for users to develop autonomous drone racing perception and control algorithms to compete in a simulation framework."
type: planning-controls
featured: false
youtube: 
date: 2019-08-1
---

The Game of Drones competition was hosted at the 2019 NeurIPS Conference in collaboration with Microsoft Research. The goal of the competition was for users to develop autonomous drone racing perception and control algorithms to compete in a simulation framework: AirSim Drone Racing Lab. This simulated competition makes drone racing more accessible to roboticists by removing the need for expensive hardware.

The competition had three tiers, each focusing on different aspects of the drone racing problem. Tier 1 involved racing against an opponent with access to ground truth information. Tier 2 was a race against time, with no opponent, and only noisy estimates on gate poses. Tier 3 tested the challenges presented in both Tier 1 and Tier 2, and included an opponent without ground truth information on the opponent or the gates. More details about the competition can be found here. The methods used by the winning teams as well as other competition information can be found on the competition web page.

Baseline algorithms for Tier 1 and 2 were developed as a means for competitors to have a starting point for their own algorithms, and as a way to benchmark how their methods performed. The Tier 1 baseline algorithm included an iterative best response trajectory planning technique that is outlined here. The Tier 2 baseline algorithm used a perception algorithm that detected gates based on their colors and planar geometry.

An important outcome of this work is the drone racing framework AirSim Drone Racing Lab [1]. This framework provides race tracks, an opponent to race against, collision penalty counts, and other features that are important to the drone racing problem. AirSim Drone Racing Lab also makes the drone racing problem accessible to allow various research communities to collaboratively work on similar challenges from different approaches.

References

[1] R. Madaan et al., “AirSim Drone Racing Lab”, Journal of Machine Learning Research, Accepted, May 2020.
