# Training YOLO on merged dataset

Merged the three datasets datasets into more robust dataset and pre-processing of dataset performed.

Merged Dataset: (Dataset M)  
* One Class: Speed Bump
* 885 images of marked and unmarked speed bumps.

Merged Dataset with Augmentation: (Dataset MA)  
* One Class: Speed Bump
* 2279 images 
* Augmentation Techniques: Horizontal Flip, Brightness, grayscale.

Yolov5 model trained on these two dataset, to get a more robust model for different distribution dataset.

## Performance metrics

| Model name    | Dataset       | Training    | Validation    | Num Class  | Precision  | Recall    | mAP@0.5   |
|:-------------:|:-------------:|:-----------:|:-------------:|:----------:|:----------:|:---------:|:---------:|
|Model 4        |Dataset M      | 697         | 175           | 1          |87.6 %      | 78.7 %    | 82.91 %   |
|Model 5        |Dataset MA     | 2091        | 175           | 1          |89.4 %      | 81.7 %    | 85.37 %   |

## Observation

* Model 4 and 5 perfromance shown above when trained on more robust distribution of dataset. The models have slight dip in performance compared to Exp 1. 
* Data Augmentation performed and trained on this dataset - performance improved.
* Model 5 is able to detect marked speed bumps but still there is problem in detecting some unmarked speed bumps.
* The number of false detection or misclassification is comparatively less compared to Exp 1 models.
* Crosswalk is being misclassified as speed bump.
* Light and weather condition leading to false detections.

## Future Work

* The features of unmarked and marked speed bumps are different, so in next experiment will work with two classes.
* Train on bigger model to improve the performance.
* Unmarked speed bumps are under represented so working on increasing the dataset.
