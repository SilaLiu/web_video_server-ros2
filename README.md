web_video_server [![Build Status](https://api.travis-ci.org/RobotWebTools/web_video_server.png)](https://travis-ci.org/RobotWebTools/web_video_server)
================

#### HTTP Streaming of ROS Image Topics in Multiple Formats
This node combines the capabilities of [ros_web_video](https://github.com/RobotWebTools/ros_web_video) and [mjpeg_server](https://github.com/RobotWebTools/mjpeg_server) into a single node.

For full documentation, see [the ROS wiki](http://ros.org/wiki/web_video_server).

[Doxygen](http://docs.ros.org/indigo/api/web_video_server/html/) files can be found on the ROS wiki.
[mjpegcanvasjs](https://github.com/rctoris/mjpegcanvasjs) can be used to display a MJPEG stream from the ROS web_video_server

This project is released as part of the [Robot Web Tools](http://robotwebtools.org/) effort.

### License
web_video_server is released with a BSD license. For full terms and conditions, see the [LICENSE](LICENSE) file.

### Authors
See the [AUTHORS](AUTHORS.md) file for a full list of contributors.

### Install    
```
sudo apt-get install ros-humble-async-web-server-cpp     
git clone this repo
colcon  build    
source install/setup.bash   
orangepi@orangepi5:~$ ros2 run web_video_server 
--prefix          web_video_server  
orangepi@orangepi5:~$ ros2 run web_video_server web_video_server 
[INFO] [1715939457.393743263] [web_video_server]: Waiting For connections on 0.0.0.0:8080
topic_type: sensor_msgs/msg/CameraInfo
topic_type: sensor_msgs/msg/Image
topic_type: rcl_interfaces/msg/ParameterEvent
topic_type: rcl_interfaces/msg/Log
```
http://192.168.10.179:8080/stream_viewer?topic=/image_raw
