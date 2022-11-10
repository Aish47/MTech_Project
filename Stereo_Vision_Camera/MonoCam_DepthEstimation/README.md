# Pedestrian detection and Depth Estimation using Single Camera

Detect pedestrian using Deep Learning Model and estimate its depth using single camera. The depth information is used to perfrom braking action of the vehicle.

## Description

* Pedestrian detection is performed using YOLO v5 algorithm.
* A region of interest is considered as shown by the blue lines in Fig 1. Pedestrian is detected only if it is present inside this region.

![fig1](https://user-images.githubusercontent.com/97548464/201071370-b67db7fb-74a4-4aed-b4bb-2f1a248b7958.png=250x250)  

* When the pedestrian is inside the region of interest and the distance is less than a certain threshold, command is sent to vehicle actuators to reduce speed to 0.

