A Hybrid CNN–Transformer Framework for Event-Based Human Activity Recognition in Challenging Scenarios
Overview

This project implements a hybrid deep learning framework for event-based human activity recognition (HAR) in challenging real-world scenarios. The approach combines 3D CNNs and Transformer-based models to capture both local spatiotemporal patterns and long-range temporal dependencies from event-based video data.

The experiments are conducted on the Challenging THU-EACT-50 (CHL) dataset.

Dataset

The dataset used in this project is THU-EACT-50, specifically the Challenging (CHL) split.

Download the dataset and the official preprocessing code from:

https://github.com/lujiaxuan0520/THU-EACT-50

Preprocessing

Use the official preprocessing code provided with the dataset to convert raw event streams into 9 frames per video.

After generating the frames, run the custom preprocessing notebook:

preprocessing_DL_project.ipynb


This step prepares the data for CNN, Transformer, and hybrid models.

Models and Files

Custom Preprocessing

preprocessing_DL_project.ipynb


3D CNN (ResNet-18)

resnet_18_3d.ipynb


Transformer (TimeSformer)

DL_project_TimeSformer_with_own_prepocess_of_8_frams.ipynb


Hybrid CNN–Transformer Model

hybrid_Model_resnet_&_timesformer.ipynb


Each model can be trained and evaluated independently after preprocessing.

Execution Order

Download THU-EACT-50 (CHL) dataset

Convert event data to 9-frame videos using the official code

Run preprocessing_DL_project.ipynb

Run any of the model notebooks (CNN, Transformer, or Hybrid)

Author

Amir Khan
