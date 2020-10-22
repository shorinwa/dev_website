---
title: Multi-Robot Manipulation without Communication
image: zijian-square.jpg
blurb: "We present novel algorithms that allow a large number of small robots to move a comparatively large object to a goal location."
type: planning-controls
featured: true
youtube: https://www.youtube.com/embed/4nLMYjqUoJ4, https://www.youtube.com/embed/UitFri52EMI, https://www.youtube.com/embed/emZVxcl3Zg4
date: 2016-07-12
---

In this work, we present novel algorithms that allow a large number of small robots to move a comparatively large object to a goal location. The algorithm does not require an explicit communication network among the robots. Instead, the robots coordinate their actions through sensing the motion of the object itself. It is proven that this implicit information is sufficient to synchronize the forces applied by the robots. A leader (either a robot or human) then steers the forces of the synchronized group to manipulate the object through the desired trajectory to the goal. Our algorithms are proven to control both translational and rotational motion of the object.
 
Our idea was first published in [1], where the consensus-based algorithm incorporates velocity and acceleration measurements to achieve the force consensus among robots without communication. The algorithm was verified through simulations with up to 1000 robots carrying a heavy piano of realistic dimensions. We also analyzed the case in [2] where robots take heterogenous velocity and acceleration measurements at their local attachment points. A kinematic force coordination algorithm that only requires velocity measurement was proposed in [3], and validated by physical experiments using 4 custom built robots equipped with force and velocity sensors. A unified framework for a class of communication-free force coordination controllers was characterized in [4]. In addition, we also looked at the distributed rotation control without communication [5], where robots can contribute torque inputs by measuring the angular velocity.  This approach was also validated in real time using four custom designed omnidirectional robots, called OuijaBot. 


[1] Zijian Wang and Mac Schwager. "Multi-robot manipulation without communication." In Distributed Autonomous Robotic Systems (DARS), pp. 135-149. (2014)
 
[2] Zijian Wang and Mac Schwager. "Multi-robot manipulation with no communication using only local measurements." In 54th IEEE Conference on Decision and Control (CDC), pp. 380-385. (2015)
 
[3] Zijian Wang and Mac Schwager. "Kinematic multi-robot manipulation with no communication using force feedback." In IEEE International Conference on Robotics and Automation (ICRA), pp. 427-432. (2016)
 
[4] Zijian Wang and Mac Schwager. “Force-Amplifying N-Robot Transport System (Force-ANTS) for Cooperative Planar Manipulation without Communication.” International Journal of Robotics Research, vol. 35, no. 13, pp. 1564-1586 (2016).
 
[5] Zijian Wang, Guang Yang, Xuanshuo Su, and Mac Schwager. “OuijaBots: Omnidirectional Robots for Cooperative Object Transport with Rotation Control using No Communication.” In Distributed Autonomous Robotic Systems (DARS). (2016).
