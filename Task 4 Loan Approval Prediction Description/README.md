# Loan Approval Prediction Project

## 📌 Project Description

This project aims to develop a machine learning model capable of predicting whether a bank loan application will be approved or rejected based on various applicant characteristics (income, credit score, assets, etc.). The provided Jupyter notebook contains the entire process, from data exploration to model evaluation.

---

## 📊 Project Structure

The notebook is organized into several sections:

1. **Library Installation and Import**
2. **Data Loading and Exploration**
3. **Data Cleaning and Preprocessing**
4. **Exploratory Data Analysis (EDA)**
5. **Data Preparation for Training**
6. **Model Training and Evaluation**
7. **Hyperparameter Optimization**
8. **Class Imbalance Management (SMOTE / UnderSampling)**
9. **Final Evaluation and Metrics**

---

## 🛠️ Technologies Used

- **Python 3**
- **Pandas / NumPy**: Data manipulation
- **Matplotlib / Seaborn**: Visualization
- **Scikit-learn**: ML models, preprocessing, evaluation
- **Imbalanced-learn**: Class imbalance management
- **Google Colab**: Execution environment

---

## 📁 Dataset

The dataset (`loan_approval_dataset.csv`) contains 4269 entries and 13 features, including:

- `loan_id`: Loan identifier
- `no_of_dependents`: Number of dependents
- `education`: Education level
- `self_employed`: Self-employed or not
- `income_annum`: Annual income
- `loan_amount`: Loan amount
- `loan_term`: Loan term
- `cibil_score`: Credit score
- `residential_assets_value`: Residential assets value
- `commercial_assets_value`: Commercial assets value
- `luxury_assets_value`: Luxury assets value
- `bank_asset_value`: Bank assets value
- `loan_status`: Loan status (Approved / Rejected)

---

## 🔍 Key Results

- **Class distribution**: 2656 approved loans, 1613 rejected (imbalance ratio ~0.61)
- **Tested models**: Logistic Regression, Decision Tree, Random Forest
- **Balancing techniques**: SMOTE and RandomUnderSampler
- **Evaluation metrics**: Accuracy, Precision, Recall, F1-score, AUC-ROC

---

## 🚀 How to Run the Project

1. Download the notebook and dataset.
2. Open the notebook in Google Colab or Jupyter.
3. Run the cells in order.
4. Make sure to import the `loan_approval_dataset.csv` file when Colab prompts you.

---

## 📈 Possible Improvements

- Try other models (XGBoost, LightGBM, etc.)
- Further hyperparameter optimization
- Additional feature engineering
- More extensive cross-validation

---

