# MPPC
In this repo a model predictive path following controller according to <a href="https://arxiv.org/pdf/2003.04882.pdf" target="_blank">this paper</a> was implemented for the <a href="https://ethz.ch/content/dam/ethz/special-interest/itet/center-pbl-dam/documents/projects/F1TENTHFlyer.pdf" target="_blank">F1TENTH racingstack</a> of ETH Zurich. 

\
The main branch is using a pacejka tire model to simulate the cars physics.

# Setup
- install ros-noetic and f110 base system
- clone repo into catkin ws
- install python requirements by running 'pip install -r requirements.txt'
- use 'catkin build' to compile ros packages
- source the setup file if not done automatically 'source ~/catkin_ws/devel/setup.bash'
- start mpcc node by running 'roslaunch mpcc_ros mpcc_controler.launch'

# Results
This work resulted in a ROS node that was enabling the racing car to reach speeds up to 6 m/s while racing autonomously. 

<img src="https://github.com/patricpa/f110-mppc/docs/mpc-curv-result.png" width="700" />