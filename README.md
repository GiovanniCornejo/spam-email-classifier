# Spam Email Classifier

This project is a machine learning-based classifier designed to distinguish between spam and ham (non-spam) email messages. The classifier is built using Python, leveraging techniques for text preprocessing, feature extraction, and binary classification.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Preprocessing](#preprocessing)
- [Modeling](#modeling)
- [Evaluation](#evaluation)
- [License](#license)

## Introduction

The Spam Email Classifier aims to accurately classify email messages as either spam or ham using a variety of machine learning techniques. This project provides insights into text data analysis, feature engineering, and model evaluation.

## Introduction

The Spam Email Classifier aims to accurately classify email messages as either spam or ham using a variety of machine learning techniques. This project provides insights into text data analysis, feature engineering, and model evaluation.

## Dataset

The dataset used for this project is the [Kaggle SMS Spam Collection Dataset](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset). It contains a collection of SMS messages labeled as either "spam" or "ham" (not spam).

## Project Structure

The project is organized as follows:

spam-email-classifier/
│
├── notebooks/
│ ├── 01_eda.ipynb # Exploratory Data Analysis
│ ├── 02_preprocessing.ipynb # Data Preprocessing
│ ├── 03_modeling.ipynb # Model Training and Evaluation
│ ├── 04_visualization.ipynb # Data Visualization
│
├── src/
│ ├── data_loader.py # Data loading functions
│ ├── feature_extraction.py # Feature extraction methods
│ ├── model.py # Model training and evaluation
│ ├── utils.py # Utility functions
│
├── data/
│ ├── raw/ # Raw data files
│ ├── processed/ # Processed data files
│
├── README.md # Project overview
├── requirements.txt # Required Python packages
├── .gitignore # Git ignore file
└── LICENSE # Project license

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

1. Exploratory Data Analysis
   Open and run `01_eda.ipynb` notebook to perform an exploratory data analysis on the dataset. This notebook includes data overview, class distribution, and text analysis.

2. Data Preprocessing:
   TODO.

## Exploratory Data Analysis

Key findings from the exploratory data analysis:

- The dataset is imbalanced with more ham messages than spam.
- Spam messages tend to be longer on average compared to ham messages.
- Common words and bigrams in spam messages indicate urgency and actions (e.g., "call", "claim", "won").

## Preprocessing

Key preprocessing steps:

- TODO.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
