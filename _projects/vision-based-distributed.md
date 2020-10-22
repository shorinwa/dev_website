---
title: Vision-Based Distributed Formation Control without an External Positioning System
image: visionformationcontrol.jpg
blurb: "We presented a fully distributed solution to drive a team of robots to reach a desired formation in the absence of an external positioning system that localizes them."
type: planning-controls
featured: true
youtube: https://www.youtube.com/embed/vBJDycZrXQ0
date: 2015-07-06
---

In this work [1], we presented a fully distributed solution to drive a team of robots to reach a desired formation in the absence of an external positioning system that localizes them. Our solution addresses two fundamental problems that appear in this context. First, we proposed a three dimensional distributed control law, designed at a kinematic level, that uses two simultaneous consensus controllers, one to control the relative orientations between robots, and another for the relative positions. The convergence to the desired configuration is shown by comparing the system with time-varying orientations against the equivalent approach with fixed orientations, showing that their difference vanishes as time goes to infinity. Secondly, in order to apply this controller to a group of aerial robots, we combined this idea with a novel sensor fusion algorithm to estimate the relative pose of the robots using on-board cameras and information from the Inertial Measurement Unit. The algorithm removes the influence of roll and pitch from the camera images, and estimates the relative pose between robots using a structure from motion approach. Simulation results, as well as hardware experiments with a team of three quadrotors, demonstrate the effectiveness of the controller and the vision system working together. 

In our experimental results, we outfitted three KMel k500 quadrotors with downward facing IP cameras that were capable of streaming a 640x480 video stream at 30 frames per second. The implementation of the image processing and the computation of the kinematic inputs has been done using ROS and OpenCV. The latter library includes all the necessary functions for the image processing, whereas ROS [2] greatly simplifies communication and synchronization issues that appear when working with multiple robots. For each quadrotor there is a dedicated node in charge of processing the images of that quadrotor, extracting and publishing the SIFT descriptors [3] to the neighboring quadrotors. Each node then computes a relative homography from its own and its neighbor's SIFT descriptors and uses the result to estimate the relative position between neighbors. An example of this process is shown in Figure 1 (left) while an example mosaic of the feature matching and pose estimation is shown in Figure 1 (right). The image processing and formation control computation together executes in a loop at 2Hz on this system. The kinematic commands are sent to a different computer where the low-level motion control of all the quadrotors is done using differential flatness.

The experiment shown in the video below uses this technique to control the three quadrotors from some initial conditions at various alititudes to a triangle formation on a plane parallel to the ground. Then the quadrotors form a different triangle formation before concluding in a perfect line formation. Figure 2 illustrates the three formations obtained in this experiment.

[1] E. Montijano, E. Cristofalo, D. Zhou, M. Schwager, and C. Sagues. Vision-based Formation Control without an External Positioning System. IEEE Transactions on Robotics. Submitted June 2015.
 
[2] M. Quigley, K. Conley, B. Gerkey, J. Faust, T. Foote, J. Leibs, R. Wheeler, and A. Y. Ng. ROS: an open-source Robot Operating System. In ICRA workshop on open source software, volume 3, 2009.
 
[3] D. Lowe. Distinctive image features from scale-invariant keypoints. International Journal of Computer Vision, 60(2):91–110, 2004.