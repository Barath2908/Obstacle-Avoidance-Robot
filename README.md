# Obstacle-Avoidance-Robot
Description:
The project, titled "Obstacle Avoidance in ROS with Sensor Data Listener," provides a Python script designed to facilitate obstacle avoidance using Robot Operating System (ROS). The script is located at Obstacle_Avoidance_ROS/scripts/sensor_data_listener.py and enables the robot to subscribe to sensor data from the /scan topic, process this data, and publish velocity commands to the /cmd_vel topic.

Key Functionalities:

Sensor Data Subscription: The Python script subscribes to the /scan topic, which contains data in the sensor_msgs.msg.LaserScan message format. The incoming laser scan data is essential for the robot to perceive its surroundings and detect obstacles.

LaserScan Processing: The script applies the LaserScanProcess() function to the incoming data. This function presumably performs essential obstacle avoidance calculations based on the laser scan information. The details of the processing logic are likely present in the script itself, but they are not explicitly described in this overview.

Velocity Command Publication: The script publishes velocity commands to the /cmd_vel topic. These commands are represented as Twist messages, which typically include linear and angular velocities. Controlling these velocities allows the robot to navigate and avoid obstacles effectively.

Visualization: To visualize the effect of the velocity commands, you can use the rostopic command to echo the /cmd_vel topic. This provides real-time feedback on the linear and angular velocities, which are crucial for understanding how the robot is responding to the obstacle avoidance logic.
