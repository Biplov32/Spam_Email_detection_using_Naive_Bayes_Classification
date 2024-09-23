# Spam Email Classification Using Naive Bayes

This project is a spam email classification system using the Naive Bayes classification algorithm. It leverages Natural Language Processing (NLP) techniques to process and classify email messages into Spam or Ham (Non-spam) categories.

## Table of Contents
- [Overview](#overview)
- [Technologies Used](#technologies-used)
- [Dataset](#dataset)
- [Implementation](#implementation)
- [Evaluation](#evaluation)
- [How to Run](#how-to-run)
- [Future Improvements](#future-improvements)
- [Contact](#contact)

## Overview

This project applies machine learning techniques for classifying emails as spam or non-spam (ham). The Naive Bayes classifier, particularly the Multinomial Naive Bayes variant, is used for this task due to its efficiency in text classification.

### Key Features:
- Data processing using the Bag of Words (BOW) model.
- Multinomial Naive Bayes for email classification.
- Visualizations of the dataset using Matplotlib and Seaborn.

## Technologies Used
- Python for general programming.
- Pandas for data manipulation and analysis.
- NumPy for numerical computations.
- Matplotlib and Seaborn for visualizations.
- Scikit-learn for machine learning and data processing.

## Dataset

The dataset contains email messages labeled as "spam" or "ham" (non-spam). Each row represents an email message with two columns:

- **Category**: Label of the message (spam or ham).
- **Msg**: The actual text content of the email.

### Example of the dataset:
| Category | Msg                                      |
|----------|------------------------------------------|
| spam     | Congratulations! You have won a lottery! |
| ham      | Let’s catch up over dinner tonight.     |

## Implementation

### Data Preprocessing:
1. Convert the email text data into numerical format using the Bag of Words (BOW) model.
2. Convert spam and ham labels into binary form (spam = 1, ham = 0).
3. Calculate message length as a feature for visualizing data distribution.

### Model Training:
- The dataset is split into 80% training and 20% testing sets.
- The Multinomial Naive Bayes algorithm is used to classify the email messages.

### Prediction:
- You can input new email texts into the trained model to classify them as spam or ham.

### Accuracy Check:
- The model’s accuracy is measured using the test set.

## Evaluation

The classifier's accuracy on the test dataset is 98.65. The accuracy is not a good evaluation metrice for classification.
