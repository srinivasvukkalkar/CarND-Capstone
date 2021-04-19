# System Inegration - Self Driving car - Capstone Project

[image1]: ./images/System_Architechture.png "System_Architechture"
[image2]: ./images/Simulator_1.png "Simulator_1"
[image3]: ./images/Simulator_2.png "Simulator_2"

This is the project repo for the final project of the Udacity Self-Driving Car Nanodegree: Programming a Real Self-Driving Car. For more information about the project, see the project introduction [here](https://classroom.udacity.com/nanodegrees/nd013/parts/6047fe34-d93c-4f50-8336-b70ef10cb4b2/modules/e1a23b06-329a-4684-a717-ad476f0d8dff/lessons/462c933d-9f24-42d3-8bdc-a08a5fc866e4/concepts/5ab4b122-83e6-436d-850f-9f4d26627fd9).

The project is to program a self driving car (Carla) to drive around a highway using ROS Nodes including control and waypoint following. The following is a system architecture diagram showing the ROS nodes and topics used in the project.


![alt text][image1]

## The project runs with ROS and is divided into the following modules :

1. tl_detector uses the camera to detect the traffic lights' color
2. twist_controller handles the control of the car
3. waypoint_follower makes sure the car follow the trajectory
4. waypoint_loader loads the route the car is going to follow
5. waypoint_updater adapts the car's route to the situation (eg. traffic light)

## For this project I have used project workspace provided by Udacity. To run the program use the following commands
Make and run styx
```bash
cd ros
catkin_make
source devel/setup.sh
roslaunch launch/styx.launch
```
Run the simulator

![alt text][image2]


![alt text][image3]
