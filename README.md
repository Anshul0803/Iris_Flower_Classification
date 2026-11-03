Iris Flower Classification Using Machine Learning

Project Overview

This project implements a supervised machine learning classification system to predict the species of an Iris flower based on its physical measurements.

The project uses the Iris dataset to train and evaluate two classification algorithms: Logistic Regression and Decision Tree Classifier. Their performance is compared using multiple evaluation metrics, including accuracy, precision, recall, and F1-score.

The project demonstrates the complete machine learning workflow, from data exploration and preprocessing to model training, evaluation, and visualization.

Objectives

* Load and explore the Iris dataset using Pandas.
* Perform Exploratory Data Analysis (EDA) using Seaborn and Matplotlib.
* Standardize numerical features using StandardScaler.
* Split the dataset into training and testing sets using an 80:20 ratio.
* Train Logistic Regression and Decision Tree classification models.
* Evaluate both models using accuracy, precision, recall, and F1-score.
* Visualize classification results using confusion matrix heatmaps.
* Plot decision boundaries to understand how the models separate different flower species.
* Compare the performance of both classification algorithms.

Dataset Description

The Iris dataset contains measurements of three Iris flower species:

* Iris Setosa
* Iris Versicolor
* Iris Virginica

Each flower is described using four numerical features:

Feature	Description
Sepal Length	Length of the sepal in centimetres
Sepal Width	Width of the sepal in centimetres
Petal Length	Length of the petal in centimetres
Petal Width	Width of the petal in centimetres
Species	Target class representing the flower species

The standard Iris dataset contains 150 observations, with 50 samples belonging to each species.

Technologies Used

* Python — Programming language
* Pandas — Data manipulation and analysis
* NumPy — Numerical computations
* Matplotlib — Data visualization
* Seaborn — Statistical visualization and heatmaps
* Scikit-Learn — Machine learning models, preprocessing, and evaluation
* Jupyter Notebook — Interactive development environment

Project Workflow

1. Data Loading and Exploration

The dataset is loaded into a Pandas DataFrame. Initial exploration includes inspecting the dataset structure, column names, data types, missing values, and statistical summaries.

2. Exploratory Data Analysis

Data visualization is performed to understand the relationships between features and the distribution of the target classes.

The visualizations include:

* Species distribution count plot
* Pairplot of numerical features
* Feature correlation heatmap

These visualizations help identify patterns that may be useful for classification.

3. Data Preprocessing

The dataset is divided into input features (X) and the target variable (y).

The data is split into:

* 80% training data for model training
* 20% testing data for model evaluation

StandardScaler is used to standardize the numerical features. The scaler is fitted on the training data and then applied to the test data to prevent data leakage.

4. Model Training

Two supervised classification algorithms are implemented.

Logistic Regression

Logistic Regression estimates class probabilities and predicts the most likely flower species. It provides a baseline classification model for comparing performance.

Decision Tree Classifier

The Decision Tree Classifier learns a sequence of feature-based decision rules to classify flower species. It can model nonlinear decision boundaries.

Both models are trained using the prepared training dataset.

5. Model Evaluation

The trained models are evaluated using the following metrics:

Metric	Purpose
Accuracy	Measures the proportion of correctly classified samples
Precision	Measures the reliability of positive predictions for each class
Recall	Measures how many actual samples of each class are correctly identified
F1-Score	Combines precision and recall into a single metric

Macro-averaged precision, recall, and F1-score are used to give equal weight to each species.

Classification reports provide additional class-wise performance details.

6. Confusion Matrix Visualization

Confusion matrix heatmaps are generated for both models.

They compare actual species labels with predicted species labels, making it easier to identify correct classifications and misclassified observations.

7. Decision Boundary Visualization

Decision boundaries are visualized using petal length and petal width.

Separate two-feature models are trained for these plots because the original dataset contains four features and cannot be represented directly in a two-dimensional graph.

The visualizations illustrate how Logistic Regression and Decision Tree divide the feature space into predicted classes.

8. Model Comparison

The accuracy, precision, recall, and F1-score of both models are compared using a results table and a bar chart.

The final comparison helps determine which model performs better on the selected test set.

Results

The notebook generates:

* Dataset exploration and statistical summaries
* Species distribution plot
* Feature pairplot
* Feature correlation heatmap
* Logistic Regression classification report
* Decision Tree classification report
* Model performance comparison table
* Performance comparison bar chart
* Confusion matrix heatmaps for both models
* Decision boundary plots for both models