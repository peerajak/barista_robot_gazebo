# ros2_theconstruct_checkpoint7, and 8
must use together with barista_robot_description repository


## Checkpoint 7

Terminal 1

```
cd ~/ros2_ws && colcon build && source install/setup.bash
ros2 launch barista_robot_description barista_urdf.launch.py
```

## Checkpoint 8

Termianl 1

```
cd ~/ros2_ws && colcon build && source install/setup.bash
ros2 launch barista_robot_description barista_two_robots.launch.py
```

Terminal 2

```
cd ~/ros2_ws && colcon build && source install/setup.bash
ros2 run robot_chase robot_chase
```

Terminal 3

```
cd ~/ros2_ws && colcon build && source install/setup.bash
ros2 run teleop_twist_keyboard teleop_twist_keyboard --ros-args --remap cmd_vel:=/morty/cmd_vel
```


