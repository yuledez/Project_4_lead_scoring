# Optimizing Lead Conversion with Machine Learning Models

## Table of Contents
1. [Project Overview](#project-overview)
2. [Data Overview](#data-overview)
3. [Methodology](#methodology)
   - [Data Cleaning and Preprocessing](#1-data-cleaning-and-preprocessing)
   - [Exploratory Data Analysis (EDA)](#2-exploratory-data-analysis-eda)
   - [Model Building](#3-model-building)
   - [Model Evaluation](#4-model-evaluation)
4. [Tools and Technologies](#tools-and-technologies)
5. [Project Timeline](#project-timeline)
6. [Key Deliverables](#key-deliverables)
7. [Success Criteria](#success-criteria)
8. [Conclusion](#conclusion)
   - [Class Imbalance](#class-imbalance)
   - [Final Results](#final-results)
   - [Business Impact](#business-impact)
9. [Recommendation](#recommendation)
10. [Code Schema/Table of Contents](#code-schematable-of-contents)

---

## Project Overview

This project aims to develop a predictive model to improve lead conversion rates for X Education, which currently stands at 38%. The existing process relies on manual lead scoring based on limited data and employee intuition, leading to inefficiencies and missed opportunities.

By leveraging predictive modeling, we assign a conversion score to each lead, allowing the sales team to focus on high-potential prospects and allocate their time more effectively. The model will enhance the current manual process by using data-driven insights, improving both the accuracy and efficiency of lead prioritization.

#### Key Metrics:
- **Precision**: Ensures the team spends less time on false positives, focusing on high-value prospects.
- **Recall**: Ensures a broad range of potential leads are captured, preventing missed opportunities and optimizing the sales funnel.

Ultimately, this project aims to streamline the sales process, improve lead conversion rates, and reduce time spent on low-potential leads, resulting in better overall sales efficiency.

---

## Data Overview

The dataset consists of 9,241 rows and 37 columns sourced from Kaggle, capturing features such as:
- Lead origin
- Engagement metrics
- Historical conversion outcomes
- Numerical and categorical variables (e.g., time spent on the website, response to marketing campaigns).

---

## Methodology

### 1. **Data Cleaning and Preprocessing**
   - Handling missing values, outliers, and categorical data encoding.
   - Standardizing numeric values using scaling techniques.

### 2. **Exploratory Data Analysis (EDA)**
   - Analyzing distributions and correlations between features.
   - Feature Engineering: Creating new variables based on user engagement levels.

### 3. **Model Building**
   - Testing multiple models: Logistic Regression (baseline), Random Forest, Neural Networks.
   - Hyperparameter tuning for optimization (GridSearchCV, Keras Tuner).

### 4. **Model Evaluation**
   - Evaluating models using precision, recall, F1 score, and accuracy.

---

## Tools and Technologies

- **Languages**: Python
- **Libraries**: Pandas, Scikit-learn, Matplotlib, TensorFlow/Keras
- **Tools**: Jupyter Notebook, GitHub, Kaggle (dataset), Keras Tuner (for hyperparameter optimization)

---

## Project Timeline

- **09/22 - 09/28**: Data collection, cleaning, and EDA
- **09/29 - 10/05**: Model building and testing
- **10/06 - 10/12**: Model evaluation and optimization
- **10/13 - 10/17**: Final report and presentation

---

## Key Deliverables

- A cleaned, preprocessed dataset ready for modeling.
- Trained and evaluated models with performance metrics like precision, recall, F1 score, and accuracy.
- Visualizations of model performance and key insights.
- A presentation showcasing the project's impact.

---

## Success Criteria

- **Accuracy**: Achieving over 85% (targeting 94% based on preliminary tests).
- **Precision & Recall**: Ensuring effective prioritization of high-conversion leads.
- **Efficiency**: Reducing time spent on low-potential leads.

---

## Conclusion

The goal of this project was to boost lead conversion rates (starting at 38%) by building a predictive model to better identify high-potential leads. Multiple models were tested, including:
- Logistic Regression (baseline)
- PCA optimization for Logistic Regression
- Random Forest
- Hyperparameter Tuning (GridSearchCV)
- Deep Learning (Keras Tuner)

### Class Imbalance
The dataset presented a class imbalance, with more "not converted" leads (5,594) compared to "converted" leads (3,425). Despite this, the models performed well due to effective feature engineering and data preprocessing. The success criteria—achieving over 85% accuracy—was met across all models.

### Final Results
- **Accuracy**: Models achieved between 92% - 94%.
- **Precision**: Up to 95%, reducing false positives and improving focus on high-quality leads.
- **Recall**: As high as 90%, ensuring that valuable opportunities weren’t missed.
- **F1 Score**: Balanced precision and recall, with up to 92% across models.

### Business Impact
The predictive model helps the sales team focus on the most promising leads, leading to increased conversions with less effort. By automating lead scoring, the team can work more efficiently, reducing operational costs and improving sales outcomes.

---

## Recommendation

Based on the evaluation, the **Random Forest model with Hyperparameter Tuning** is recommended for deployment. It offers the best balance between precision, recall, and accuracy, making it the optimal solution for prioritizing high-quality leads and boosting conversions.

---

## Code Schema/Table of Contents

1. **Import Dependencies**
2. **Data Preprocessing**
   - Data Loading
   - Data Inspection
   - Exploratory Data Analysis (EDA)
     - Handling "Select" Values
     - Standardizing Column Names
     - Calculating Missing Values
     - Dropping Columns with Excessive Missing Data
     - Individual Feature Analysis
     - Correlation Heatmap of Numerical Features
   - Clean Data Frame
   - Feature Engineering and Transformation
     - Numerical Scaling
     - Categorical Encoding
3. **Model Implementation**
   - Define Target Variable
   - Calculate Baseline
     - Conversion Ratio
     - Naive Prediction
   - Supervised Learning
     - Logistic Regression
     - Random Forest
     - Deep Learning (Neural Networks)
4. **Conclusions**
   - Model Performance

---

## UCB-Data-Proj4 
### UCBerkeley-Ext Data Analytics Bootcamp Project 4 

Yuleica Ledezma

**Special Acknowledgment to Elias, Brian, and Karen  their invaluable support and guidance throughout the project.**


