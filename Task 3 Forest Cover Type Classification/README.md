
# Forest Cover Type Classification

## Description
This project uses machine learning techniques to classify forest cover types based on geographic and environmental data. The dataset comes from the UCI Machine Learning Repository.

## Objective
To build and evaluate several classification models to predict the forest cover type among 7 possible classes.

## Dataset
- **Source**: [UCI Machine Learning Repository - Forest Covertype](https://archive.ics.uci.edu/ml/datasets/Covertype)
- **Size**: 581,012 samples, 54 features
- **Features**:
  - 10 numerical variables (elevation, slope, distance to hydrology, etc.)
  - 44 binary variables (wilderness areas and soil types)
- **Target**: `Cover_Type` (7 classes)

## Preprocessing
- Normalization of numerical features using `StandardScaler`
- No missing values detected

## Models Used
- Logistic Regression
- Decision Tree
- Random Forest
- XGBoost

## Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

## Project Structure
- `Forest_Cover_Type_Classification.ipynb`: Main notebook containing all the code
- `covtype.data.gz`: Dataset downloaded from UCI

## How to Run
1. Download the notebook and the dataset.
2. Run the cells in order.
3. The necessary libraries are listed at the beginning of the notebook.

## Results
Model performances are compared at the end of the notebook.

