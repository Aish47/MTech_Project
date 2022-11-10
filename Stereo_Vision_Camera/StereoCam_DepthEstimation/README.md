# Pedestrian detection and distance estimation using Stereo Vision

ZED 2i Stereo Vision camera used to perform detection based on Deep Learning Model and distance estimation perfromed.

## Description

* Pedestrian detected using YOLO v5 algorithm.
* A region of interest is considered as shown in figure below by the blue lines. Pedestrian is detected only if it is present inside this region. This is required to avoid detection of pedestrian on sidewalks.
* When Pedestrian detected inside ROI, distance calculation perfromed with stereo vision.
* Tested the algorithm with vehicle actuation control.
* Brake test performed.

## Results

Brake Test performed to check the stopping distance when pedestrian detected and also to understand the limitations of ZED 2i camera.

| Set Speed  | Set Stopping Distance | ZED Stopping distance | Actual Stopping Distance|
|:----------:|:---------------------:|:---------------------:|:-----------------------:|
| 8 kmph     | 7m                    | 2.7m                  | 2.7m                    |
| 8 kmph     | 10m                   | 5.12m                 | 5.1m                    |
| 10 kmph    | 7m                    | collision             | -                       |
| 10 kmph    | 10m                   | 4.12m                 | 3.9m                    |

* Stereo vision camera can give accurate measurements of the actual distance with
max error of ± 0.2m .
* Maximum range at which the stereo vision can detect in 16-20m.

