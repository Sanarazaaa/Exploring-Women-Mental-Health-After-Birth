# Exploring-Women-Mental-Health-After-Birth

This project involves the analysis of a maternal health dataset to explore factors that contribute to postpartum depression and bonding between mothers and their children. The dataset includes information on age, BMI, blood pressure, complications, and bonding scores, among other variables.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset Overview](#dataset-overview)
- [Data Preprocessing](#data-preprocessing)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Modeling](#modeling)
- [Statistical Tests](#statistical-tests)
- [Clustering](#clustering)
- [Conclusion](#conclusion)
- [Requirements](#requirements)
- [Installation](#installation)

## Project Overview

The goal of this project is to analyze maternal health data, identify patterns, and develop predictive models to assess the likelihood of postpartum depression. The aim is to understand how various health indicators like age, BMI, and blood pressure contribute to mental well-being post-pregnancy.

## Dataset Overview

The dataset contains 200 records and the following columns:
- **Age**: The age of the mother (in years)
- **BMI**: Body Mass Index of the mother
- **Blood Pressure**: Systolic blood pressure of the mother
- **Complications**: Whether the mother experienced pregnancy complications (1 for Yes, 0 for No)
- **Postpartum Depression**: Whether the mother experienced postpartum depression (1 for Yes, 0 for No)
- **Bonding Score**: A score representing the bonding between mother and child

## Data Preprocessing

I performed the following preprocessing steps:
- Checked for missing values and ensured there were none.
- Converted categorical variables (e.g., `Complications` and `Postpartum Depression`) into numerical values for analysis.
- Standardized numerical features for the modeling phase.

## Exploratory Data Analysis

I conducted an exploratory data analysis (EDA) to uncover insights from the dataset:
- Visualized the distribution of age, BMI, blood pressure, and bonding scores.
- Used a correlation matrix to examine relationships between variables.
- Created box plots to analyze the impact of complications and depression on bonding scores.

## Modeling

I developed a **Random Forest Classifier** to predict the likelihood of postpartum depression:
- **Accuracy**: 70%
- **Precision for non-depressed mothers**: 78%
- **Recall for non-depressed mothers**: 88%
- **Precision for depressed mothers**: 0%
- **Recall for depressed mothers**: 0%

The model was effective in identifying non-depressed mothers but struggled with predicting depression due to class imbalance.

## Statistical Tests

I used T-tests to compare the means of various features between mothers with and without postpartum depression. The tests showed no significant differences in age, BMI, blood pressure, or bonding scores.

## Clustering

K-Means clustering was applied to segment mothers into 3 groups based on their health indicators. The clustering revealed distinct groups that could be helpful for understanding different health profiles among mothers.

## Conclusion

- The analysis provided insights into maternal health, though the dataset did not show strong predictors for postpartum depression.
- Further improvements to the predictive model can be made by addressing class imbalance and experimenting with different algorithms.
- Additional data on social, psychological, and environmental factors may help improve our understanding of postpartum depression.

## Requirements

The following Python libraries are required to run the project:
- pandas
- numpy
- matplotlib
- seaborn
- sklearn
- scipy

