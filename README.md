# network-intrusion-detection-ml
Multi-class network intrusion detection using machine learning to classify normal traffic and DoS, Probe, R2L and U2R attacks.
# Multi-Class Network Intrusion Detection using Machine Learning

## Overview

This project explores the use of machine learning for network intrusion detection. The objective is to build and evaluate a multi-class classifier capable of distinguishing normal network traffic from four major categories of attacks:

- Denial of Service (DoS)
- Probe
- Remote-to-Local (R2L)
- User-to-Root (U2R)

The project uses an improved and de-duplicated version of the classic KDD Cup 1999 network intrusion detection dataset containing approximately 148,000 labelled network connection records and 41 traffic, content-based, and time-based features.

---

## Project Objectives

The main objectives of this project are to:

- Build a machine learning model for multi-class network attack classification
- Distinguish normal traffic from DoS, Probe, R2L, and U2R attacks
- Analyse the dataset and prepare features for machine learning
- Evaluate model performance across different attack categories
- Compare Accuracy, Precision, Recall, and F1-score
- Analyse which features contribute most to the model's decisions
- Examine challenges caused by differences in attack frequency and class distribution

---

## Attack Categories

| Class | Description |
|---|---|
| Normal | Legitimate network activity |
| DoS | Attacks intended to make systems or services unavailable |
| Probe | Attempts to gather information about systems and services |
| R2L | Attacks where an external attacker gains access to a local account |
| U2R | Attacks where a local user attempts to gain elevated privileges |

---

## Dataset

The dataset is an improved and de-duplicated version of the KDD Cup 1999 dataset.

### Dataset Characteristics

- Approximately 148,000 network connection records
- 41 input features
- Multi-class attack classification
- Traffic-based features
- Content-based features
- Time-based features

The dataset represents network connections labelled as either normal activity or one of several categories of malicious activity.

> The dataset is used for educational and research purposes. This repository does not include proprietary or sensitive network data.

---

## Project Workflow

The project follows the following workflow:

```text
Dataset
   ↓
Exploratory Data Analysis
   ↓
Data Cleaning and Preprocessing
   ↓
Feature Encoding and Transformation
   ↓
Model Training
   ↓
Multi-Class Classification
   ↓
Model Evaluation
   ↓
Feature Importance Analysis

Machine Learning Tasks

The project includes the following key stages:

1. Data Preparation
Loading and inspecting the dataset
Checking class distribution
Handling categorical features
Encoding attack categories
Preparing features for model training
Creating training and testing datasets
2. Exploratory Data Analysis

The dataset is analysed to understand:

Attack category distribution
Feature characteristics
Differences between normal and malicious traffic
Relationships between important network features
3. Model Training

Machine learning models are trained to classify network traffic into the following categories:
Normal
DoS
Probe
R2L
U2R
4. Model Evaluation

Model performance is evaluated using:

Accuracy
Precision
Recall
F1-score
Confusion Matrix
Class-wise performance

Special attention is given to the performance of minority attack categories such as R2L and U2R.

5. Feature Importance

The project also investigates which network characteristics have the greatest influence on the model's classification decisions.

This helps answer an important question:

Which characteristics of a network connection are most useful for distinguishing legitimate activity from different categories of attacks?

Technologies Used
Python
Pandas
NumPy
Scikit-learn
Matplotlib
Machine Learning
Network Security

Repository Structure

The repository will be organised as follows:
network-intrusion-detection-ml/
│
├── data/
│   └── README.md
│
├── notebooks/
│   └── intrusion_detection_analysis.ipynb
│
├── src/
│   ├── preprocess.py
│   ├── train.py
│   └── evaluate.py
│
├── results/
│   ├── confusion_matrix.png
│   └── feature_importance.png
│
├── README.md
├── requirements.txt
└── LICENSE

Key Learning Areas

Through this project, I explored:

Multi-class machine learning classification
Network intrusion detection
Cybersecurity dataset analysis
Class imbalance
Feature engineering
Model evaluation
Security-focused machine learning
Feature importance and explainability
Results

Detailed model performance and visualisations will be added as the project is documented and refined.

The final analysis will focus not only on overall accuracy, but also on how reliably the model identifies individual attack categories.

Future Improvements

Potential areas for further development include:

Comparing multiple machine learning models
Hyperparameter tuning
Advanced feature selection
Handling class imbalance
SHAP or other explainability techniques
Testing model robustness
Evaluating performance on previously unseen network traffic
Author

Rakshak

Cybersecurity | Identity & Access Management | DFIR | Cloud & AI Security

Disclaimer

This project is created for educational and portfolio purposes using publicly available cybersecurity datasets. It does not involve testing against unauthorised systems or networks.
