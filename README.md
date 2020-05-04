# ROS_turtlebot_kf

## Overview
Applying a EKF ROS package to TurtleBot and visualizing the output on Rviz and Rqt multiplot.

## Build Instructions

**Catkin Workspace, cloning the repository **

Create a catkin workspace :
```
mkdir -p ~/catkin_ws/src
cd ~/catkin_ws/src
```

Cloning the repository
```
git clone --recursive https://github.com/amrish1222/ROS_turtlebot_kf.git
```
And move the turtlebot_kf folder to the src folder and delete the parent folder

Cloning the other depencies/ packages that are required
```
git clone https://github.com/turtlebot/turtlebot_simulator
git clone https://github.com/udacity/robot_pose_ekf
git clone https://github.com/udacity/odom_to_trajectory
git clone https://github.com/turtlebot/turtlebot
```

Build
```
cd ..
catkin_make
```

Setting the environment variables
```
source devel/setup.bash
```

## Running Instructions

```
roslaunch turtlebot_kf turtlebot_kf.launch
```
