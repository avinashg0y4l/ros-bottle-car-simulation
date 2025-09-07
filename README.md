# ROS Water Bottle Car Simulation

This is a simulation of a differential-drive robot modeled after a water bottle, as seen in the image below. The project is built for ROS Noetic and Gazebo and runs on Windows using WSL 2.

![Demonstration GIF](https://github.com/YourUsername/ros-bottle-car-simulation/blob/main/demo.gif)
*(This is a placeholder for a demonstration GIF which will be added after implementing sensors.)*

## Features
-   Custom robot model (URDF/XACRO) built with primitive shapes to match a real-world object.
-   Differential drive controller for teleoperation.
-   Pre-configured launch file for easy startup in Gazebo.

## How to Run
1. Clone this repository into your `catkin_ws/src` folder.
2. Build the workspace with `catkin_make`.
3. Launch the simulation: `roslaunch bottle_car_description spawn_bottle_car.launch`
4. In a new terminal, run the controller: `rosrun teleop_twist_keyboard teleop_twist_keyboard.py`