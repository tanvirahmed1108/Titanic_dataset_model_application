Project Overview
This project is a comprehensive machine learning exercise focused on the fundamental stages of a data science workflow: Data Preprocessing, Exploratory Data Analysis (EDA), Model Training, and Evaluation.

Using the Titanic dataset, the goal was adapted for a multi-class classification task: predicting the Embarked (Port of Embarkation: C, Q, or S) of a passenger based on other features.

The project demonstrates the application and comparative analysis of five different classification algorithms.

Goal
To build and evaluate five distinct classification models capable of predicting the Port of Embarkation (Embarked) of a passenger using demographic and travel-related features (Pclass, Sex, Age, Fare, etc.).

Methodology
1. Data Preprocessing & EDA
Data Cleaning Handled missing values (Age, Fare) using median imputation. Dropped highly sparse feature (Cabin). Feature Engineering Dropped unique identifiers (Name, Ticket, PassengerId). Encoding One-Hot Encoding for categorical features in X (Sex, Pclass). Label Encoding for the multi-class target y (Embarked). Scaling Applied StandardScaler to numerical features (Age, Fare, SibSp, Parch). Split Used an 80/20 split for Training and Testing sets (stratified).

2. Visualization Requirements
Generated Histograms for feature distribution. Plotted Scatter Plots to visualize feature relationships (e.g., Age vs. Fare colored by Embarked). Created a Correlation Heatmap to analyze feature collinearity.

3. Machine Learning Models
Five classification algorithms were trained and evaluated:

Logistic Regression (Multi-class: Multinomial)

K-Nearest Neighbors (KNN)

Decision Tree Classifier

Random Forest Classifier

Support Vector Machine (SVM) (One-vs-Rest)

Model Evaluation
For each model, the following metrics and visualizations were generated:

Confusion Matrix Plot Visual analysis of true positives, false positives, etc. Classification Report Precision, Recall, and F1-score for each class. ROC Curve (One-vs-Rest strategy for the Logistic Regression model) Learning Curve (Training Score vs. Cross-validation Score)
