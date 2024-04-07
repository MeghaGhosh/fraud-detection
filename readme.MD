# Medicare Fraud Detection

## Overview
This project aims to detect potential fraud in Medicare claims using a logistic regression classification model. The objective is to identify fraudulent claims based on various features derived from beneficiary, inpatient, and outpatient data.

## Approach
1. **Data Preprocessing:** The datasets were cleaned, and missing values were handled appropriately. Key features such as age, claim duration, and admission duration were extracted from the data.
2. **Feature Engineering:** New features were created to capture important aspects of the data, such as total reimbursement amount, chronic condition count, average claim duration, frequency of attending physicians, and beneficiary risk score. These features were designed to enhance the model's ability to detect potential fraud.
3. **Model Training:** A logistic regression model was chosen for its interpretability and simplicity. The model was trained on a balanced split of the data to ensure fair representation of both fraudulent and non-fraudulent claims.
4. **Model Evaluation:** The model's performance was evaluated on a validation set using metrics such as accuracy, precision, recall, and F1-score.

## Model Performance Analysis
The logistic regression model achieved the following performance metrics on the validation set:
- **Accuracy:** 77.60%
- **Precision:** 70.86%
- **Recall:** 61.16%
- **F1 Score:** 65.65%

The classification report further provides insights into the model's performance:

0       0.81      0.86      0.83
1       0.71      0.61      0.66

accuracy                    0.78    


The model demonstrates a decent balance between precision and recall, with a slight emphasis on precision. This indicates that the model is more conservative in flagging claims as fraudulent, potentially reducing the number of false positives.

## Dependencies
- Python 3.8+
- pandas
- numpy
- scikit-learn

To install the required dependencies, run:
```bash
pip install pandas numpy scikit-learn
