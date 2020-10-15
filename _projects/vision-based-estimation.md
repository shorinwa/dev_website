---
title: Vision-Based Active Estimation for 3D Scene Reconstruction
image: activevisionsquare.jpg
blurb: "We  develop an autonomous multi-robot system of aerial vehicles with on-board cameras that is capable of actively reconstructing the three-dimensional (3D) pose and geometry of its environment."
type: planning-controls
featured: false
youtube: https://www.youtube.com/watch?v=8_kyeGNJCiY
date: 2014-12-11
---

The purpose of this research is to develop an autonomous multi-robot system of aerial vehicles with on-board cameras that is capable of actively reconstructing the three-dimensional (3D) pose and geometry of its environment. This approach computes a control action for the robot using the images from the on-board cameras such that the resulting 3D model is as accurate as possible. Imagine the ability to monitor any environmental feature at any given time with an autonomous, deployable network of aerial robots. Such a system could maneuver around a building, base, or infrastructure while producing an accurate 3D model for inspection. This system could have countless useful research applications, such as studying the effects of climate change on forests or searching for new archeological sites. In fact a proposed framework for completing the former task was submitted to the 2016 American Control Conference [1].
 
Recently, we submitted our first active-vision results to the 2016 International Conference on Robotics and Automation (ICRA) [2]. Here we proposed an online, active control strategy for estimating the three-dimensional structure of objects in a static environment by using a monocular camera mounted on an aerial robot. The pinhole camera model was used as the nonlinear measurement equation for the Extended Kalman Filter, which estimates the unknown depth of each 3D feature with respect to the camera’s current coordinate frame. The robot was actively controlled using an explicit expression for the gradient descent of the estimation error covariance at the next time step. The active technique was then abstracted into a simpler control strategy, which leads to circular trajectories as a function of image feature position. Finally, the two controllers were compared in simulations and in real-time experiments on a quadrotor with a downward facing camera. Our results suggest that moving a camera in a circular trajectory about the object of interest provides near-optimal reconstruction results in a filter-based estimation framework. The active control is computationally efficient and does not require a time consuming optimization in-the-loop, making it best suited for fast, online reconstructions onboard micro aerial vehicles.

In the past, we simulated the deterministic version of this active control by using a nonlinear observer technique proposed by Spica et al. [3]. The premise of this controller is to drive a 6 DOF camera such that the estimate of the unknown depth of a feature in the onboard image is minimized. Specifically, this can be achieved by maximizing the singular value of the matrix that linearly relates the unknown state (image feature depth) to the dynamics of the measured states (x and y feature position in the image). Further, we have implemented this approach when tracking multiple objects by actively maximizing the worst-case feature estimation at any given time step, rather than the average of the features as in Giordano et al. [4]. The results of these simulations are shown in the video below.

[1] H. Ding, E. Cristofalo, J. Wang, D. Castañon, E. Montijano, V. Saligrama, M. Schwager, “A Multi-Resolution Approach for Discovery and 3D Modeling of Archaeological Sites Using Satellite Imagery and a UAV-borne Camera,” 2016 IEEE American Control Conference, Submitted Sept 2015.

[2] E. Cristofalo, E. Montijano, and M. Schwager, “Active Vision-based Control for Fast 3D Reconstruction with an Aerial Robot,” 2016 IEEE International Conference on Robotics and Automation, Submitted Sept 2015.

[3] R. Spica, P. Giordano. A Framework for Active Estimation: Application to Structure from Motion. In IEEE Conference on Decision and Control, 2013.

[4] P. Giordano, R. Spica, F. Chaumette. An Active Strategy for Plane Detection and Estimation with a Monocular Camera. In IEEE International Conference on Robotics and Automation, 2014.