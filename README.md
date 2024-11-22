![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

---

# Diabetes Prediction Machine Learning Project

## Overview

This project aims to predict the likelihood of diabetes based on various health-related factors. The dataset includes features such as age, gender, cholesterol levels, physical activity, smoking habits, and more. The goal is to classify individuals into two categories: those with diabetes and those without, based on the provided attributes.

## Dataset

The dataset consists of the following columns:

- **Age**: Age category of the individual.
- **Sex**: Gender (1 = male; 0 = female).
- **HighChol**: Whether the individual has high cholesterol (1 = yes; 0 = no).
- **CholCheck**: Whether the individual had a cholesterol check in the last 5 years (1 = yes; 0 = no).
- **BMI**: Body Mass Index (continuous variable).
- **Smoker**: Whether the individual has smoked at least 100 cigarettes in their lifetime (1 = yes; 0 = no).
- **HeartDiseaseorAttack**: Whether the individual has coronary heart disease or a history of myocardial infarction (1 = yes; 0 = no).
- **PhysActivity**: Whether the individual has engaged in physical activity in the past 30 days (1 = yes; 0 = no).
- **Fruits**: Whether the individual consumes fruit at least once per day (1 = yes; 0 = no).
- **Veggies**: Whether the individual consumes vegetables at least once per day (1 = yes; 0 = no).
- **HvyAlcoholConsump**: Whether the individual consumes alcohol heavily (1 = yes; 0 = no).
- **GenHlth**: General health rating (1 = excellent; 5 = poor).
- **MentHlth**: Number of days with poor mental health in the past 30 days.
- **PhysHlth**: Number of days with poor physical health in the past 30 days.
- **DiffWalk**: Whether the individual has serious difficulty walking or climbing stairs (1 = yes; 0 = no).
- **Stroke**: Whether the individual has had a stroke (1 = yes; 0 = no).
- **HighBP**: Whether the individual has high blood pressure (1 = yes; 0 = no).
- **Education**: Education level (scale 1-6).
- **Income**: Annual income level (scale 1-8).
- **Diabetes (Target)**: The target variable indicating diabetes status (0 = no diabetes; 1 = prediabetes; 2 = diabetes).

## Data Preprocessing

- **Downsampling**: The target variable was imbalanced, with more individuals classified as non-diabetic. To address this, downsampling was applied to the target variable to balance the classes.
  
- **Binarization**: For the purpose of classification, the prediabetic class (value 1) was merged with the diabetic class (value 2), creating a binary target variable (0 = non-diabetic; 1 = diabetic).

## Exploratory Data Analysis (EDA)

The dataset was first explored through statistical analysis and visualizations, including:

- Descriptive statistics (mean, median, mode, standard deviation).
- Visualizations such as histograms, box plots, and correlation matrices to understand the distribution of features and relationships between variables.
- Outlier detection and handling.

## Machine Learning

Several machine learning models were tested, including:

- Logistic Regression
- Decision Trees
- Support Vector Machines (SVM)
  
Model performance was evaluated using metrics such as accuracy, precision, recall, and F1-score.

## Improvements

- Model hyperparameter tuning was performed to enhance performance.
- Further preprocessing steps, including feature scaling and encoding, were applied to improve model accuracy.

## Requirements

- Python 3.x
- Libraries: pandas, numpy, scikit-learn, matplotlib, seaborn

## How to Run the Project

1. Clone this repository to your local machine.
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter notebooks:
   - `EDA.ipynb`: Performs the exploratory data analysis.
   - `ML.ipynb`: Includes the machine learning modeling and evaluation.

## Conclusion

This project provides insights into predicting diabetes based on various health attributes. It demonstrates the use of preprocessing techniques, machine learning models, and performance improvement strategies to create an effective predictive model.

---
