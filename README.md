# The EZGripper Overlay provides an updated URDF hierarchy for EZGrippers with the following features:

- Separation of ezgripper_palm and the mount

- Addition of double mount and triple mount to the meshes

- URDFs for the double and triple gripper mounts

This is not fully developed.  To be developed:

- further ezgripper_control files
- further ezgripper_gazebo files
- any ezgripper move_it! files


# INSTALLATION

make a directory AWAY FROM xxx.ws

cd into new directory

git clone https://github.com/SAKErobotics/ezgripper-overlay

cd ezgripper-overlay

cp -r ezgripper* ~/####_ws/src/EZGripper_ros2

cd ~/####_ws

colcon build

source install/setup.bash


# How to run an example EZGripper double

ros2 launch ezgripper_description ezgripper_double_display.launch.py
