# ROS_Drone

--------------------------------
## About

** Rospy codes and nodes to control an AR.Drone 2.0 using ROS **

* ROS distro: Indigo
* AR.Drone 2.0
* Tested on Ubuntu 14.04 (ROS Indigo won't work in earlier versions) 

## Setup
--------------------------------

** Installation instructions ** 

1. Create a catkin workspace for the simulator


    
```
#!bash

mkdir -p tum_simulator_ws/src
cd  tum_simulator_ws/src
catkin_init_workspace
```

2. Clone this repository

```
#!bash

git clone https://bitbucket.org/rafaelmd/ros_ardrone
```

3. Catkin make (can take a few minutes)

```
#!bash

cd ..
catkin_make
```

4. Source the environment

```
#!bash

source devel/setup.bash
```


## How to start
--------------------------------

** How to start the Ar.drone simulator controlled by keyboard ** 

1. If environment is not sourced yet:

```
#!bash

source devel/setup.bash
```

2. Start a simulation: drone controlled by keyboard
```
#!bash

roslaunch ardrone_tutorials keyboard_controller_simu.launch
```

3. Control the drone using the keyboard:

* Y = take-off
* H = land
* W = turn left
* R = turn right
* S = fly left
* F = fly right
* E = move forward
* D = move backward
* Q = fly up
* A = fly down


## Credits and references
--------------------------------

1. Tum simulator ported for ROS-Indigo
https://github.com/dougvk/tum_simulator

2. Packages to control the drone using keybord and joystick
https://github.com/mikehamer/ardrone_tutorials