# Rosette Scans > 2023-07-14 1:06pm
https://universe.roboflow.com/rosette-identification-matdat-2023-4kpql/rosette-scans

Provided by a Roboflow user
License: CC BY 4.0

Rosette Scans - v2 2023-07-14 1:06pm
==============================

This dataset was exported via roboflow.com on July 14, 2023 at 5:10 PM GMT

Roboflow is an end-to-end computer vision platform that helps you
* collaborate with your team on computer vision projects
* collect & organize images
* understand and search unstructured image data
* annotate, and create datasets
* export, train, and deploy computer vision models
* use active learning to improve your dataset over time

For state of the art Computer Vision training notebooks you can use with this dataset,
visit https://github.com/roboflow/notebooks

To find over 100k other datasets and pre-trained models, visit https://universe.roboflow.com

The dataset includes 650 images.
The training set inlcudes 586 (post-augmentation) images.
The validation set inlcudes 32 images.
The test set inlcudes 32 images.

This split is representative of an 80%, 10%, 10% train, validation, and test split. The training set was expanded using augmentation techniques described below.

Rosettes are annotated in YOLOv8 format.

The annotation structure follows the following format. Each line in the labels file corresponds to one rosette annotation.

[Class ID] [x1] [y1] [x2] [y2] [x3] [y3] [x4] [y4] [x1] [y1]

The Class ID is always 0 which corresponds to a rosette object. The values for x1, y1, x2, y2, x3, y3, x4, y4, x1, y1 are all normalized coordinates for 4 points defining the boundary box of the annotated object.

The following pre-processing was applied to each image:
* Auto-orientation of pixel data (with EXIF-orientation stripping)
* Tile 10 rows x 10 columns
* Filter Null: Require at least 40% of images to contain annotations.

The following augmentation was applied to create 3 versions of each source image:
* 50% probability of horizontal flip
* 50% probability of vertical flip
* Random brigthness adjustment of between -25 and +25 percent
* Mosaic Applied
