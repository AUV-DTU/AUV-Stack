# DTU-AUV Simulations

Ignition gazebo based simulations for our vehicles (using bluerov for now)


## Getting started

Setting the environment variable

```bash
export GZ_SIM_RESOURCE_PATH=/{path_to_this_directory}/
```

Running the simulations

Add this package to the src folder in your workspace , from the root run
```bash
colcon build
source ./install/setup.bash
ros2 launch simulation display.launch.py
```

To run the teleop node , open a new terminal and source the workspace
```bash
cd src/simulation/scripts
chmod +x bluerov_teleop_ign.py
./bluerov_teleop_ign.py