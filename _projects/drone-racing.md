---
title: Game Theoretic Planning for Autonomous Drone Racing
image: drone-racing.jpg
blurb: "How should robots plan to compete? We propose a game theoretic planner which allows drones to reason online about their opponents' actions during race scenarios."
banner: /images/projects/msl_herd-4.jpg
keyword: Game Theoretic Planning
youtube: https://www.youtube.com/watch?v=ayPamTiUzvA, https://www.youtube.com/watch?v=589YHBMSFjQ
type: planning-control, perception
featured: true
date: 2020-09-16
---

We propose an online 3-D planning algorithm for a drone to race competitively against a single adversary drone.  The algorithm computes an approximation of the Nash equilibrium in the joint space of trajectories of the two drones at each time step, and proceeds in a receding horizon fashion. The algorithm uses a novel sensitivity term, within an iterative best response computational scheme, to approximate the amount by which the adversary will yield to the ego drone to avoid a collision. This leads to racing trajectories that are more competitive than without the sensitivity term. We prove that the fixed point of this sensitivity enhanced iterative best response satisfies the first-order optimality conditions of a Nash equilibrium. We present results of a simulation study of races with 2-D snd 3-D race courses, showing that our game theoretic planner significantly out-performs a Model Predictive Control (MPC) racing algorithm. We also present results of multiple drone racing experiments on a 3-D track in which drones sense each others' relative position with on-board vision. The proposed game theoretic planner again out-performs the MPC opponent in these experiments where drones reach speeds up to 1.25m/s
