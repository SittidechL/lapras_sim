# lapras_sim
```
mkdir nav2sim_ws && cd nav2sim_ws
git clone https://github.com/SittidechL/lapras_sim.git
mkdir src
mv lapras_sim src/
colcon build
cd ..
source /opt/ros/galactic/setup.bash
cd nav2sim_ws
colcon build
source install/local_setup.bash
sudo apt install ros-galactic-gazebo-ros   # install "gazebo"
sudo apt install ros-galactic-gazebo-plungins   # E: Unable to locate package ros-galactic-gazebo-plungins (cmd: env |grep ROS)
export GAZEBO_MODEL_PATH=/usr/share/gazebo-11/models:${GAZEBO_MODEL_PATH}:~/nav2sim_ws/src/lapras_sim # dir to "nav2sim_ws" path: nav2sim_ws/src/lapras_sim/config/env_config --> double click
ros2 launch lapras_sim lapras_world.launch.py
```
### galactic
```
ctr+atl+t
source /opt/ros/galactic/setup.bash
ros2 topic list

```
