# Machine Learning: Concrete Compressive Strength Analysis

[![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.7+-green.svg)](https://scikit-learn.org/)

A comprehensive machine learning project analyzing concrete compressive strength using various supervised and unsupervised learning techniques. This project was completed as part of the 02452 Machine Learning course (Fall 2025).

## 📊 Project Overview

This project applies machine learning techniques to predict and analyze concrete compressive strength based on mixture ingredients and age. The analysis includes exploratory data analysis, feature engineering, dimensionality reduction, and predictive modeling using both regression and classification approaches.

### Key Highlights

- **Dataset**: 1,030 instances of concrete samples with 8 input features
- **Techniques**: PCA, Linear Regression, Ridge Regression, Artificial Neural Networks, Logistic Regression
- **Validation**: K-fold cross-validation with statistical hypothesis testing
- **Visualizations**: Comprehensive plots showcasing data distribution, correlations, model performance, and feature importance

## 📂 Repository Structure

```
.
├── ML Assignment 1 - Data; Feature Extraction, and Visualization.ipynb
├── ML Assignment 2 - Supervised Learning; Classification and Regression.ipynb
├── Concrete_Data.xls                    # Dataset
├── Concrete_Readme.txt                  # Dataset documentation
├── Plots/                               # Generated visualizations
│   ├── Correlation Matrix.png
│   ├── PCA Projection.png
│   ├── Generalization Error vs λ.png
│   └── ... (16 plots total)
├── requirements.txt                     # Python dependencies
└── README.md                           # This file
```

## 🎯 Assignments

### Assignment 1: Data Analysis, Feature Extraction, and Visualization

**Notebook**: [ML Assignment 1](./ML%20Assignment%201%20-%20Data%3B%20Feature%20Extraction%2C%20and%20Visualization.ipynb)

This notebook covers:
- **Exploratory Data Analysis (EDA)**
  - Data loading and preprocessing
  - Missing value analysis
  - Statistical summaries and distributions
  - Correlation analysis
  
- **Dimensionality Reduction with PCA**
  - Principal Component Analysis implementation
  - Variance explained analysis
  - Feature contribution to principal components
  - 2D and 3D visualizations of transformed data
  
- **Comprehensive Visualizations**
  - Histograms showing feature distributions
  - Boxplots for outlier detection
  - Correlation matrices and heatmaps
  - PCA scree plots and cumulative variance
  - Feature contribution plots

**Key Findings**:
- Strong correlations between cement content and compressive strength
- Age of concrete is a significant factor in strength development
- PCA reveals 3-4 principal components capture majority of variance

### Assignment 2: Supervised Learning (Classification and Regression)

**Notebook**: [ML Assignment 2](./ML%20Assignment%202%20-%20Supervised%20Learning%3B%20Classification%20and%20Regression.ipynb)

This notebook implements:

#### Regression Analysis
- **Linear Regression**: Baseline model with feature importance analysis
- **Regularized Ridge Regression**: With λ parameter tuning via cross-validation
- **Artificial Neural Networks (ANN)**: Multi-layer perceptron for non-linear modeling
- **Model Comparison**: Statistical testing (paired t-tests) to compare model performance

#### Classification Analysis
- **Binary Classification**: Categorizing concrete strength (high/low)
- **Logistic Regression**: Linear decision boundary
- **Multi-Layer Perceptron Classifier**: Non-linear classification
- **Baseline Comparison**: Dummy classifier for performance benchmarking
- **Statistical Validation**: McNemar's test for classifier comparison

**Key Results**:
- Ridge regression with optimal λ reduces overfitting
- ANN models capture non-linear relationships in the data
- Cross-validation RMSE ranges from ~9-11 MPa across models
- Classification achieves >85% accuracy for strength categorization

## 📈 Sample Visualizations

The project includes 16 high-quality visualizations in the `Plots/` directory:

- **Data Exploration**: Histograms, Boxplots, Correlation Matrix
- **PCA Analysis**: Scree Plot, Cumulative Variance, PC Projections, Feature Contributions
- **Model Performance**: Generalization Error curves, RMSE Comparisons, Training Loss
- **Statistical Tests**: Pairwise MSE Differences for model comparison

## 🔧 Technologies & Libraries

- **Python 3.9+**
- **Data Analysis**: NumPy, Pandas
- **Machine Learning**: scikit-learn, SciPy
- **Visualization**: Matplotlib, Seaborn
- **Notebook Environment**: Jupyter, IPython

## 🚀 Getting Started

### Prerequisites

Ensure you have Python 3.9 or higher installed.

### Installation

1. Clone this repository:
```bash
git clone https://github.com/chrisd314/02452_Machine_Learning_Project_Fall_2025.git
cd 02452_Machine_Learning_Project_Fall_2025
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

### Running the Notebooks

1. Launch Jupyter Notebook:
```bash
jupyter notebook
```

2. Open either notebook in your browser:
   - `ML Assignment 1 - Data; Feature Extraction, and Visualization.ipynb`
   - `ML Assignment 2 - Supervised Learning; Classification and Regression.ipynb`

3. Run cells sequentially to reproduce the analysis

### Viewing on GitHub

GitHub automatically renders Jupyter notebooks! You can view the notebooks directly by clicking the links above without installing anything.

## 📊 Dataset Information

**Source**: UCI Machine Learning Repository  
**Donated by**: Prof. I-Cheng Yeh, Chung-Hua University, Taiwan

### Features (8 Input Variables)
1. **Cement** (kg/m³)
2. **Blast Furnace Slag** (kg/m³)
3. **Fly Ash** (kg/m³)
4. **Water** (kg/m³)
5. **Superplasticizer** (kg/m³)
6. **Coarse Aggregate** (kg/m³)
7. **Fine Aggregate** (kg/m³)
8. **Age** (days: 1-365)

### Target Variable
- **Concrete Compressive Strength** (MPa)

### Dataset Characteristics
- **Instances**: 1,030
- **Missing Values**: None
- **Type**: Multivariate, Quantitative
- **Task**: Regression

## 🔬 Methodology

### Cross-Validation Strategy
- **K-Fold Cross-Validation** (K=10) for regression tasks
- **Stratified K-Fold** for classification to maintain class balance
- **Nested Cross-Validation** for hyperparameter tuning

### Model Evaluation Metrics
- **Regression**: Root Mean Squared Error (RMSE), R²
- **Classification**: Accuracy, Precision, Recall, F1-Score
- **Statistical Tests**: Paired t-tests, McNemar's test

## 📚 Key Learning Outcomes

This project demonstrates proficiency in:
- Exploratory data analysis and data visualization
- Feature engineering and dimensionality reduction (PCA)
- Implementing multiple ML algorithms (regression and classification)
- Model selection and hyperparameter tuning
- Cross-validation and statistical hypothesis testing
- Creating publication-quality visualizations
- Documenting and presenting technical work

## 📄 License & Attribution

Dataset usage requires attribution to:
> I-Cheng Yeh, "Modeling of strength of high performance concrete using artificial neural networks," *Cement and Concrete Research*, Vol. 28, No. 12, pp. 1797-1808 (1998).

## 👤 Author

**Christian Dunord**

This project showcases my skills in machine learning, data analysis, and statistical modeling as part of my academic portfolio.

---

⭐ If you find this project interesting or useful, please consider giving it a star!