
# QuadCopter Simulation in Gazebo and ROS

The "Quadcopter Simulation in Gazebo and ROS" repository offers a comprehensive environment for simulating quadcopters within the Gazebo simulation platform, integrated with the Robot Operating System (ROS). This simulation environment provides a realistic representation of quadcopter dynamics and behavior, allowing for the development and testing of various control algorithms, navigation strategies, and sensor integration techniques. Within this simulation, a range of sensors is available, including a 3D LiDAR for environment perception, a camera for visual data acquisition, an Inertial Measurement Unit (IMU) for attitude estimation, a GPS for localization, and a range finder for altitude sensing. These sensors collectively enable the quadcopter to perceive its surroundings, navigate autonomously, and perform tasks such as mapping, localization, and path planning. By leveraging this simulation environment, researchers and developers can iteratively refine and optimize quadcopter algorithms and systems in a cost-effective and safe manner before deployment in real-world scenarios.

# Prerequisite Installation
- [Ubuntu 20.04]()
- [ROS Neotic]()

# Installation
- First update and upgrade the System (Ubuntu 20.04).
```bash
  sudo apt update
  sudo apt upgrade
```

- Installation of packages
``` bash
sudo apt-get install ros-noetic-gazebo-ros-pkgs ros-noetic-gazebo-ros-control ros-noetic-ros-control ros-noetic-ros-controllers
sudo apt-get install ros-noetic-joint-state-controller ros-noetic-effort-controllers ros-noetic-position-controllers
```
# configuring the workspace

open a Terminal

- Initiate a workspace in your home directory
```bash
source /opt/ros/noetic/setup.bash 
```
- make a workspace with the name of your choice
``` bash
mkdir -p ~/drone_ws/src
cd ~/drone_ws/src
catkin_init_workspace
```

- Perform catkin make
``` bash
cd ~/drone_ws
catkin_make
```

- source the workspace
``` bash
source ~/drone_ws/devel/setup.bash
```

- Clone the repository in the source directory of the workspace
```bash
cd src
git clone https://github.com/pratik7229/Quadcopter_Simulation.git
```
- move back to the origin of workspace and perform catkin make
``` bash
cd ..
catkin_make
```
# Follow the Youtube Video 




