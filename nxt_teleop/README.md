
<h1 align="center">
<br>
<img src ="https://avatars0.githubusercontent.com/u/32429642?v=4&s=100" />
<br>
NXT ROS - Teleop
<br>
</h1>

This repository contains a keyboard interface to use with NXT ROS.

## Installation

The repository is expected to be placed inside the source folder of a working catkin environnement.

```
mkdir nxt_teleop
cd nxt_teleop
mkdir src
cd src
git clone https://github.com/NXT-ROS/nxt_teleop.git
cd ..
catkin init
catkin build
```

You now have a working package with the nxt_teleop package in it.

## Using NXT Teleop

The teleop package needs the core NXT ROS package to be properly loaded in order to work, more information on this [here](https://github.com/NXT-ROS/nxt).

As for any catkin package, you first need to add its folders to your environnement (make sure to select the correct file for your system).

```
cd nxt_teleop
source devel/setup.(bash|sh|zsh)
```

You can then start ros with the provided launch file:

```
roslaunch nxt_teleop teleop_keyboard.launch
```

## Credits

Original maintainer of the project is Wim Meeussen.