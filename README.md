# Privacy-Preserving Synthetic Data Generation using SDV Models

## Overview

Privacy-preserving data sharing has become increasingly important in healthcare, finance, government, and research domains where sensitive information cannot be shared directly. Synthetic data generation provides an effective solution by creating artificial datasets that preserve the statistical characteristics of the original data while protecting individual privacy.

This project presents a complete end-to-end framework for generating and evaluating synthetic tabular data using the Synthetic Data Vault (SDV). Three different SDV synthesizers—Gaussian Copula, CTGAN, and TVAE—are implemented and compared using multiple evaluation metrics including data quality, privacy preservation, statistical similarity, machine learning utility, and data drift.

The framework automatically recommends the best-performing model based on a weighted evaluation strategy.

---

# Problem Statement

Organizations often possess valuable datasets containing sensitive personal information that cannot be shared publicly due to privacy regulations and ethical concerns.

Traditional anonymization techniques frequently reduce data utility and may still expose sensitive information.

This project addresses these challenges by generating realistic synthetic datasets that preserve the statistical properties and predictive performance of the original dataset without revealing actual individual records.

---

# Objectives

- Generate privacy-preserving synthetic tabular data
- Compare multiple SDV synthesizers
- Evaluate statistical similarity between real and synthetic datasets
- Measure machine learning utility
- Analyze privacy preservation
- Detect data drift
- Compare computational performance
- Recommend the best synthetic data generation model

---

# Dataset

**Dataset:** Adult Income Dataset

Dataset Characteristics

- Approximately 5,000 records
- 15 attributes
- Mixed numerical and categorical features
- Binary classification problem

Target Variable

- Income

---

# Project Workflow

```
Real Dataset
      │
      ▼
Data Loading
      │
      ▼
Data Preprocessing
      │
      ▼
Metadata Detection
      │
      ▼
Synthetic Data Generation
      │
      ├── Gaussian Copula
      ├── CTGAN
      └── TVAE
      │
      ▼
Synthetic Dataset
      │
      ▼
Evaluation
      │
      ├── Data Quality
      ├── Privacy Evaluation
      ├── Statistical Comparison
      ├── Machine Learning Utility
      ├── Data Drift
      ├── PCA Analysis
      ├── t-SNE Analysis
      ├── SHAP Analysis
      ├── ROC Curve
      ├── Precision-Recall Curve
      └── Model Recommendation
```

---

# Repository Structure

```
Privacy-Preserving-Synthetic-Data-Generation-using-SDV-Models/

│
├── data/
│      Adult Income Dataset
│
├── notebook/
│      Privacy_Preserving_Synthetic_Data_Generation.ipynb
│
├── images/
│      Project screenshots
│
├── results/
│      Synthetic datasets
│      Statistical comparison reports
│
├── paper/
│      Research paper
│
├── README.md
├── requirements.txt
├── LICENSE
└── .gitignore
```

---

# Technologies Used

| Category | Technologies |
|-----------|--------------|
| Programming Language | Python |
| Data Processing | Pandas, NumPy |
| Data Visualization | Matplotlib, Seaborn |
| Synthetic Data Generation | SDV, CTGAN |
| Machine Learning | Scikit-learn |
| Explainable AI | SHAP |
| Statistical Analysis | SciPy |
| Excel Export | OpenPyXL |
| Development Environment | Jupyter Notebook |

---

# Synthetic Data Models

| Model | Description |
|---------|-------------|
| Gaussian Copula | Statistical probabilistic model for tabular data generation |
| CTGAN | Conditional Generative Adversarial Network for tabular datasets |
| TVAE | Variational Autoencoder-based synthetic data generator |

---

# Evaluation Metrics

The generated synthetic datasets are evaluated using the following criteria.

## Data Quality

- Quality Score
- Column Shapes
- Pair Trends

## Privacy Evaluation

- Privacy Nearest Neighbor Score

## Statistical Evaluation

- Mean
- Standard Deviation
- Median
- Distribution Comparison

## Machine Learning Utility

- Accuracy
- F1 Score
- Recall
- ROC-AUC
- PR-AUC

## Data Drift

- Feature Drift Analysis
- Overall Drift Score

## Computational Performance

- Training Time
- Sampling Time
- Memory Usage

---

# Visualizations

The project includes the following visualizations.

- Dataset Overview
- Missing Value Analysis
- Age Distribution
- Income Distribution
- Quality Score Comparison
- Privacy Score Comparison
- Data Drift Comparison
- KDE Distribution Comparison
- Correlation Heatmaps
- Correlation Difference Analysis
- PCA Visualization
- t-SNE Visualization
- SHAP Feature Importance
- ROC Curve
- Precision-Recall Curve
- Overall Model Performance
- Recommendation Score Comparison

---

# Results

The framework performs a comprehensive comparison of Gaussian Copula, CTGAN, and TVAE based on:

- Data Quality
- Privacy Preservation
- Statistical Similarity
- Machine Learning Utility
- Computational Efficiency

A weighted recommendation framework is used to identify the most suitable synthetic data generation model for the given dataset.

In this project, **CTGAN** achieved the highest overall recommendation score based on the combined evaluation metrics.

---

# Project Features

- End-to-end synthetic data generation pipeline
- Automatic metadata detection
- Three SDV model comparison
- Privacy evaluation
- Statistical comparison
- Machine learning utility testing
- Data drift analysis
- Correlation analysis
- PCA visualization
- t-SNE visualization
- SHAP explainability
- ROC and Precision-Recall analysis
- Automated model recommendation
- Export synthetic datasets to Excel

---

# Future Scope

Future enhancements may include:

- Differential Privacy integration
- Large-scale synthetic dataset generation
- Hyperparameter optimization
- Support for time-series synthetic data
- Support for image and text synthetic data
- Streamlit web application
- Docker deployment
- Cloud deployment
- REST API integration

---

# Installation

Clone the repository

```bash
git clone https://github.com/Rakshitha765/Privacy-Preserving-Synthetic-Data-Generation-using-SDV-Models.git
```

Navigate to the project directory

```bash
cd Privacy-Preserving-Synthetic-Data-Generation-using-SDV-Models
```

Install the required libraries

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook

```bash
jupyter notebook
```

Open the notebook inside the **notebook** folder and execute the cells sequentially.

---

# Research Paper

This implementation is based on the research work:

**Privacy-Preserving Synthetic Data Generation using SDV Models**

The repository contains both the complete implementation and the associated research paper.

---

# Author

**Rakshitha G**

Bachelor of Engineering (Artificial Intelligence and Machine Learning)

Interested in Data Analytics, Data Science, Machine Learning, and Artificial Intelligence.

GitHub: https://github.com/Rakshitha765

---

# License

This project is licensed under the MIT License.

See the LICENSE file for additional information.
