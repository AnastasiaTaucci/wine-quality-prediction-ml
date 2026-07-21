# Red Wine Quality Classification Using Machine Learning

## Overview

This project uses machine learning to classify red wine quality scores based on chemical properties such as acidity, sugar content, pH, sulphates, density, and alcohol level.

The project was completed as a final project for AI240: Machine Learning at Bellevue College in Spring 2025.

The goal was to practice the machine learning workflow, including dataset exploration, feature selection, model training, model evaluation, and comparison of classification algorithms.

## Problem Statement

Wine quality is often evaluated by human experts, which can be subjective and time-consuming. This project explores how machine learning can use measurable chemical features to predict wine quality scores in a more automated and data-driven way.

The target variable is the wine quality score, ranging from 3 to 9.

Because the target values are discrete categories, this is a multi-class classification problem, not a regression problem.

## Dataset

This project uses a balanced version of the UCI Red Wine Quality dataset from Kaggle.

Dataset source: Kaggle — Balanced Wine Quality Dataset  
https://www.kaggle.com/datasets/taweilo/wine-quality-dataset-balanced-classification

The balanced dataset was selected because the original wine quality dataset is highly imbalanced, with most wines rated 5 or 6 and fewer examples of very low or very high ratings. Using a balanced dataset helped reduce class bias and made it easier to compare classification models.

## Features

The model uses 11 chemical attributes:

- Fixed acidity
- Volatile acidity
- Citric acid
- Residual sugar
- Chlorides
- Free sulfur dioxide
- Total sulfur dioxide
- Density
- pH
- Sulphates
- Alcohol

## Machine Learning Models

Two classification models were compared:

### Logistic Regression

Logistic Regression was used as a simple baseline classification model. It is fast to train and useful for testing whether simple patterns can predict wine quality.

### Decision Tree Classifier

Decision Tree was used because it can capture more complex, non-linear relationships between chemical features and wine quality scores.

## Model Evaluation

The models were evaluated using:

- Accuracy score
- Confusion matrix
- Classification report
- Precision
- Recall
- F1-score

## Results

| Model | Accuracy |
|---|---:|
| Logistic Regression | 29% |
| Decision Tree Classifier | 59% |

The Decision Tree model performed better than Logistic Regression. This suggests that wine quality depends on multiple interacting chemical features, and a model that can capture non-linear patterns is more effective for this task.

## Conclusion

The Decision Tree Classifier was the stronger model for this project, achieving 59% accuracy across seven wine quality classes.

Although the result is not perfect, it is reasonable for a multi-class classification problem with wine quality scores ranging from 3 to 9. The project demonstrates how machine learning can support quality prediction by identifying patterns in chemical data.

## Technologies Used

- Python
- pandas
- matplotlib
- seaborn
- scikit-learn
- Jupyter Notebook

## Files

- `wine_quality_final.ipynb` — Jupyter Notebook with data exploration, model training, and evaluation
- `wine_data.csv` — dataset used for the project
- `Wine_Quality_Prediction_Presentation.pdf` — final project presentation
- `original_formats/Wine_Quality_Prediction_Presentation.pptx` — editable PowerPoint version of the presentation

## Skills Demonstrated

- Machine learning fundamentals
- Multi-class classification
- Data exploration
- Feature-based prediction
- Model training and testing
- Model comparison
- Accuracy evaluation
- Confusion matrix interpretation
- Classification report interpretation
- Python programming
- pandas data manipulation
- Data visualization with matplotlib and seaborn
- scikit-learn
- Technical presentation

## Setup

To run the notebook locally, install the required Python libraries:

```bash
pip install pandas matplotlib seaborn scikit-learn
