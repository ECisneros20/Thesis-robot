# Thesis-robot

## Description

This repository contains the virtual tests of the mobile robot developed in my thesis applying three autonomous navigation proposals from the following papers [1], [2], [3]. The world used in the three cases is the one provided by the Darpa Challenge [4].

## Installation

Open a new terminal and type the following path:

    cd ~/catkin_ws/src

To clone the most stable release into your workspace:

    git clone https://github.com/ECisneros20/Thesis-robot.git

To clone the latest release into your workspace:

    git clone -b release/1.0.0 https://github.com/ECisneros20/Thesis-robot.git

## Link transformations

Open a new terminal and type the following path:

    cd ~/catkin_ws/src/Thesis-robot

Run this command to get the tf references:

    rosrun tf2_tools view_frames.py

A pdf example is shown below:

<br/>
<p align="center">
  <img src="https://github.com/ECisneros20/Thesis-robot/assets/88266673/ed295abb-b24c-4d6c-beaa-e5694e6e0509" width="1200">
</p>

## Usage for virtual tests

### For the thesis_description package:

<table align="center">
  <tr>
    <th>Arg name</th>
    <th>Default value</th>
    <th>Package</th>
    <th>Other values</th>
  </tr>
  <tr>
    <td>world_name</td>
    <td>standard</td>
    <td>thesis_gazebo</td>
    <td>underground</td>
  </tr>
  <tr>
    <td>rvizconfig</td>
    <td>urdf</td>
    <td>thesis_description</td>
    <td>all, navigation, sensors</td>
  </tr>
  <tr>
    <td>show_gazebo</td>
    <td>false</td>
    <td>thesis_description</td>
    <td>true</td>
  </tr>
  <tr>
    <td>show_rviz</td>
    <td>false</td>
    <td>thesis_description</td>
    <td>true</td>
  </tr>
</table>

    roslaunch thesis_description spawn_robot.launch

### For the thesis_teleop package:

<table align="center">
  <tr>
    <th>Arg name</th>
    <th>Default value</th>
    <th>Package</th>
    <th>Other values</th>
  </tr>
  <tr>
    <td>joy_config</td>
    <td>logitech</td>
    <td>thesis_teleop</td>
    <td>keyboard, ps4</td>
  </tr>
</table>

    roslaunch thesis_teleop teleop.launch

## Next steps

- Create the ROS packages.

- According to the new changes, complete the Usage section.

## License

MIT License

## References

[1] C. Zheng, Q. Zhu, W. Xu, X. Liu, Q. Guo and F. Zhang, "FAST-LIVO: Fast and Tightly-coupled Sparse-Direct LiDAR-Inertial-Visual Odometry," <em>2022 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)</em>, Kyoto, Japan, 2022, pp. 4003-4009, doi: 10.1109/IROS47612.2022.9981107.

[2] 

[3] 

[4] 

[5] <a href = "https://automaticaddison.com/naming-and-organizing-packages-in-large-ros-2-projects/">Naming and Organizing Packages in Large ROS 2 Projects</a>
