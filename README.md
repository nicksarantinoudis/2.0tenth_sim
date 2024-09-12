# 2.0tenth_sim
A simulator for the 2.0 Tenth platform using the new Gazebo sim. 

## ROS2 Build
1. Create your workspace folder
2. Create a src folder
3. Run `colcon build` on the empty folder to initialize
5. Clone the repository into the src folder
6. Run `rosdep update`
7. Run `rodep install --from-paths src -i -y`
8. Run `colcon build`

The build should be succesfully completed

## Tips 

Don't forget to `source /opt/ros/humble/setup.bash` if not 
in your `.bashrc` file.
Also `source install/setup.bash` on your workspace after the 
succesful build 

## Launch Files
There ia 1 useful `.launch` files which can be used for testing

1. `ros2 launch f1_tenth_bringup f1_tenth.launch.py` -> Launches both Gazebo simulator, Rviz  and 
a control node which requires the Logitech F710 controller connected to the host system to control 
the simulated vehicle.
