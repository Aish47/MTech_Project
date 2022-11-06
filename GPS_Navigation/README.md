# GPS Waypoint Based Autonomous Navigation

GPS waypoints are given as reference path and vehicle is controlled to autonomously navigate from its current position to each of the defined waypoint. 

Sensor Input:    
GNSS Receiver:   GPS latitude, longititude and IMU heading angle

## Steps

1. First waypoints needs to be collected along the reference path. Code written to collect the waypoints.
2. Give the reference waypoints as input to the navigation algorithm which performs lateral control of vehicle at constant speed.
3. Perfom testing of autonomous navigation.
