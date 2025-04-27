# Credit Card Fraud Detection

## Overview

This project aims to build a machine learning model capable of accurately distinguishing fraudulent credit card transactions from legitimate ones. The model is trained and evaluated using a dataset containing various transaction details.

### Objectives

* Develop a machine learning model for credit card fraud detection.
* Preprocess transaction data, including details like amount, user ID, merchant information, and timestamps.
* Identify key transactional attributes indicative of fraudulent behavior.
* Achieve a fraud detection system that minimizes false positives while maximizing fraud detection accuracy.
* Provide explanations for transaction misclassifications.

### Dataset

The dataset used in this project contains credit card transaction information with the following attributes:

* `trans_date_trans_time`: Transaction date and time
* `cc_num`: Credit card number
* `merchant`: Merchant name
* `category`: Transaction category
* `amt`: Transaction amount
* `first`: First name
* `last`: Last name
* `gender`: Gender
* `street`: Street address
* `city`: City
* `state`: State
* `zip`: Zip code
* `lat`: Latitude
* `long`: Longitude
* `city_pop`: City population
* `job`: Job
* `dob`: Date of birth
* `trans_num`: Transaction number
* `unix_time`: Unix timestamp
* `merch_lat`: Merchant latitude
* `merch_long`: Merchant longitude
* `is_fraud`: Fraudulent transaction indicator (0: legitimate, 1: fraudulent)

### Dependencies

* `numpy`
* `pandas`
* `scikit-learn`

### Data Preprocessing

The following preprocessing steps are applied to clean and prepare the data for model training:

* Removal of irrelevant columns such as `Unnamed: 0`, `cc_num`, `first`, `last`, `street`, `city`, `state`, `zip`, `dob`, `trans_num`, and `trans_date_trans_time`.
* Handling missing values (if any).

### Model Training and Evaluation

* The dataset is split into training and testing sets.
* A Decision Tree Classifier model is trained on the training data.
* The model's performance is evaluated on the testing data using accuracy metrics.

### Results

The trained Decision Tree Classifier model achieved an accuracy of [insert accuracy here] on the test set.

### Misclassification Explanation

Further analysis is required to provide detailed explanations of misclassified transactions. This will involve examining the specific attributes of these transactions and comparing them with typical patterns of fraudulent and legitimate activities.

### Future Improvements

* Explore other machine learning models for potential performance improvements.
* Implement techniques to handle imbalanced datasets (if applicable) to improve fraud detection accuracy.
* Incorporate feature engineering to create new relevant attributes.
* Conduct more detailed analysis of misclassified transactions to identify patterns and improve model accuracy.
