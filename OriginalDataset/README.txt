# Rosette Scans > OriginalResolution
https://universe.roboflow.com/rosette-identification-matdat-2023-4kpql/rosette-scans

Provided by a Roboflow user
License: CC BY 4.0

Rosette Scans - v32 OriginalResolution
==============================

This dataset was exported via roboflow.com on April 30, 2025 at 2:09 AM GMT

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

The dataset includes 32 images.
Rosettes are annotated in YOLOv8 format.

The annotation structure follows the following format. Each line in the labels file corresponds to one rosette annotation.

[Class ID] [x1] [y1] [x2] [y2] [x3] [y3] [x4] [y4]

The Class ID is always 0 which corresponds to a rosette object. The values for x1, y1, x2, y2, x3, y3, x4, y4 are all normalized coordinates for 4 points defining the boundary box of the annotated object.




