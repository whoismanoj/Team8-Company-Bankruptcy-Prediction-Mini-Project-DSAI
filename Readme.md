## SC 1015: Data Science Mini Project - Company Bankruptcy Prediction

### Lab Group: PT1 (Team 8)

### Team Members: 

1.  Krishnadas Manoj
2.  Cao XingPing
3.  Keong Wee Kiat Edwin

### Introduction

This repository contains information referencing from Jupyter Notebooks, Datasets and Source Materials used as part of the project. In this project, Machine Learning are used for risk assessment in the prediction for bankruptcy of companies. Following which, the mentioned prediction can be obtained using suitable models, through various Machine Learning techniques. The purpose of this ReadMe file highlights the key summary accomplished in this project. Of note, readers can refer to the Jupyter Notebook, where the contents residing within the project offers in-depth descriptions, which are not mentioned here.

### Table of Contents:

1.  Introduction
2.  Problem Formulation
3.  Data Preparation / Cleaning
4.  Project Flow
5.  Conclusion
6.  Contributors

### 1.  Introduction

This is a project for Nanyang Technological Unviersity Singapore on SC1015 module (i.e. Introduction to Data Science and Artificial Intelligence). In this project, we chose to explore various machine learning models to predict the success of a company. 

### 2.  Problem Formulation

What are the key predictors that determine the success of the company, and are we able to detect companies that are in the midst of bankruptcy through the result of various NLP modelling techniques?

### 3.  Cleaning / Data Preparation

Dataset Source: Company Bankruptcy Prediction from Kaggle. Please refer to the source [here.](https://www.kaggle.com/datasets/fedesoriano/company-bankruptcy-prediction)

Dataset Description: The dataset used contains financial rations of 5,606 comapnies, of which 220 have gone bankrupt.

A challenging aspect is that the dataset consists of too much information. It poses a challenge for us to analyse the complexity of data and modeling, that requires more computational resources which results in slower performance and longer processing time. 

Apart from performing basic cleaning checks on our raw data, our approach is to first identify critical predictors that are essential to the determining of the final result, which helps us to understand the structure and characteristics of the dataset before cleaning the dataset.

### 4.  Project Flow

1.  Data Preparation: Basic cleaning and processing of raw dataset
2.  Data Analysis: Determine the critical variables and do further cleaning to the dataset
3.  Model Selection : Select the most relevant models
4.  Model Evaluation: Evaluate and report its performance metrics
5.  Results on findings and derived a conclusion

### Conclusion

Our regression model consists of 19 important predictors (i.e. "Operating Gross Margin", "Operating Profit Rate", "Research and development expense rate", "Cash flow rate", "Interest-bearing debt interest rate", "Revenue Per Share (Yuan ¥)", "Total Asset Growth Rate", "Cash Reinvestment %", "Borrowing dependency", "Average Collection Days", "Fixed Assets Turnover Frequency", "Allocation rate per person", "Working Capital/Equity", "Long-term Liability to Current Assets", "Total expense/Assets", "Cash Turnover Rate", "Fixed Assets to Assets", "Total assets to GNP price" and "Bankrupt?") and their coefficients were used to determine how much one variables have its impact on a company success.

On the other hand, the 77 least relevant predictors were singled out and filtered off, to help improves the quality of the data to achieve the effectiveness of data analysis and modeling.

After deep analysis of the results from the begining, here's the summary of what we discovered and suggest:

1.  ‘Liability-Assets Flag’ - If Total Liability exceeds Total Assets, there is a high chance of bankruptcy.
2.  ‘Debt Ratio’, ‘Current Liability to Assets’, ‘Borrowing Dependency’, ‘Liability to equity’, ‘Expense to Assets’ these predictors have a good positive correlation with bankruptcy
3.  ‘Net_Income_Flag’ only had value for one category in the data that we had. Thus, we could not utilize it.
4.  'Net Income to Total Assets', 'ROA before interest and % after tax', 'Net worth/Assets', 'Persistent_EPS_in_the_Last_Four_Seasons', 'Retained_Earnings_to_Total_Assets' - these predictors are highly negatively correlated with bankruptcy.

### Learning Lesson

To begin with, there was high class imbalance in the data (i.e. Only 3.2 % of total records) were bankrupt companies. Notably, the minority class is too small to be modeled effectively. To solve this issue, we used a technique called "Oversampling", to balance the imbalanced dataset. SMOTE (Synthetic Miniority Oversampling Technique) was used, as it creates realistic synthetic data sample for the minority classes, by interpolating between the selected observation and the chosen neighbour, based on a random ratio. This help improves the accuracy of models trained on the imbalanced datasets.

Following which, we combined a performance evaluation tool (i.e. Confusion Matrix) to summarizes the amount of correct and incorrect predictions made by the model on a test set, which is used to calculate various metrics, such as precision and recall.

![image](https://user-images.githubusercontent.com/128292326/231409055-e571384a-fc5b-40e4-97f3-8273ad187223.png)

#### -1*(Photo above shows the illustration of the heatmap, which illustrate the correlation between predictors.)

Through the aforementioned conclusion and learning lesson, we managed to meet the ojective by building a classifier that have the best predictive ability to identify unstable companies that might go bankrupt.

### Contributors

1.  Krishnadas Manoj - Predictive Modeling, Basic Visualization and Presentation Slides
2.  Cao XingPing - Data Preparation and Cleaning, Presentation Slides and Heatmap Visualisation
3.  Keong Wee Kiat Edwin - Basic Visualization, Writeup and Presentation Slides

