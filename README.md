# SMS Spam Classification

## Project Overview

This project classifies SMS messages as either **Ham** (normal messages) or **Spam** using machine learning.

The project follows an end-to-end classification workflow, including data preparation, train/test splitting, text feature extraction, model training, and evaluation.

## Dataset

The project uses the **SMS Spam Collection** dataset.

- Total messages: 5,572
- Ham messages: 4,825
- Spam messages: 747

## Machine Learning Workflow

- Loaded the SMS dataset using Pandas
- Checked dataset shape and columns
- Checked for missing values
- Examined class distribution
- Split the data into training and testing sets
- Converted text into numerical features using TF-IDF
- Trained a Logistic Regression classifier
- Generated predictions on the test data
- Evaluated the model using a confusion matrix, precision, recall, and F1-score

## Model Used

**Logistic Regression**

## Evaluation Results

| Metric | Result |
|---|---:|
| Precision | 1.00 |
| Recall | 0.7987 |
| F1-score | 0.8881 |

### Confusion Matrix

- True Negatives: 966
- False Positives: 0
- False Negatives: 30
- True Positives: 119

## Key Takeaway

The model achieved a precision of 1.00, meaning the messages predicted as spam were correctly classified in the test set. The recall was 0.7987, meaning the model identified most of the spam messages but missed some spam messages.

The F1-score of 0.8881 provides a useful combined measure of precision and recall, especially because the dataset contains more ham messages than spam messages.

## Tools Used

- Python
- Pandas
- Scikit-learn
- TF-IDF
- Logistic Regression
- Matplotlib
- Seaborn
- Jupyter Notebook
