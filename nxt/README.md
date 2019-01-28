
<h1 align="center">
<br>
<img src ="https://avatars0.githubusercontent.com/u/32429642?v=4&s=100" />
<br>
NXT ROS - Core
<br>
</h1>

Software stack containing all the required pieces to use Lego Mindstorms NXT with ROS

## Installation

### ROS package

The repository is expected to be used as the source folder of a working catkin environnement.

```
mkdir nxt
cd nxt
git clone --recursive https://github.com/NXT-ROS/nxt.git src
catkin init
catkin build
```

You now have all the required packages to run the ros-nxt core.

### NXT USB

In order to communicate with the NXT, you will need to set the correct permissions.

```
sudo groupadd lego
sudo usermod -a -G lego $(id -un)
echo "SUBSYSTEM=="usb", ATTRS{idVendor}=="0694", GROUP="lego", MODE="0660"" > /tmp/70-lego.rules && sudo mv /tmp/70-lego.rules /etc/udev/rules.d/70-lego.rules
```

You can now reboot your system and hook up your NXT.

## Dependencies

The nxt-ros packages depends on:

* ROS Kinetic
* Python 3
* NXT Python v3 (shipped as submodule)

## Using NXT ROS

As for any catkin package, you first need to add its folders to your environnement (make sure to select the correct file for your system).

```
cd nxt
source devel/setup.(bash|sh|zsh)
```

You can then start ros core and use any componnents of the nxt stack:

```
roscore
```