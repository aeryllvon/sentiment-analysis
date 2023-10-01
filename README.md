### Sentiment Analysis for Enhanced Business Intelligence

**Model and Evaluation**


- **Logistic Regression - 77.69% Accuracy**
- **Random Forest Classifier - 82.57% Accuracy**
- **Naive Bayes - 71.26% Accuracy**
- **Recurrent Neural Network - 77% Accuracy**
- **Epoch-wise Accuracy**

- **Epoch 1:**
    - Training Accuracy: 78.18%
    - Validation Accuracy: 78.30%
- **Epoch 2:**
    - Training Accuracy: 78.79%
    - Validation Accuracy: 78.04%
- **Epoch 3:**
    - Training Accuracy: 79.52%
    - Validation Accuracy: 77.88%
- **Epoch 4:**
    - Training Accuracy: 79.82%
    - Validation Accuracy: 77.47%
- **Epoch 5:**
    - Training Accuracy: 79.92%
    - Validation Accuracy: 77.54%

**Vader - 76.69% Accuracy**

## Objective:

To see if sentiment analysis of Amazon product reviews might offer useful information for making strategic business decisions.

To determine whether suggestions for business strategies can be gleaned from the sentiment analysis of customer evaluations.

To investigate how insights from sentiment analysis might improve marketing, sales forecasting, customer service and product development.


## Dataset

The dataset consisted of product reviews, each labeled with a score indicating the sentiment of the review. a score above 3 was considered positive, below 3 was considered negative and a score of 3 was neutral.

| Column                 | Non-Null Count | Dtype |
|------------------------|----------------|-------|
| Id                     | 568454         | int64 |
| ProductId              | 568454         | object|
| UserId                 | 568454         | object|
| ProfileName            | 568428         | object|
| HelpfulnessNumerator   | 568454         | int64 |
| HelpfulnessDenominator | 568454         | int64 |
| Score                  | 568454         | int64 |
| Time                   | 568454         | int64 |
| Summary                | 568427         | object|
| Text                   | 568454         | object|


## Methodology

**Data Pre-processing**

The **raw** text data was **preprocessed** by removing **HTML** tags, converting to lowercase, tokenizing, removing stopwords and performing stemming and lemmatization.

**Exploratory Data Analysis**

Visualised the initial **distribution** of **sentiments** and generated **WordClouds** for each sentiment class after **preprocessing** the text.

**Data Balancing**

Employed **SMOTE** to handle **class imbalance** in the dataset.

**Model Training and Evaluation** 

Multiple models were trained and evaluated on the processed dataset using **accuracy** and **classification report**.


