# Predicting Insurance Claims Using Gini Index

## Project Overview

This project focuses on predicting whether a customer would make an insurance claim using a decision tree model based on the Gini index. The Gini index is used to evaluate the quality of potential splits in the dataset, ultimately leading to a decision tree that classifies whether a claim will be made.

## Objective

The goal of this project is to develop a decision tree model using the Gini index to predict insurance claims. The model's performance is evaluated by calculating the Gini index for different splits and determining the best split to improve classification accuracy.

## Data

The dataset includes the following features:
- **Gender**: The gender of the customer (e.g., Man, Woman).
- **Driving License Years**: The number of years the customer has held a driving license.
- **Car Category**: The type of car owned by the customer (e.g., Sedan, SUV, Sport).
- **Claim**: Whether the customer has made an insurance claim (1 for claim, 0 for no claim).

## Methodology

### 1. Gini Index Calculation
- **Full Dataset Gini Index**: Calculate the Gini index for the entire dataset before any splits to determine the initial impurity.
  - Gini Index: 0.46

### 2. Identifying the First Split Node
- **Splitting Based on Variables**: The dataset is evaluated for different potential splits based on features like Driving License Years and Car Category.
  - **Best First Split**: The Gini index is calculated for different thresholds, with the lowest Gini index indicating the best split.

### 3. Dataset Splitting and Further Node Selection
- **Left and Right Splits**: After the initial split, the dataset is divided into two subsets.
  - **Left Dataset**: Contains data points where the splitting condition is met.
  - **Right Dataset**: Contains data points where the splitting condition is not met.
  
- **Further Splitting**: The process is repeated on the left dataset to find additional nodes that further refine the decision tree.

### 4. Final Decision Tree Model
- **Tree Visualization**: A decision tree is constructed using the identified splits, allowing for the prediction of whether a customer will make a claim based on the features in the dataset.

## Files in This Repository

- **AutoInsuranceRisk_trees.xlsx**: The Excel file containing the dataset and the calculated Gini indices.
- **Hw7_Project_Report.pdf**: A detailed report outlining the project approach, methodology, results, and conclusions.

## Conclusion

This project successfully applies the Gini index to build a decision tree model for predicting insurance claims. By iteratively calculating the Gini index for potential splits, the model identifies the best variables and thresholds to improve classification accuracy.

For a detailed explanation, please check the Project_Report.pdf.
