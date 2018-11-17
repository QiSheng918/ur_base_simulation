# This package run a simulation in the gazebo in which ur robot is on the AGV car.
# You can control the UR robot in the moveit and publish velocity msgs to control the AGV car


in order to run the simulation,you can type the following lines of code in the terminal
```
$ roslaunch ur_base_simulation ur10_base_simulation.launch
```

if you want to move the AGV car,you can type the following lines of code in the terminal. keep in mind change the frame in the Rviz to /odom,you can see the AGV car move in the Rviz and Gazebo

```
$ rostopic pub /cmd_vel geometry_msgs/Twist '{linear:[1,1,0],angular:[0,0,1]}' 
```



