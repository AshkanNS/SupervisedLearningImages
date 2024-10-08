# Waste Classification with Machine Learning

This project applies supervised machine learning models to classify waste into two categories: Organic (O) and Recyclable (R). The classification is based on image data, and models like Logistic Regression and K-Nearest Neighbors (KNN) are used along with dimensionality reduction via PCA (Principal Component Analysis).

## Dataset

- The dataset consists of images categorized into two classes:
  - **O** (Organic)
  - **R** (Recyclable)
  
- The images are stored in two directories:
  - **TRAIN**: Used for training the models.
  - **TEST**: Used for testing the models.
  
Each of these directories contains subdirectories "O" and "R", representing the two classes.

The dataset was sourced from Kaggle.

## Exploratory Data Analysis (EDA)

During EDA, we:
- Counted the number of images in each category (O and R) for both training and testing sets.
- Visualized some of the sample images to understand the dataset better.
- Applied **PCA** to reduce the dimensionality of the image data for easier processing and visualization.

## Supervised Machine Learning Models

We used the following supervised machine learning models:

### 1. Logistic Regression:
- We applied **Logistic Regression** to the dataset after applying PCA for dimensionality reduction.
- We evaluated the model performance using classification metrics like accuracy, precision, recall, and F1-score.

### 2. K-Nearest Neighbors (KNN):
- We also tested the **KNN** algorithm with the PCA-transformed data.
- The model was evaluated using the same metrics.

### 3. Dimensionality Reduction with PCA:
- We reduced the number of features by applying **PCA** to the image data. This allowed us to optimize the model performance and reduce computational complexity.

## Results and Evaluation

- **Logistic Regression** performed reasonably well in classifying the images after PCA was applied.
- **KNN** was also tested, and we compared the performance of both models.
- **PCA** helped in reducing the dimensionality of the image data, which improved model performance by eliminating redundant information.

## Visualization

- We visualized the performance of the models using:
  - **Scatter plots** to compare true and predicted values.
  - **Confusion matrices** to show the correct and incorrect classifications.
  - **ROC curves** to evaluate model performance in terms of true positive rate vs false positive rate.

## How to Run the Project

### Prerequisites

- Install the following Python libraries:
  - `numpy`
  - `pandas`
  - `matplotlib`
  - `scikit-learn`
  - `umap-learn` (optional, for UMAP dimensionality reduction)

To install these, run:
```bash
pip install numpy pandas matplotlib scikit-learn umap-learn
