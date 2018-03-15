# stage_ros
Package which contains ROS specific hooks and tools for the Stage simulator.

This is a stage_ros with update so that lasers and sonars publish to different topics

* lasers (samples > 1) publish to base_scan with sensor_msgs/LaserScan msg type

* sonars (samples = 1) publish to sonar_scan with sensor_msgs/Range msg type

* Before, stage_ros only differentiated between laser and sonar by samples (1 sample = sonar, otherwise is laser) This would publish to base_scan with sensor_msgs/LaserScan msg type
