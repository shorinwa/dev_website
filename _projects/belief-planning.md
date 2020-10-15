---
title: Belief Space Planning for Continuous-Time Dynamical Systems
image: belief-planning.png
blurb: "We propose a novel belief space planning technique for continuous dynamics by viewing the belief system as a hybrid dynamical system with time-driven switching."
type: planning-controls
featured: false
youtube:
date: 2018-01-01
---

We propose a novel belief space planning technique [1] for continuous dynamics by viewing the belief system as a hybrid dynamical system with time-driven switching. Our approach is based on the perturbation theory of differential equations and extends Sequential Action Control [2] to stochastic belief dynamics. The resulting algorithm, which we name SACBP, does not require discretization of spaces or time and synthesizes control signals in near real-time. SACBP is an anytime algorithm that can handle general parametric Bayesian filters under certain assumptions. We demonstrate the effectiveness of our approach in an active sensing scenario and a model-based Bayesian reinforcement learning problem. In these challenging problems, we show that the algorithm significantly outperforms other existing solution techniques including approximate dynamic programming and local trajectory optimization.

[1] Nishimura, H., Schwager, M.: SACBP: Belief Space Planning for Continuous-Time Dynamical Systems via Stochastic Sequential Action Control. The 13th International Workshop on the Algorithmic Foundations of Robotics (WAFR), Mérida, México (2018)

[2] Ansari, A.R., Murphey, T.D.: Sequential Action Control: Closed-Form Optimal Control for Nonlinear and Nonsmooth Systems. IEEE Transactions on Robotics 32(5), 1196–1214 (2016)