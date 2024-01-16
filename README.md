# SpamGuard: Intelligent SMS Filtering System

SpamGuard is an intelligent SMS filtering system designed to detect and filter spam messages using machine learning techniques. It utilizes the SMS Spam Collection dataset from Kaggle and implements a Bag of Words approach along with the Multinomial Naive Bayes algorithm for efficient spam detection.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Implementation](#implementation)
  - [Data Cleaning and Exploration](#data-cleaning-and-exploration)
  - [Feature Engineering](#feature-engineering)
  - [Text Preprocessing](#text-preprocessing)
  - [Bag of Words in scikit-learn](#bag-of-words-in-scikit-learn)
  - [Naive Bayes Model Training](#naive-bayes-model-training)
  - [Model Evaluation](#model-evaluation)
- [Results](#results)
- [Usage](#usage)
- [Dependencies](#dependencies)
- [License](#license)

## Introduction

SpamGuard is a spam detection system for SMS messages, developed using machine learning algorithms. The system achieves high accuracy and precision in identifying spam, making it a reliable tool for filtering unwanted messages.

## Dataset

The system uses the SMS Spam Collection dataset from Kaggle, containing a collection of spam and non-spam (ham) SMS messages. The dataset is preprocessed and explored to create a robust model.

## Implementation

### Data Cleaning and Exploration

- Loaded the dataset and removed unnecessary columns.
- Renamed columns for clarity.
- Explored basic statistics and visualizations of the data.

### Feature Engineering

- Added a new feature "length" to represent the length of each SMS.
- Visualized the distribution of SMS lengths for both spam and ham messages.

### Text Preprocessing

- Tokenized and preprocessed the text data using a Bag of Words approach.
- Created a frequency list of words for each document.

### Bag of Words in scikit-learn

- Used scikit-learn's `CountVectorizer` to convert the text data into a matrix of token counts.
- Split the dataset into training and testing sets.

### Naive Bayes Model Training

- Applied the Multinomial Naive Bayes algorithm to the training data.

### Model Evaluation

- Evaluated the model's performance using metrics such as accuracy, precision, recall, and F1 score.

## Results

The SpamGuard system achieved impressive results on the test set:
- Accuracy: 98.48%
- Precision: 94.20%
- Recall: 93.53%
- F1 Score: 93.86%

## Usage

To use SpamGuard, follow these steps:
1. Install the required dependencies.
2. Run the provided Python script.

## Dependencies

- numpy
- pandas
- nltk
- matplotlib
- seaborn
- scikit-learn

Install dependencies using:

```bash
pip install numpy pandas nltk matplotlib seaborn scikit-learn
```

## License

This project is licensed under the [MIT License](LICENSE).
