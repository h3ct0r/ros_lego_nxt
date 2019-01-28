
<h1 align="center">
<br>
<img src ="https://avatars0.githubusercontent.com/u/32429642?v=4&s=100" />
<br>
NXT ROS - Robots
<br>
</h1>

This repository contains all you need to get started with NXT ROS. You will find here a demo robot, including the building instructions and URDF model for visualization.

## Installation

The repository is expected to be used as the source folder of a working catkin environnement.

```
mkdir nxt_robots
cd nxt_robots
git clone https://github.com/NXT-ROS/nxt_robots.git src
catkin init
catkin build
```

You now have a working package with the demo robot ready to roll.

## Using NXT Robots

The robot package needs the core NXT ROS package to be properly loaded in order to work, more information on this [here](https://github.com/NXT-ROS/nxt).

As for any catkin package, you first need to add its folders to your environnement (make sure to select the correct file for your system).

```
cd nxt_robots
source devel/setup.(bash|sh|zsh)
```

You can then start ros with the provided launch file:

```
roslaunch nxt_robots_gyro_car robot.launch
```

You can then visualize it using rviz:

```
rosrun rviz rviz
```

## Credits

Original maintainer of the project and designer of the robot is [Melonee Wise](https://github.com/mmwise).