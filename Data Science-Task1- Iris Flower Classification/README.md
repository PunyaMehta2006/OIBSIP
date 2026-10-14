# Iris Flower Classification Using Machine Learning

## Project Overview

This project implements a machine learning classification system to predict Iris flower species based on their sepal and petal measurements. The primary objective is to explore the Iris dataset, understand relationships between its features, train multiple classification models, and compare their performance using evaluation metrics.

The analysis uses Python-based data manipulation, exploratory data analysis (EDA), and supervised machine learning techniques to identify the best-performing model on the test dataset.

## Objectives

- Explore the Iris dataset and understand its structure.
- Analyze feature distributions and relationships between different flower species.
- Investigate which measurements are most useful for distinguishing Iris species.
- Train and evaluate Logistic Regression and Random Forest classifiers.
- Compare model performance using accuracy, precision, recall, and F1-score.
- Visualize evaluation metrics to identify the better-performing model.

## Dataset

The project uses the Iris dataset available through the `scikit-learn` library.

**Dataset details:**
- **Total observations:** 150
- **Input features:** 4
- **Target classes:** 3
- **Missing values:** None

The dataset contains the following features:

- `sepal length (cm)`: Length of the sepal in centimeters.
- `sepal width (cm)`: Width of the sepal in centimeters.
- `petal length (cm)`: Length of the petal in centimeters.
- `petal width (cm)`: Width of the petal in centimeters.
- `target`: Encoded Iris species label.

The three target classes are Iris Setosa, Iris Versicolor, and Iris Virginica. The dataset was loaded into a Pandas DataFrame for analysis and preprocessing.

## Tech Stack

- **Python** — Core programming language
- **Pandas** — Data manipulation and analysis
- **NumPy** — Numerical operations
- **Matplotlib** — Data visualization
- **Seaborn** — Statistical visualization
- **Scikit-learn** — Dataset loading, model training, and evaluation
- **Jupyter Notebook** — Interactive analysis and experimentation

## Methodology

1. **Data loading and inspection:** Loaded the Iris dataset and examined its dimensions, data types, descriptive statistics, and missing values.
2. **Exploratory Data Analysis (EDA):** Used pairplots and boxplots to investigate feature distributions and differences across species.
3. **Feature selection:** Selected all four sepal and petal measurements as input features and separated the target variable.
4. **Train-test split:** Divided the dataset into 80% training data and 20% testing data using stratified sampling to preserve class proportions.
5. **Logistic Regression:** Trained a Logistic Regression classifier as a baseline model for multiclass classification.
6. **Random Forest:** Trained a Random Forest classifier to compare an ensemble-based approach with Logistic Regression.
7. **Model evaluation:** Evaluated both models using accuracy, macro-averaged precision, recall, F1-score, confusion matrices, and classification reports.
8. **Model comparison:** Created a metric comparison heatmap to visualize the performance of both classifiers and determine which performed better on the test set.

## Key Findings

- Petal length and petal width showed strong potential for distinguishing the three Iris species.
- Iris Setosa was clearly distinguishable from the other two species based on its feature measurements.
- Some overlap between Iris Versicolor and Iris Virginica made their classification comparatively more challenging.
- Logistic Regression achieved a test accuracy of **96.67%**, correctly classifying 29 out of 30 test observations.
- Random Forest achieved a test accuracy of **90.00%**, correctly classifying 27 out of 30 test observations.
- Logistic Regression outperformed Random Forest on the current test split based on accuracy.

These results represent performance on a single train-test split and do not guarantee that Logistic Regression will outperform Random Forest on other splits or datasets.

## Visualizations

The Jupyter Notebook includes:

- Pairplot showing relationships between features, differentiated by Iris species.
- Boxplots comparing the distributions of individual features across target classes.
- Confusion matrices for Logistic Regression and Random Forest.
- Classification reports showing class-wise precision, recall, F1-score, and support.
- Model performance comparison heatmap covering accuracy, macro precision, macro recall, and macro F1-score.

## Skills Demonstrated

- Exploratory Data Analysis (EDA)
- Data inspection and preprocessing
- Feature selection and target separation
- Supervised machine learning
- Multiclass classification
- Training and testing data splitting
- Logistic Regression and Random Forest
- Model evaluation and performance comparison
- Confusion matrix interpretation
- Statistical data visualization
- Communicating data-driven findings

## Project Structure

```text
Iris-Flower-Classification/
├── iris_classification.ipynb
└── README.md
```

The notebook filename and directory structure can be adjusted to match the actual repository.

## Limitations

The evaluation is based on a relatively small dataset containing 150 observations and a single 80:20 train-test split. Consequently, the reported metrics may vary with different data splits.

The project compares two classification algorithms without extensive hyperparameter tuning or cross-validation. Further validation would help assess model stability and generalization performance.

## Conclusion

This project demonstrates how exploratory data analysis and supervised machine learning can be used to classify Iris flower species from numerical measurements. By training and comparing Logistic Regression and Random Forest models, Logistic Regression emerged as the better-performing classifier on the current test split.

The project strengthened my understanding of feature analysis, multiclass classification, model evaluation, and visualization of machine learning results.

**Project category:** Data Science | Machine Learning | Classification

**Author:** Punya Mehta