# Credit Card Fraud Detection

This project focuses on detecting fraudulent credit card transactions using a publicly available dataset. The primary objective is to classify transactions as fraudulent or legitimate based on anonymized features derived through PCA (Principal Component Analysis).

## Project Overview

Credit card fraud detection is a critical problem in the finance industry. This project leverages machine learning techniques, including logistic regression, to build a model capable of identifying fraudulent transactions effectively.

### Dataset Information

- **Source**: The dataset is publicly available on [Kaggle](https://www.kaggle.com).
- **Features**:
  - `Time`: Seconds elapsed since the first transaction in the dataset.
  - `V1` to `V28`: Anonymized features derived from PCA.
  - `Amount`: The transaction amount.
- **Target**:
  - `Class`: A binary variable where `1` indicates a fraudulent transaction and `0` indicates a legitimate one.
- **Size**: 284,807 transactions across 31 columns.

### Key Highlights

- The dataset is highly imbalanced, with fraudulent transactions constituting a small fraction of the total.
- To address this, random undersampling was performed on legitimate transactions, selecting a balanced subset of 492 records for modeling.
- Logistic regression is employed as the primary classification model, focusing on distinguishing between fraudulent and legitimate transactions.

## Methodology

### 1. Data Preprocessing

- Verified the absence of missing values.
- Scaled the `Amount` and `Time` features for compatibility with the model.

### 2. Modeling

- Logistic regression was chosen due to its interpretability and effectiveness for binary classification tasks.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/winter000boy/credit-card-fraud-detection.git
