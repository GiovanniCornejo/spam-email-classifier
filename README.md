# Spam Email Classifier

![Thumbnail](thumbnail.jpg)

This project is a machine learning-based classifier designed to distinguish between spam and ham (non-spam) email messages. The classifier is built using Python, leveraging techniques for text preprocessing, feature extraction, and binary classification.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Preprocessing](#preprocessing)
- [Modeling](#modeling)
- [Evaluation](#evaluation)
- [License](#license)

## Introduction

The Spam Email Classifier aims to accurately classify email messages as either spam or ham using a variety of machine learning techniques. This project provides insights into text data analysis, feature engineering, and model evaluation.

## Dataset

The dataset used for this project is the [Kaggle SMS Spam Collection Dataset](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset). It contains a collection of SMS messages labeled as either "spam" or "ham" (not spam).

## Installation

To set up the project locally, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/GiovanniCornejo/spam-email-classifier.git
   cd spam-email-classifier
   ```

2. Create a virtual environment and activate it:

   ```bash
   python -m venv venv
   source venv/bin/activate # On Windows use `venv\Scripts\activate`
   ```

3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. **Exploratory Data Analysis**
   Open and run `01_eda.ipynb` notebook for an exploratory data analysis on the dataset. This notebook includes data overview, class distribution, and text analysis.

2. **Data Preprocessing**
   Before modeling, preprocess the data to prepare it for ML algorithms. Open and execute the preprocessing steps outlined in the `02_preprocessing.ipynb` notebook. This includes tasks such as text cleaning, handling class imbalance, and feature extraction.

3. **Modeling**
   After preprocessing the data, proceed to `03_modeling.ipynb` notebook to build and train machine learning models for email classification. Explore various algorithms and techniques to find the most effective classifier.

4. **Evaluation**
   Once models are trained, evaluate their performance using `04_evaluation.ipynb` notebook. Assess the effectiveness of each model using metrics such as accuracy, precision, recall, F1 score, and area under the ROC curve (AUC).

## Exploratory Data Analysis

Key findings from the exploratory data analysis:

- The dataset is imbalanced with more ham messages than spam.
- Spam messages tend to be longer on average compared to ham messages.
- Common words and bigrams and trigrams in spam messages indicate urgency and actions (e.g., "call", "claim", "won").

## Preprocessing

Key preprocessing steps:

- **Text Cleaning**: Remove punctuation, special characters, unnecessary whitespace, and convert text to lowercase to ensure consistency.
- **Stopword Removal**: Remove common words (e.g., "the", "is", "and", etc.) that do not carry significant meaning.
- **Vectorization**: Convert text data into numerical vectors using TF-IDF (Term Frequency-Inverse Document Frequency) technique.

## Modeling

Common algorithms used for text classification are modeled:

- **Logistic Regression**: A linear model used for binary classification tasks.
- **Random Forest**: An ensemble learning method that builds multiple decision trees and combines their predictions.
- **Support Vector Machine (SVM)**: A supervised learning algorithm that separates data points using hyperplanes in high-dimensional space.
- **Naive Bayes**: A probabilistic classifier based on Bayes' theorem with strong independence assumptions between features.
- And a few others.

## Evaluation

The performance of trained models is assessed using various metrics to measure their effectiveness in distinguishing between spam and ham messages.

- **Accuracy**: The proportion of correctly classified instances out of the total instances.
- **Precision**: The proportion of true positive predictions out of all positive predictions.
- **Recall** (Sensitivity): The proportion of true positive predictions out of all actual positive instances.
- **F1 Score**: The harmonic mean of precision and recall, providing a balanced measure between the two.

Further analysis is done using:

- **Confusion Matrix**: A table that summarizes the performance of a classification model by comparing actual and predicted classes.
- **Area Under the ROC Curve (AUC)**: A measure of the classifier's ability to distinguish between classes, where higher values indicate better performance.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
