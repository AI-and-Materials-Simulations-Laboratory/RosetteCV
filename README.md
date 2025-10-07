# RosetteCV

The project demonstrates the development of a data pipeline that automates the detection of CSC Rosettes and conducts preliminary analytics to derive insights like lobe to lobe distance and rosette diameter. The pipeline includes the following steps:
1. Data Input
2. Rosette Detection
3. Human in the loop verification
4. Rosette Segmentation
5. Preliminary Analytics

The repository contains the following:
1. dataPipeline.ipynb
2. Original Dataset
3. Detection
4. Segmentation

The dataPipeline.ipynb contains the code necessary to run the data pipeline using the trained and tested models. The notebook contains a "Final Pipeline" section in which users can update the root path of the github folder and run the pipeline on a Large FF-TEM Scan. The input path can be updated to generate detections and results for desired scans.

The Original Dataset folder contains the images and labels of the original 32 images that were utilized in model development. This folder contains the raw data prior to any data processing/augmentation.

The Detection folder contains the following:
1. RosetteAugmentedData: This folder contains the preprocessed and augmented dataset used in detection model training and evaluation. The README within this folder goes into more detail about the dataset, including information like dataset split, preprocessing techniques, and augmentation techniques.
2. Yolov8Detection: This folder contains the Yolov8 detection model evaluation and testing results. The folder also contains results from training in the "yolov8m_v8_25e_rosetteAugmented" subfolder. Within this folder are also the finalized trained model weights for Yolov8.
3. Yolov9Detection: This folder contains the Yolov9 detection model evaluation and testing results. The folder also contains results from training in the "yolov9c_v9_25e_rosetteAugmented" subfolder. Within this folder are also the finalized trained model weights for Yolov9.
4. detection.ipynb: This notebook contains the training, evaluation, and testing code for the Yolov8 and Yolov9 Detection Models.

The Segmentation folder contains the following:
1. LobeSegmentation_v3: This folder contains the preprocessed dataset used in segmentation model training and evaluation. The README within this folder goes into more detail about the dataset.
2. Yolov8Segmentation: This folder contains the Yolov8 segmentation model evaluation and testing results. The folder also contains results from training in the "yolov8n_v3_seg_run" subfolder. Within this folder are also the finalized trained model weights for Yolov8 segmentation.
3. Yolov9Segmentation: This folder contains the Yolov9 segmentation model evaluation and testing results. The folder also contains results from training in the "yolov9n_v3_seg_run" subfolder. Within this folder are also the finalized trained model weights for Yolov9 segmentation.
4. segmentation.ipynb: This notebook contains the training, evaluation, and testing code for the Yolov8 and Yolov9 Segmentation Models.
