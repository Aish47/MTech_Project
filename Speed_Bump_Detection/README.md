# Speed Bump Detection

 Vision based speed bump detection with respect to Indian scenario in order to help navigate Autonomous vehicle.

## Datasets

Image dataset is prepared by merging different public domain datasets representing Indian scenarios.

1. https://github.com/AGV-IIT-KGP/SpeedBumpDetection 
2. S. Swan, “yolov5 speed breaker detection driver alert system dataset,”
Kaggle Data, vol. 1, 2021.
3. V. Varma, “Speed hump/bump dataset,” Mendeley Data, vol. 1, 2018.

## Requirements

Software: pytorch, Colab, CUDA  
Hardware: Jetson Orin

## Experiments

As YOLOv5 is giving accurate real-time object detection which is essential for Autonomous vehicles, so used pre-trained model to train the last few layers on speed bump dataset. 

* Exp 1 :     
Trained YOLO model on above three datasets. The models were overfitting on these datasets. Understood   the challenges in detecting speed bump.
* Exp 2 :   
Pre-processing of the dataset to clean the dataset and merged all three datasets - trained yolov5. This trained model was giving decent performance even on different distribution. Marked speed bump detection imporved, but unmarked speed bumps were not recognised. Feature difference could be the problem.
* Exp 3 :   
The dataset is now labelled as two classes - Marked and Unmarked. This improved the performance of unmarked speed bump detection. 

False detection of speed bump is still a problem due to shadows, water and different light condition on the road. Now working on depth based speed bump detection using stereo vision. 





