# Contactless Oxygen Saturation Detection Based on Face Analysis


```Python3 | Ensemble Learning | XGBoost | CNNs```

## Required Packages

```
tensorflow == 2.11.0
xgboost == 0.90
keras == 2.11.0
cv2 == 4.6.0
PIL == 7.1.2
onnxruntime == 1.13.1
numpy == 1.21.6
```

To load,
```pip3 install -r requirements.txt```

## 🧬 Overview

This repository contains the code used for our research **Contactless Oxygen Saturation Detection Based on Face Analysis: An Approach and Case Study** using facial videos and machine learning techniques. Our method extracts features from specific facial regions using **pre-trained CNN models**, then predicts SpO₂ using an **XGBoost Regressor**.

This approach demonstrates the potential of video-based health monitoring, offering an accessible, cuff-less, and non-invasive alternative to traditional pulse oximeters.

> ⚠️ **Note:** The datasets used in this project (e.g., VIPL-HR and UBFC-RPPG) are **not included** in this repository due to licensing restrictions. The codebase is fully functional and compatible with these datasets if you have access.




## 🧠 Methodology

###Preprocessing

1. Extract frames from facial videos.

2. Identify Regions of Interest (ROIs) on the face.

###Feature Extraction

1. Use pre-trained CNNs (e.g., ResNet50, MobileNetV2) to extract features from each ROI over time.

###SpO₂ Prediction

1.cTrain an XGBoost Regressor on the extracted features to predict SpO₂ values.

2. Evaluate on three test sets using: MAE (Mean Absolute Error), Pearson's correlation test, visual analysis of predicted SpO₂ distributions

## 📁 Repository Structure

```
Video-Based Blood Pressure Estimation/
│
├── Training.ipynb # Script for training models (Check the article for more info about the preprocessing stage)
├── Testing-VIPL.ipynb # Script for evaluating trained models on VIPL-HR Dataset
├── Testing-UBFC.ipynb #Script for evaluating trained models on UBFC-RPPG Dataset
├── requirements.txt # Required Python packages
└── README.md # Project documentation
```

## 📦 Model Weights
If you would like to access the pretrained models for testing or research purposes, please contact me at [bkhamud@itmo.ru] and I will share them upon request.

##🤝 Contributing
If you find a bug or have a suggestion for improvement, feel free to open an issue or submit a pull request. Contributions are always welcome.

##📜 Citation
If you found our work interesting, please cite it as:
```
@INPROCEEDINGS{10143059,
  author={Hamoud, Batol and Othman, Walaa and Shilov, Nikolay and Kashevnik, Alexey},
  booktitle={2023 33rd Conference of Open Innovations Association (FRUCT)}, 
  title={Contactless Oxygen Saturation Detection Based on Face Analysis: An Approach and Case Study}, 
  year={2023},
  volume={},
  number={},
  pages={54-62},
  keywords={Training;Technological innovation;Shape;Estimation;Predictive models;Feature extraction;Convolutional neural networks},
  doi={10.23919/FRUCT58615.2023.10143059}}

```

