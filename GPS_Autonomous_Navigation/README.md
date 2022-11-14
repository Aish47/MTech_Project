# GPS Waypoint Based Autonomous Navigation

GPS waypoints are given as reference path and vehicle is controlled to autonomously navigate from its current position to each of the defined waypoint. 

Sensor Input:    
GNSS Receiver:   GPS latitude, longititude and IMU heading angle

## Steps

1. First waypoints needs to be collected along the reference path. 
2. Give the reference waypoints as input to the navigation algorithm which performs lateral control of vehicle at constant speed.
3. Perfom testing of autonomous navigation.  

After autonomous navigation performed successfully, integrated pedestrian detection and depth estimation. This will perform braking action when pedestrian detected along the navigation path.

## Results

Below shows the testing of Autonomous Navigation along with Pedestrian detection that was implemented in the vehicle

<p align="center" width="70%">
    <img width="33%" src="https://github.com/Aish47/MTech_Project/blob/main/GPS_Autonomous_Navigation/nav_gif.gif">    
</p>

## Requirements

Software: ROS, pytorch, ZED SDK, CUDA  
Hardware: Jetson Orin (compute platform), GNSS Receiver, ZED 2i camera.

**Codes for the project above have not been uploaded as the research is still ongoing.
