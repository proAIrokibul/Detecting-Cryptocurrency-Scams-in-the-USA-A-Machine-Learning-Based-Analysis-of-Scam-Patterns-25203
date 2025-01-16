# Detecting-Cryptocurrency-Scams-in-the-USA-A-Machine-Learning-Based-Analysis-of-Scam-Patterns-25203
This project aims to detect and classify crypto scams using machine learning models. The dataset includes information about scams categorized into various categories and subcategories, with additional details such as URLs, descriptions, and reporter data. The project encompasses data preprocessing, visualization, and modeling, leveraging techniques to handle missing values, balance the dataset, and evaluate multiple classification models.

## Features

- **Data Preprocessing**:
  - Handling missing values by filling or dropping as necessary.
  - Encoding categorical features and deriving new insights such as the presence of addresses.
  - Balancing the dataset using **SMOTE** to address class imbalance issues.
  
- **Data Visualization**:
  - Insightful visualizations to understand data distribution and key trends, such as category and subcategory analysis, address presence, and reporter frequency.

- **Modeling**:
  - Implementation of three unique classification models:
    - **Random Forest Classifier**
    - **Logistic Regression**
    - **Multinomial Naive Bayes**
  - Evaluation of models using metrics like accuracy, precision, recall, f1-score, and confusion matrices.
  - Visualization of model performance for easy comparison.

## Results

### Random Forest Classifier:
- **Accuracy**: 99.85%
- **Confusion Matrix**:  
  ```
  [[1977    0]
   [   6 1963]]
  ```
- **Classification Report**:
  ```
                  precision    recall  f1-score   support

      Coinbase       1.00      1.00      1.00      1977
  CryptoScamDB       1.00      1.00      1.00      1969

      accuracy                           1.00      3946
     macro avg       1.00      1.00      1.00      3946
  weighted avg       1.00      1.00      1.00      3946
  ```

### Logistic Regression:
- **Accuracy**: 90.90%
- **Confusion Matrix**:  
  ```
  [[1977    0]
   [ 359 1610]]
  ```
- **Classification Report**:
  ```
                  precision    recall  f1-score   support

      Coinbase       0.85      1.00      0.92      1977
  CryptoScamDB       1.00      0.82      0.90      1969

      accuracy                           0.91      3946
     macro avg       0.92      0.91      0.91      3946
  weighted avg       0.92      0.91      0.91      3946
  ```

### Multinomial Naive Bayes:
- **Accuracy**: 85.22%
- **Confusion Matrix**:  
  ```
  [[1977    0]
   [ 583 1386]]
  ```
- **Classification Report**:
  ```
                  precision    recall  f1-score   support

      Coinbase       0.77      1.00      0.87      1977
  CryptoScamDB       1.00      0.70      0.83      1969

      accuracy                           0.85      3946
     macro avg       0.89      0.85      0.85      3946
  weighted avg       0.89      0.85      0.85      3946
  ```

## Business Impacts

The project has several key business impacts for industries and stakeholders dealing with cryptocurrency:

1. **Fraud Prevention**: 
   - Early detection of scams helps prevent financial losses for individuals and organizations, protecting billions of dollars in investments.
2. **Increased Trust in Cryptocurrency**: 
   - By identifying fraudulent schemes, this project can enhance consumer confidence in blockchain-based systems.
3. **Regulatory Support**:
   - Providing clear categorizations and detection methods can assist regulators in combating crypto-related crimes and shaping effective policies.
4. **Operational Efficiency**:
   - Automating scam detection reduces the manual effort required by investigators, allowing resources to be redirected toward more strategic activities.
5. **Brand Reputation**:
   - Organizations implementing such solutions can position themselves as secure and trustworthy platforms, gaining a competitive edge in the market.

