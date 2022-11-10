# Pedestrian detection and Depth Estimation using Single Camera

Detect pedestrian using Deep Learning Model and estimate its depth using single camera. The depth information is used to perfrom braking action of the vehicle.

## Description

* Pedestrian detection is performed using YOLO v5 algorithm.
* A region of interest is considered as shown by the blue lines in Fig 1. Pedestrian is detected only if it is present inside this region.

![alt text](https://github.com/Aish47/MTech_Project/blob/main/Stereo_Vision_Camera/MonoCam_DepthEstimation/fig1.png?raw=true)  

* When the pedestrian is inside the region of interest and the distance is less than a certain threshold, command is sent to vehicle actuators to reduce speed to 0.