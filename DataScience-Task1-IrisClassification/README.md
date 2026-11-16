# 🌸 Iris Flower Classification Using Machine Learning

## Oasis Infobyte Data Science Internship – Task 1

### Project Overview

This project implements a supervised machine learning classification system to identify Iris flower species based on their physical measurements.

Using Python and Scikit-learn, the project explores the complete Data Science workflow, from data preparation and exploratory data analysis (EDA) to model training, hyperparameter optimisation, evaluation and prediction.

Five machine learning algorithms are trained and compared to identify a suitable classification model.

**Project objective:** Build a reproducible machine learning pipeline that accurately classifies Iris flower species while demonstrating practical understanding of data science and machine learning techniques.

---

## 🎯 Business and Technical Objectives

The project aims to:

- Explore and understand the Iris dataset.
- Perform data inspection and exploratory data analysis.
- Identify patterns and relationships between flower measurements.
- Prepare numerical and categorical features for machine learning.
- Train and compare five classification algorithms.
- Evaluate model performance using multiple classification metrics.
- Apply cross-validation to assess model consistency.
- Optimise Random Forest hyperparameters using GridSearchCV.
- Evaluate the final tuned model using unseen test data.
- Generate predictions for new flower measurements.
- Save the trained model for future reuse.

---

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| Python | Programming language |
| Google Colab | Development environment |
| Pandas | Data manipulation and analysis |
| NumPy | Numerical computing |
| Matplotlib | Data visualisation |
| Seaborn | Exploratory data visualisation |
| Scikit-learn | Machine learning and model evaluation |
| Joblib | Model persistence |
| GitHub | Version control and project documentation |

---

## 📊 Dataset Description

The project uses the existing Iris dataset.

The dataset contains measurements of three Iris flower species:

- Iris Setosa
- Iris Versicolor
- Iris Virginica

The standard Iris dataset contains four numerical measurement features:

| Feature | Description |
|---|---|
| Sepal Length | Length of the flower's sepal |
| Sepal Width | Width of the flower's sepal |
| Petal Length | Length of the flower's petal |
| Petal Width | Width of the flower's petal |

**Target variable:** Iris Species

---

## 🔍 Project Workflow

The project follows an end-to-end machine learning workflow.

### 1. Data Inspection and Preparation

- Load the existing dataset.
- Inspect dataset dimensions and data types.
- Examine missing values.
- Review descriptive statistics.
- Separate input features from the target variable.

### 2. Exploratory Data Analysis (EDA)

Use data visualisation to understand the dataset.

Techniques include:

- Pair plots to explore relationships between features.
- Histograms to understand feature distributions.
- Box plots to examine feature variation.
- Species-based comparisons to identify distinguishing patterns.

### 3. Train-Test Split

Split the dataset into:

- 80% training data.
- 20% testing data.

Use stratified sampling to maintain species distribution across both datasets.

### 4. Data Preprocessing

Build a Scikit-learn preprocessing pipeline.

**Numerical features:**
- Missing-value imputation using the median.
- Feature standardisation using StandardScaler.

**Categorical features:**
- Missing-value imputation using the most frequent value.
- One-hot encoding using OneHotEncoder.

The preprocessing pipeline helps prevent data leakage by fitting transformations within the training workflow.

### 5. Machine Learning Model Development

Train and compare five classification algorithms:

1. Logistic Regression
2. Random Forest
3. Support Vector Machine (SVM)
4. K-Nearest Neighbors (KNN)
5. Decision Tree

Evaluate each model using:

- Accuracy
- Precision
- Recall
- F1-score

### 6. Model Performance Comparison

Compare the five algorithms using a performance table and accuracy visualisation.

The objective is to identify which algorithm performs best on the testing data.

### 7. Cross-Validation

Apply five-fold Stratified Cross-Validation to the training dataset.

Evaluate model consistency using:

- Mean cross-validation accuracy.
- Standard deviation.

The test dataset remains separate during cross-validation.

### 8. Hyperparameter Tuning

Use GridSearchCV to optimise the Random Forest classifier.

Parameters investigated include:

- Number of estimators: 100, 200 and 300.
- Maximum tree depth: None, 5 and 10.
- Minimum samples split: 2 and 5.
- Minimum samples leaf: 1 and 2.

The objective is to identify a suitable Random Forest configuration through cross-validation.

### 9. Final Model Evaluation

Evaluate the tuned Random Forest model against the previously unseen testing dataset.

Performance measurements include:

- Accuracy
- Precision
- Recall
- F1-score
- Classification report
- Confusion matrix

### 10. Feature Importance Analysis

Examine the importance of individual flower measurements in the Random Forest model.

Visualise feature importance to understand which measurements contribute most to the model's predictions.

### 11. New Flower Predictions

Use the trained model to classify new flower measurements.

The prediction pipeline also generates class probabilities where supported by the model.

### 12. Model Saving and Exporting

Save the complete trained machine learning pipeline using Joblib.

Export the following results into CSV files:

- Model comparison results.
- Cross-validation results.
- Feature importance results.
- Actual versus predicted species.

---

## 📈 Model Evaluation Metrics

| Metric | Purpose |
|---|---|
| Accuracy | Measures overall classification correctness |
| Precision | Measures how many positive predictions are correct |
| Recall | Measures how many actual class observations are identified |
| F1-score | Balances precision and recall |
| Confusion Matrix | Shows correct and incorrect classifications |
| Cross-validation | Assesses model performance consistency |

---

## 📁 Project Structure

```text
OIBSIP/
│
└── DataScience-Task1-IrisClassification/
    │
    ├── Iris_Flower_Classification.ipynb
    │
    ├── dataset/
    │   └── iris.csv
    │
    ├── models/
    │   └── iris_classification_model.pkl
    │
    ├── results/
    │   ├── model_comparison.csv
    │   ├── cross_validation_results.csv
    │   ├── feature_importance.csv
    │   └── prediction_results.csv
    │
    └── README.md
```

---

## 💡 Technical Considerations

The project follows important machine learning practices:

- Maintain separation between training and testing datasets.
- Perform cross-validation exclusively on training data.
- Apply preprocessing within machine learning pipelines.
- Evaluate models using multiple performance metrics.
- Test the final tuned model on unseen observations.
- Interpret model results rather than reporting accuracy alone.
- Save the complete preprocessing and prediction pipeline for reuse.

---

## 🚀 Project Deliverables

The completed project includes:

1. Documented Google Colab notebook.
2. Iris dataset.
3. Data cleaning and exploratory analysis.
4. Data visualisation outputs.
5. Five trained classification algorithms.
6. Model comparison report.
7. Cross-validation report.
8. Hyperparameter tuning results.
9. Final model evaluation.
10. Confusion matrix.
11. Feature importance analysis.
12. New prediction results.
13. Saved machine learning model.
14. GitHub project documentation.

---

## 🎓 Skills Demonstrated

- Python Programming
- Data Cleaning and Preparation
- Exploratory Data Analysis
- Statistical Data Analysis
- Data Visualisation
- Supervised Machine Learning
- Classification Algorithms
- Feature Engineering and Preprocessing
- Model Evaluation
- Cross-Validation
- Hyperparameter Optimisation
- Model Persistence
- GitHub Documentation

---

## 🏁 Conclusion

This project demonstrates the practical application of machine learning techniques to a classification problem.

By implementing a structured workflow covering data preparation, exploratory analysis, model development, optimisation and evaluation, the project demonstrates an understanding of the end-to-end Data Science lifecycle.

The resulting machine learning pipeline provides a reusable foundation for classifying Iris flower species using their physical measurements.

**Project:** Iris Flower Classification Using Machine Learning  
**Programme:** Oasis Infobyte Internship (OIBSIP)  
**Track:** Data Science  
**Task:** Task 1 – Iris Classification  
**Tools:** Python, Pandas, NumPy, Matplotlib, Seaborn and Scikit-learn

---

*Developed as part of the Oasis Infobyte Data Science Internship.*

