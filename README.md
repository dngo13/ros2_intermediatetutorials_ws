# ROS2 Intermediate Tutorials Workspace
## Requirements
- Ubuntu 24.02
- ROS2 Jazzy (Install [here](https://docs.ros.org/en/jazzy/Installation/Ubuntu-Install-Debs.html))

This ROS2 workspace has the packages from the intermediate tutorials from the ROS 2 Jazzy documentation. 
All tutorials are from [here](https://docs.ros.org/en/jazzy/Tutorials/Intermediate.html).

## Packages in `/src`
- `custom_action_interfaces`

## Running code
- Ensure the workspace is built with `colcon build`
- If you need to build a specific package then run `colcon build --packages-select "package name"`
- Make sure the environment is sourced with `source install/setup.bash`
- Install any missing dependencies by going to root folder `ros2_intermediatetutorials_ws` and run `rosdep install -i --from-path src --rosdistro jazzy -y`
- `ros2 run <package_name> <node_name>`