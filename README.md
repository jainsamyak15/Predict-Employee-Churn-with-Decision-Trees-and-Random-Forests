# Predict Employee Churn with Decision Trees and Random Forests

## Table of Contents

1. [Libraries Used](#libraries-used)
2. [Exploratory Data Analysis](#exploratory-data-analysis)
3. [Encoding Categorical Features](#encoding-categorical-features)
4. [Visualizing Class Imbalance](#visualizing-class-imbalance)
5. [Creating Training and Test Sets](#creating-training-and-test-sets)
6. [Building an Interactive Decision Tree Classifier](#building-an-interactive-decision-tree-classifier)
7. [Building an Interactive Random Forest Classifier](#building-an-interactive-random-forest-classifier)
8. [Feature Importance and Evaluation Metrics](#feature-importance-and-evaluation-metrics)
9. [Results and Outcomes](#results-and-outcomes)

## Libraries Used

The following libraries were imported and used throughout the project:

- numpy
- pandas
- matplotlib
- ydata_profiling (for generating data profiling reports)
- scikit-learn
- yellowbrick
- graphviz
- ipywidgets

## Exploratory Data Analysis

Exploratory Data Analysis (EDA) is performed on the `employee_data.csv` dataset. The notebook displays the first few rows of the dataset and generates a data profiling report using `ydata_profiling`. Additionally, bar plots are created to visualize the frequency of employee turnover based on salary and department.

## Encoding Categorical Features

Categorical features in the dataset, such as department and salary, are encoded using one-hot encoding.

## Visualizing Class Imbalance

The class imbalance in the target variable (employee churn) is visualized using the `ClassBalance` module from the `yellowbrick` library.

## Creating Training and Test Sets

The dataset is split into training and test sets using `train_test_split` from `scikit-learn`. The `stratify` parameter is used to maintain the class distribution in both sets.

## Building an Interactive Decision Tree Classifier

An interactive Decision Tree Classifier is built using the `DecisionTreeClassifier` class from `scikit-learn`. The notebook provides an interactive widget to adjust various hyperparameters of the Decision Tree, such as the criterion, splitter, maximum depth, minimum number of samples for splitting, and minimum number of samples for a leaf node. It displays the training and test accuracies, as well as a visualization of the learned tree.

## Building an Interactive Random Forest Classifier

An interactive Random Forest Classifier is built using the `RandomForestClassifier` class from `scikit-learn`. The notebook provides an interactive widget to adjust various hyperparameters of the Random Forest, such as the criterion, whether to use bootstrapping, maximum depth, number of trees in the forest, minimum number of samples for splitting, and minimum number of samples for a leaf node. It displays the training and test accuracies, as well as a visualization of one of the trees in the forest.

## Feature Importance and Evaluation Metrics

The importance of features is visualized using the `FeatureImportances` module from `yellowbrick` for both the Decision Tree and Random Forest models. Additionally, the Receiver Operating Characteristic (ROC) curves are plotted using the `ROCAUC` module from `yellowbrick` to evaluate the models' performance.

## Results and Outcomes

The notebook provides interactive visualizations and evaluations of the Decision Tree and Random Forest models for predicting employee churn. By adjusting the hyperparameters, users can explore the models' behavior and performance.
