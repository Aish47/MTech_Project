# Training YOLOv5 separately on three datasets

## Dataset Descriptions

Mendeley :  467 images containing both marked and unmarked speed bumps. (Around Coimbatore)  
Kaggle :  2932 images containing both marked and unmarked speed bumps. (Tamil Nadu)  
IIT Kgp : 1889 images containing marked speed bumps. (Inside IIT Kgp campus)  

Observation:  

Speed Bumps vary in size and nature from one location to another in Indian Scenario. Broadly speed bumps can be classified as Marked Speed Bumps and Unmarked Speed Bumps. Even in marked speed bumps, no standard marking is followed. 

## Perfromance Metrics 

Below table gives the performance metrics when YOLOv5 model is trained on three datasets separately:

| Model name    | Dataset       | Training    | Validation    | Precision    | Recall    | mAP@0.5  |
|:-------------:|:-------------:|:-----------:|:-------------:|:------------:|:---------:|:--------:|
|Model 1        |Mendeley       | 368         | 72            | 98.5 %       | 89.0 %    | 95.4 %   |
|Model 2        |Kaggle         | 2200        | 532           | 96.6 %       | 95.0 %    | 97.0 %   |
|Model 3        |IIT Kgp        | 1889        | 372           | 97.1 %       | 94.8 %    | 97.9 %   |

## Observations

* All these trained models are able to detect all marked speed bumps. But fail to detect some unmarked speed bumps.
* Kaggle and IIT kgp datasets have lot of repeatitive images and the models trained on these datasets seemed to be overfiting. Performance of these models are not good for different distribution dataset.

Below table describes the performance of Model 2 and Model 3 when tested on Mendeley dataset:

| Model name     | Validation Dataset    | Precision    | Recall    | mAP@0.5  |
|:--------------:|:---------------------:|:------------:|:---------:|:--------:|
| Model 2        | Mendeley(368 images)  | 74.2 %       | 42.5 %    | 47.6 %   |
| Model 3        | Mendeley(368 images)  | 75.9 %       | 37.9 %    | 43.0 %   |

* Zebra crossings and shadows are also misclassified as Speed bumps.
* Different weather and lighting conditions are affecting the detection of speed bumps

## Future Work

* In next experiment, pre-processing of dataset to be performed - remove repeatative images and merge all the datatsets to get robust dataset.
* Data Augmentation to be performed to increase the training data.



