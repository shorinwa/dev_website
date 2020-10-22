---
title: Cooperative Multi-Quadrotor Pursuit of an Evader in an Environment with No-Fly Zones
image: cooperative-pursuit.jpg
blurb: "We investigate the cooperative pursuit of an evader by a group of quadrotors in an environment with no-fly zones."
type: planning-controls
featured: false
youtube: https://www.youtube.com/watch?v=rwCT3mzQ-HU
date: 2015-09-14
---

We investigate the cooperative pursuit of an evader by a group of quadrotors in an environment with no-fly zones. While the pursuers cannot enter into no-fly zones, the evader may freely move through zones to avoid capture. Once the evader enters a no-fly zone, the pursuers calculate a reachable set of evader positions. Using tools from Voronoi-based coverage control applied to the evader's reachable set, we provide an algorithm that distributes the pursuers around the zone's boundary and minimizes the capture time once the evader leaves the no-fly zone. Robust model predictive control (RMPC) tools are used to control the quadrotors and to ensure that they always remain in free space. We demonstrate the performance of our proposed algorithms through a series of experiments on KMEL Nano+ quadrotors.
 
This paper was a finalist for the Best Conference Paper Award at ICRA 2016.