# Drivable Area Detection using UNET

To perform semantic segmentation to detect drivable space detection. Sematic segmentation is deep learning method that classifies each pixel of the image to a particular class. There are many popular architecture for segmentation like UNET, FCN, SegNet, DeepLab. Out of these UNET architecture was implemented from scratch in Keras framework. The architecture was modified to be able to fit the image size of 80 * 160 and to give output as 3 channel classification (R, G, B). For the dataset, BDD drivable space dataset was used which has ego lane and adjacent lane labelled as RGB mask. A subset of original BDD dataset was considered for training (3000 images). Data augmentation steps like flipping the image was applied which increased the dataset to 6000 images. Train-test split of 85-15 % was used which divided the dataset into 5100 images for training and 900 images for validation.




