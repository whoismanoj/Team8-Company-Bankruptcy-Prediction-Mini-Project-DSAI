## SC 1015: Data Science Mini Project - Bankruptcy Prediction

### Lab Group: PT1 (Team 8)

### Team Members: 

a.  Krishnadas Manoj
b.  Cao XingPing
c.  Keong Wee Kiat Edwin

### Introduction

This repository contains information referencing from Jupyter Notebooks, Datasets and Source Materials used as part of the project. In this project, Machine Learning are used for risk assessment in the prediction for bankruptcy of companies. Following which, the mentioned prediction can be obtained using suitable models, through various Machine Learning techniques. The purpose of this ReadMe file highlights the key summary accomplished in this project. Of note, readers can refer to the Jupyter Notebook, where the contents residing within the project offers in-depth descriptions, which are not mentioned here.

### Table of Contents:

1.  Introduction
2.  Problem Formulation
3.  Data Preparation / Cleaning
4.  Project FLow
5.  Conclusion
6.  Contributors

### 1.  Introduction

This is a project for Nanyang Technological Unviersity Singapore on SC1015 module (i.e. Introduction to Data Science and Artificial Intelligence). In this project, we chose to explore various machine learning models to predict the sucess of a company. 

### 2.  Problem Formulation

What are the key variables that determine the success of the company, and are we able to detect companies that are in the midst of bankruptcy through the result of various NLP modelling techniques?

### 3.  Data Preparation / Cleaning

Dataset Source: Company Bankruptcy Prediction from Kaggle. Please refer to the source [here.](https://www.kaggle.com/datasets/fedesoriano/company-bankruptcy-prediction)

Dataset Description: The dataset used contains financial rations of 5,606 comapnies, of which 220 have gone bankrupt.

Cleaned dataset: Please download from [here.](https://github.com/zentorno365/Company-Bankruptcy-Prediction-Mini-Project-DSAI/blob/main/Data_Source%20(cleaned)/data.csv)

### 4.  Project Flow

1.  Data Preparation: Clean and process the raw dataset
2.  Model Selection : Select the most relevant models
3.  Model Evaluation: Evaluate and report its performance metrics
4.  Results on findings and derived a conclusion

### Conclusion

Our regression model consists of various important predictors (i.e. "Bankruptcy Label", "Net Income to Total Assets", ""Total Debt to Total Assests", "EBIT to Total Assets Ration", "Market Value to Book Value Ratio", "Working Capital to Total Assests Ratio", "Current Liability to Assets Ratio", Sales to Total Assets Ratio" and "Cash Flow to Total Assets Ratio") and their coefficients were used to determine how much one variables have its impact on a company success.

On the other hand, the least relevant predictors were singled out to be (i.e. "Current Liability to CUrrent Assets", "Working Capital Turnover", "Working Capital to Fixed Assets", "Net Income to Total Assets", "Total Assets to GNP Price", "Quick Asset Ratio", "Borrowing Dependency", "Inventory and Accounts Receivable/Net Operating Revenue", "Operating Profit Per Person" and "Current Liability to Assets".

To further explain on the regression model.

### Learning Lesson

To eleaborate on our learning lesson.

### Contributors

a.  Krishnadas Manoj - Predictive Modeling, Predictive Modeling and Presentation Slides
b.  Cao XingPing - Data Preparation and Cleaning, Presentation Slides and Heatmap Visualisation
c.  Keong Wee Kiat Edwin - Basic Visualization, Writeup and Presentation Slides
