# Diabetes Prediction Model

This project focuses on developing a classification model to predict the likelihood of an individual developing diabetes over the next 5 years, based on various health parameters. The model is designed to assist in early detection, enabling timely intervention and improved health outcomes.

## Problem Statement

Diabetes is a chronic condition with serious implications for individual health and well-being. Early diagnosis is crucial to reducing the risk and long-term effects of the disease. This project aims to build a predictive model that can classify whether an individual is likely to develop diabetes in the near future, based on medical and personal data.

## Data Preparation

The dataset contains health records of 678 individuals, with the following features:
- **Pregnancies**: Number of times the individual has been pregnant
- **Glucose**: Plasma glucose concentration
- **Blood Pressure**: Diastolic blood pressure (mm Hg)
- **Skin Thickness**: Triceps skinfold thickness (mm)
- **Insulin**: 2-hour serum insulin (mu U/ml)
- **BMI**: Body Mass Index (weight in kg/(height in m)^2)
- **Diabetes Pedigree Function**: A function that scores the likelihood of diabetes based on family history
- **Age**: The age of the individual (years)

### Data Preprocessing

1. **Handling Missing Values**: Missing values were identified and appropriately handled to avoid bias in model predictions.
2. **Outlier Detection**: Outliers were managed to ensure that the dataset provided reliable input to the models.
3. **Feature Selection**: Features were carefully selected based on their relevance and importance to the prediction of diabetes.

## Model Development

Five machine learning algorithms were employed to build classification models:

1. **Logistic Regression**: 
   - A linear model suitable for binary classification tasks. It provides interpretability and is effective for baseline performance.
   
2. **K-Nearest Neighbors (KNN)**:
   - A non-parametric, instance-based learning method that captures complex patterns and relationships in the data.

3. **Support Vector Machine (SVM)**:
   - A robust algorithm capable of modeling both linear and non-linear decision boundaries using various kernel functions.

4. **Random Forest**:
   - An ensemble learning method that aggregates multiple decision trees to improve accuracy and control overfitting.

5. **XGBoost**:
   - A high-performance gradient boosting algorithm known for its scalability, speed, and accuracy.

### Model Training and Hyperparameter Tuning

Each model was trained using the preprocessed dataset. To improve the performance of each classifier, hyperparameter tuning was performed, optimizing parameters such as learning rate, number of trees, kernel functions, and others specific to each algorithm. The goal was to enhance model accuracy and generalization on unseen data.

## Results

The models were evaluated based on key metrics such as accuracy, precision, recall, and F1-score to compare their effectiveness. Further details on the performance of each model are available in the notebook.

## How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/AmoolyaS/diabetes-prediction-case-study.git
