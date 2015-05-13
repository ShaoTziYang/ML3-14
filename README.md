#ML3-14
Final year project of the Hong University of Science and Technology, 2015 department of ELEC group ML3-14, please contact TziYang for any issues( tziyangshao@gmail.com). This repository is created for the convenience of anyone who are willing to continue the work and expand the possibilities.
##Objective
This project was aimed to create a software framework that enables Simultaneous Localization and Mapping( A.K.A. SLAM) with multiple robots on a median level laptop. The entire framework is established on Robot Operating System( A.K.A. ROS, link http://www.ros.org/).
##Related Libraries
This framework mainly consists of two SLAM methods, a monocular density SLAM called *LSD-SLAM[1]*, and a visual-based topological SLAM called *FAB-MAP[2]*. Point cloud obtained are filtered with the help of implementation in the Point Cloud Library, *PCL[3]*.  
*[1] LSD-SLAM: Large-Scale Direct Monocular SLAM, J. Engel, T. Schöps, D. Cremers, ECCV '14*  
*(link http://vision.in.tum.de/research/lsdslam)*  
*[2]  FAB-MAP,Accelerated Appearance-Only SLAM,M. Cummins, P. Newman, ICRA '08*  
*(link http://www.robots.ox.ac.uk/~mjc/Software.htm)*  
*[3] Point Cloud Library (link http://www.pointclouds.org/)*  
##System Flow  
###Hardware  
The framework aimed to realized multiple robot SLAM on a median level laptop. The hardware structure of a robot is: a median level laptop, a turltebot( link http://www.turtlebot.com/), and a calibrated camera. The setup of the turtlebot system on ROS can be find on the tutorial section of official page( link http://wiki.ros.org/Robots/TurtleBot), and also the calibration of camera( link http://wiki.ros.org/camera_calibration/Tutorials/MonocularCalibration). In our project, we tried omni-directional camera and fish eye camera since it is very easily for LSD-SLAM to loose track of the images once there is insufficient overlapping. Using cameras with larger field of view can solve it problem.
###Sofware  
####Turtlebot  

####Central Computer
