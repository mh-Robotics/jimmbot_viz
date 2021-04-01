jimmbot_viz
===========

jimmBOT visualization package for the mhRobotics jimmBOT. Available launch files:

 - view_model.launch : Model visualization of jimmBOT with no controllers.
 - view_robot.launch : Robot visualization with sensors and controllers.

Instructions:

Model visualization can be launched standalone. Only RVIZ will be oppened and you can rotate wheels with GUI Joint State Publisher.

```bash
roslaunch jimmbot_viz view_model.launch
```

Robot visualization should be launched after the Simulation is started or Real robot is brought up. RVIZ will then be oppened and you can see the visualization of sensors and everything else either from Simulation or Real Robot.

Real robot
```bash
1. roslaunch jimmbot_bringup jimmbot_robot.launch
2. roslaunch jimmbot_viz view_robot.launch
```

Simulation
```bash
1. roslaunch jimmbot_gazebo jimmbot_empty_world.launch
2. roslaunch jimmbot_viz view_robot.launch
```