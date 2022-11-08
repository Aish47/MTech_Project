# Training with Two classes

The Merged Dataset (Dataset M) is re-labelled to separate speed bump class into two classes - marked speed bump and unmarked speed bump.
Training performed on this dataset.

Merged Dataset with two classes (Dataset M2):    
* Two classes: Marked and Unmarked
* 885 images total
    * Marked speed bump instances: 823
    * Unmarked Speed Bump instances: 323

Augmentation applied to Dataset M2 (Dataset M2A):  
* Two classes: Marked and Unmarked
* 885 images
* Augmentation Techniques: Horizontal Flip, Brightness, grayscale.

Yolov5 model trained on these two dataset, to check if it improves the detection of unmarked speed bump.

## Performance Metrics

| Model name    | Dataset       | Training    | Validation    | Num Class  | Precision  | Recall    | mAP@0.5   |
|:-------------:|:-------------:|:-----------:|:-------------:|:----------:|:----------:|:---------:|:---------:|
|Model 6        |Dataset M2     | 697         | 175           | 2          |82.6 %      | 78.2 %    | 80.29 %   |
|Model 7        |Dataset M2A    | 2091        | 175           | 2          |93.5 %      | 76.6 %    | 84.21 %   |

## Observation.

* Model 7 has slight improvement in performance compared to when trained as one class. 
* Unmarked speed bumps are now detected with more confidence.
* False detection rate has decreased.
* Model 7 gives the best detection results compared to all other previous models.

## Future Work

* There is still lot of scope for performance improvement. 
* Dataset collection going on in and around the campus to get a more local distribution of dataset.
* Perform next experiment with bigger DNN.
