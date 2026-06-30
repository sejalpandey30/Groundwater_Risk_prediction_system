# Groundwater_Risk_prediction_system

# Groundwater Risk Prediction System using Graph Attention Networks

> **An AI-driven Integrated Water Intelligence Framework for district-level groundwater risk prediction by combining groundwater stress assessment, water quality analysis, water pipeline leakage detection, and graph neural networks.**

![Python](https://img.shields.io/badge/Python-3.10-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-DeepLearning-red)
![PyTorch Geometric](https://img.shields.io/badge/GNN-PyTorch_Geometric-green)
![YOLOv8](https://img.shields.io/badge/YOLOv8-ObjectDetection-yellow)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

# Project Overview

Water resource management is one of the major sustainability challenges in India. Existing systems generally analyze groundwater quantity, water quality, and infrastructure failures independently, making it difficult to obtain a comprehensive understanding of district-level water security.

This project proposes an **Integrated Water Intelligence Framework** that combines:

* Groundwater Stress Assessment
* Water Quality Assessment
* Water Pipeline Leakage Detection
* Graph Attention Networks (GAT)

to generate an **Integrated Water Risk Index (IWRI)** for each district.

---

# Key Features

* Groundwater Stress Index (GSI)
* Water Quality Score (WQS)
* Water Pipeline Leakage Detection using YOLOv8
* Integrated Water Risk Index (IWRI)
* District-wise Graph Construction
* Graph Attention Network for spatial learning
* Explainable AI using attention weights
* District-level risk ranking

---

# System Architecture

```text
Groundwater Dataset
        │
        ▼
Groundwater Stress Assessment
        │
        ▼
Groundwater Stress Score
──────────────────────────────────

Water Quality Dataset
        │
        ▼
Water Quality Assessment
        │
        ▼
Water Quality Score
──────────────────────────────────

Leakage Images
        │
        ▼
YOLOv8 Leakage Detection
        │
        ▼
Leakage Score
──────────────────────────────────

Population + Rainfall
        │
        ▼
Feature Integration
        │
        ▼
Integrated Water Risk Index
        │
        ▼
District Graph Construction
        │
        ▼
Graph Attention Network
        │
        ▼
District Risk Prediction
```

---

# Repository Structure

```
Groundwater_Risk_Prediction_System/

│
├── README.md
│
├── stress_assessment.ipynb
│      Groundwater stress assessment pipeline
│      • Data preprocessing
│      • Feature engineering
│      • Groundwater Stress Index calculation
│
├── water_potability.csv
│      Water quality dataset
│
├── rs.csv
│      Groundwater resource dataset
│
├── water_leak_detection_1000_rows.csv
│      Leakage detection annotations
│
├── water-leakage-detection.ipynb
│      YOLOv8 training pipeline
│      • Dataset loading
│      • Model training
│      • Prediction
│
└── outputs/
       Model predictions
       Risk maps
       Trained models
```

---

# Datasets Used

## 1. Groundwater Resource Dataset

Source:
Central Ground Water Board (CGWB)

Features:

* Annual Recharge
* Net Groundwater Availability
* Annual Draft
* Stage of Groundwater Development
* Future Irrigation Availability
* Domestic Water Demand

---

## 2. Water Quality Dataset

Source:

Kaggle Water Potability Dataset

Features

* pH
* Hardness
* Solids
* Chloramines
* Sulfate
* Conductivity
* Organic Carbon
* Trihalomethanes
* Turbidity

---

## 3. Leakage Detection Dataset

Source

Water Pipes Dataset (Kaggle)

Contains annotated images of water pipelines for leakage detection using YOLOv8.

---

# Methodology

## Step 1

Groundwater Stress Assessment

Calculate

* Recharge
* Extraction
* Stress Index
* Irrigation Dependency
* Future Sustainability

↓

Groundwater Stress Score

---

## Step 2

Water Quality Assessment

Preprocess

↓

Normalize

↓

Train ML Model

↓

Generate Water Quality Score

---

## Step 3

Leakage Detection

YOLOv8

↓

Leak Detection

↓

Leakage Severity Score

---

## Step 4

Integrated Water Risk Index

Combine

Groundwater Stress

*

Water Quality

*

Leakage

↓

IWRI

---

## Step 5

Graph Construction

Each district

↓

Node

Neighbouring districts (<100 km)

↓

Edges

↓

Weighted Graph

---

## Step 6

Graph Attention Network

Input Features

↓

GAT Layer

↓

Attention Learning

↓

District Risk Prediction

---

# Machine Learning Models

| Module            | Algorithm               |
| ----------------- | ----------------------- |
| Water Quality     | Random Forest           |
| Leakage Detection | YOLOv8                  |
| Spatial Learning  | Graph Attention Network |

---

# Evaluation Metrics

Regression

* MAE
* RMSE
* R² Score

Detection

* Precision
* Recall
* F1 Score
* mAP

---

# Results

Example district prediction

| District | Risk Score |
| -------- | ---------- |
| Lucknow  | 82         |
| Kanpur   | 74         |
| Agra     | 45         |

---

# Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* PyTorch
* PyTorch Geometric
* Ultralytics YOLOv8
* Matplotlib
* OpenCV

---

# Future Improvements

* IoT sensor integration
* Real-time groundwater monitoring
* Satellite imagery integration
* Aquifer-level graph modeling
* Interactive web dashboard
* State-wide and national-scale deployment

---

# Research Paper

This repository accompanies the research work:

**"An AI-driven Integrated Water Intelligence Framework for Explainable District-Level Groundwater Risk Prediction using Graph Attention Networks."**

---

# Citation

```bibtex
@misc{groundwaterrisk2026,
  title={Groundwater Risk Prediction System using Graph Attention Networks},
  author={Sejal Pandey},
  year={2026},
  howpublished={GitHub Repository}
}
```

---

# Author

**Sejal Pandey**

* LinkedIn: https://www.linkedin.com/in/sejal-pandey-2aa018270/
* GitHub: [https://github.com/sejalpandey30](https://github.com/sejalpandey30)

```

