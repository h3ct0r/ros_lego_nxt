
<h1 align="center">
<br>
<img src ="https://avatars0.githubusercontent.com/u/32429642?v=4&s=100" />
<br>
NXT ROS - Viz
<br>
</h1>

This repository contains visualization plugins for the Lego color sensor and ultrasonic sensor for rviz.

## Installation

The repository is expected to be placed inside the source folder of a working catkin environnement.

```
mkdir nxt_viz
cd nxt_viz
mkdir src
cd src
git clone https://github.com/NXT-ROS/nxt_viz.git
cd ..
catkin init
catkin build
```

You now have a working package with the nxt_viz package in it.

## Using NXT Viz

The viz package needs the core NXT ROS package to be properly loaded in order to work, more information on this [here](https://github.com/NXT-ROS/nxt).

As for any catkin package, you first need to add its folders to your environnement (make sure to select the correct file for your system).

```
cd nxt_viz
source devel/setup.(bash|sh|zsh)
```

Next time you start rviz, you will find the new visualizers inside the list.

## Credits

Original maintainer of the project is David Butterworth.