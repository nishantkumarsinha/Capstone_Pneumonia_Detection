## RSNA Pneumonia Detection Detection - Capstone Project
Capstone Project completed as a part of Great Learning's PGP - Artificial Intelligence and Machine Learning.

## 📁 Getting Started
The project is built on Google Colab Jupyter Notebook. Clone this repository to get started, as mentioned below. You can upload the cloned folder to your google drive or else git clone from google colab.
```
$ git clone https://github.com/sharmapratik88/Capstone_Pneumonia_Detection.git
```

## 🤔 Problem Statement
In this capstone project, the goal is to build a pneumonia detection system, to locate the position of inflammation in an image. Tissues with sparse material, such as lungs which are full of air, do not absorb the X-rays and appear black in the image. Dense tissues such as bones absorb X-rays and appear white in the image. While we are theoretically detecting “lung opacities”, there are lung opacities that are not pneumonia related. In the data, some of these are labeled “Not Normal No Lung Opacity”. This extra third class indicates that while pneumonia was determined not to be present, there was nonetheless some type of abnormality on the image and oftentimes this finding may mimic the appearance of true pneumonia.

## 📜 Approach
### 📈 Step 1: Exploratory Data Analysis & Data Preparation
* Understanding the data with a brief on train/test labels and respective class info
* Look at the first five rows of both the csvs (train and test)
* Identify how are classes and target distributed
* Check the number of patients with 1, 2, ... bounding boxes
* Read and extract metadata from dicom files
* Perform analysis on some of the features from dicom files
* Check some random images from the training dataset
* Draw insights from the data at various stages of EDA
* Visualize some random masks generated

**Outcome**
* [Jupyter Notebook Link](https://nbviewer.jupyter.org/github/sharmapratik88/Capstone_Pneumonia_Detection/blob/master/Pneumonia_Detection_EDA_%26_Data_Prep.ipynb) containing the exploration steps.
* [Module Link](https://github.com/sharmapratik88/Capstone_Pneumonia_Detection/blob/master/module/eda.py) contains custom module which was built to help in performing EDA.
* [Data Generator](https://github.com/sharmapratik88/Capstone_Pneumonia_Detection/blob/master/module/data_generator.py) contains custom module which was built for data generate and help in visualizing the masks.
* [Output (pickle files)](https://github.com/sharmapratik88/Capstone_Pneumonia_Detection/tree/master/output) contains output files such as `train_class_features.pkl` containing metadata features and `train_feature_engineered.pkl` after feature engineering on training dataset.
