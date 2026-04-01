//=====================...........................=================================
// Authors : Milou de Zwaan (2629070), Shatrunjay Palkar (3669734)
// Group : 14
// License : LGPL open source license
//
// Brief : how to run
//=====================...........................=================================

Package relbot_sequence_controller

#### here we assume all the other packages are already ready (msg, launch, simulator etc ). because the sequence controller was the only thing we had to submit:  
build:
cd ~/ros2_ws 
colcon build --packages-select relbot_sequence_controller
source install/setup.bash

Run:
ros2 launch relbot_launch relbot_sequence_controller.launch.py


Core components:
- calculate_velocity(): The function that you will have to alter.
- timer_callback(): publishes the velocity to both wheel 30 times per second.

Core components:
- calculate_velocity(): The function that you will have to alter.
- timer_callback(): publishes the velocity to both wheel 30 times per second.

Output:
`/input/left_motor/setpoint_vel`
- Type: example_interfaces/msg/Float64

`/input/left_motor/setpoint_vel`
- Type: example_interfaces/msg/Float64