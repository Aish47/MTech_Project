# Pedestrian detection and Depth Estimation using Single Camera

Detect pedestrian using Deep Learning Model and estimate its depth using single camera. The depth information is used to perfrom braking action of the vehicle. This was a simple method to understand how algorithm can be implemented to actuate the vehicle. A more robust method will be explored with stereo vision system.

## Description

* Pedestrian detection is performed using YOLO v5 algorithm.
* A region of interest is considered as shown in figure below by the blue lines. Pedestrian is detected only if it is present inside this region.

<p align="center" width="70%">
    <img width="33%" src="https://github.com/Aish47/MTech_Project/blob/main/Stereo_Vision_Camera/MonoCam_DepthEstimation/fig1.png">    
</p>

* When the pedestrian is inside the region of interest and the distance is less than a certain threshold, command is sent to vehicle actuators to reduce speed to 0.

## Results

<img align="left" width="33%" src="https://github.com/Aish47/MTech_Project/blob/main/Stereo_Vision_Camera/MonoCam_DepthEstimation/fig2.png">  
* Distance threshold given = 6m<br>  
* Vehicle Stopped at 3.5m<br>  
* Actual measurement = 3.7m<br>  
* Even with single camera able to get good results for distance estimation with error within ±  0.4m.<br>



