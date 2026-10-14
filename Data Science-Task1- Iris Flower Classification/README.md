Project Overview

This project implements a machine learning classification system to predict the species of an Iris flower based on its sepal and petal measurements. It uses exploratory data analysis (EDA), data visualization, and supervised machine learning algorithms to compare model performance and identify the better-performing classifier.

The project demonstrates a complete beginner-friendly machine learning workflow, from understanding the dataset to evaluating and comparing trained models.

Problem Statement

Given four measurements of an Iris flower, predict which of the following three species it belongs to:

Setosa

Versicolor

Virginica

This is a multiclass classification problem because the target variable contains three possible classes.

Dataset

The project uses the Iris dataset available through scikit-learn.

Total observations: 150

Input features: 4

Target classes: 3

Missing values: None

Features

Feature

Description

Sepal Length

Length of the sepal in centimeters

Sepal Width

Width of the sepal in centimeters

Petal Length

Length of the petal in centimeters

Petal Width

Width of the petal in centimeters

The target variable represents the Iris species, encoded numerically.

Technologies Used

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

Jupyter Notebook

Project Workflow

1. Data Loading and Inspection

Loaded the Iris dataset into a Pandas DataFrame and examined its structure, dimensions, data types, descriptive statistics, and missing values.

2. Exploratory Data Analysis (EDA)

Performed exploratory analysis to understand feature distributions and relationships.

Visualizations included:

Pairplot to examine relationships between features and species.

Boxplots to compare feature distributions across target classes.

A correlation heatmap to examine relationships between numerical features.

The exploratory analysis highlighted the importance of petal measurements in distinguishing Iris species.

3. Feature Selection

Used all four available measurements as input features:

Sepal length

Sepal width

Petal length

Petal width

The target species was separated from the input features before model training.

4. Train-Test Split

Split the dataset into training and testing sets using an 80:20 ratio. Stratified sampling was used to preserve the class distribution in both sets.

Training samples: 120

Testing samples: 30

A fixed random state was used for reproducibility.

5. Model Training

Two supervised machine learning classifiers were trained and evaluated.

Logistic Regression

Used as a classification baseline.

Predicts the probability of each species belonging to a particular class.

Random Forest Classifier

An ensemble learning algorithm based on multiple decision trees.

Combines tree predictions to classify observations.

6. Model Evaluation

The models were evaluated using the following metrics:

Accuracy: Proportion of correctly classified observations.

Precision: Proportion of positive predictions that are correct, calculated using macro averaging across classes.

Recall: Proportion of actual class observations correctly identified, calculated using macro averaging.

F1-score: Harmonic mean of precision and recall, calculated using macro averaging.

Confusion Matrix: Shows correct predictions and misclassifications for each class.

Classification Report: Provides class-wise precision, recall, F1-score, and support.

A metric comparison visualization was created to compare both classifiers.

Results

On the current train-test split, the models achieved the following accuracy scores:

Model

Test Accuracy

Logistic Regression

96.67%

Random Forest

90.00%

Best-performing model on this test split: Logistic Regression.

Logistic Regression correctly classified 29 out of 30 test observations, while Random Forest correctly classified 27 out of 30.

These results apply to this particular test split and do not guarantee that Logistic Regression will outperform Random Forest on every dataset or split.

Key Learnings

Conducting exploratory data analysis before model training.

Understanding feature distributions and correlations.

Preparing input features and target labels for supervised learning.

Performing stratified train-test splitting.

Training and evaluating multiclass classification models.

Interpreting accuracy, precision, recall, F1-score, and confusion matrices.

Comparing multiple models and justifying model selection using evaluation metrics.

Creating visualizations to communicate model performance.

Project Structure

Iris-Flower-Classification/
│
├── iris_classification.ipynb
├── README.md

Update the notebook filename and folder structure if your repository uses different names.

Installation and Usage

1. Clone the repository

git clone https://github.com/PunyaMehta2006/OIBSIP
cd Iris-Flower-Classification

2. Install dependencies

pip install -r requirements.txt

3. Run the notebook

jupyter notebook

Open iris_classification.ipynb and execute the cells in sequence.

Dependencies

If you do not already have a requirements.txt file, create one containing:

pandas
numpy
matplotlib
seaborn
scikit-learn
jupyter

Future Improvements

Evaluate model stability using stratified cross-validation.

Tune hyperparameters for both classifiers.

Compare additional algorithms, such as Support Vector Machines and K-Nearest Neighbors.

Visualize decision boundaries for selected features.

Save the trained model and build a simple interface for making predictions on new flower measurements.

Conclusion

This project demonstrates an end-to-end machine learning classification workflow using the Iris dataset. Through exploratory data analysis, model training, evaluation, and metric visualization, Logistic Regression emerged as the better-performing model on the current test split.