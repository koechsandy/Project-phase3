# Diabetes Risk Predictor: Applying Health Indicators for Early Detection


# Business Uderstanding
The dataset contains health indicators from the Behavioral Risk Factor Surveillance System (BRFSS) 2015, with a binary outcome indicating whether a patient has diabetes. The goal is to develop a predictive model that can accurately classify whether a patient has diabetes based on various health indicators. This model can be used by healthcare providers to identify at-risk individuals and implement early intervention strategies, ultimately improving patient outcomes and reducing healthcare costs.

# Dataset Description
The "diabetes_binary_health_indicators_BRFSS2015.csv" file is a clean dataset of 253,680 survey responses to the CDC's BRFSS2015. The target variable is Diabetes_binary, which has 2 classes. 0 is for no diabetes, and 1 is for prediabetes or diabetes. This dataset has 21 feature variables and is not balanced.

### Objectives
Objective:

The primary objective is to analyze the dataset containing health indicators from the Behavioral Risk Factor Surveillance System (BRFSS) 2015 to uncover insights into the factors that can predict the likelihood of diabetes, enabling early intervention. By leveraging this data, the project aims to:

. To identify individuals at high risk of developing diabetes before symptoms appear.

.  To tailor treatment and management plans based on individual risk profiles..

. To enhance public health strategies and policies by identifying trends and risk factors.

. To lower the long-term costs associated with diabetes management and complications.

## Modelling

### Data Preprocessing
Loading the Data: The dataset was loaded from a CSV file into a pandas DataFrame.

Data Inspection: We inspected the dataset to understand its structure, including the number of entries, columns, and data types. The dataset contains 253,680 entries and 22 columns, all of which are numerical.

### Model Building
Logistic Regression:
Logistic Regression is used as a baseline model due to its simplicity and interpretability. This model is particularly useful for binary classification problems like predicting whether an employee will leave (Yes) or stay (No). It estimated the probability of the attrition based on the input features.
The coefficients from the Logistic Regression were interpreted to understand the impact of each feature on the probability of attrition.



## Model Evaluation
Precision, Recall, F1-Score:
Given the potential imbalance in the dataset , metrics like Precision, Recall, and F1-Score were crucial for assessing model performance.
Precision measured the accuracy of positive predictions, Recall measured the ability to identify all positive instances, and F1-Score is the harmonic mean of Precision and Recall.

## Conclusion
Logistic Model Performance Summary:

Accuracy: 84.93%
Precision: 54.49%
Recall: 14.40%
F1 Score: 81.03%
### 1. Overall Accuracy:

The Logistic model has a high accuracy of 84.93%, indicating that it performs well in correctly predicting both attrition and non-attrition cases overall.
### 2. Precision:

With a precision of 54.49%, the model is moderately effective at identifying instances of attrition when it predicts them. This means that about half of the instances flagged as attrition are true positives. However, there is a considerable proportion of false positives, where the model incorrectly labels non-attrition cases as attrition.
### 3. Recall:

The recall of 14.40% is relatively low, indicating that the model identifies only a small fraction of actual attrition cases. This suggests that many employees who are likely to leave are not being flagged by the model, which could be problematic if the goal is to proactively address potential attrition.
### 4. F1 Score:

The F1 Score of 81.03%  highlights that the model captures effectively  the positive cases (attrition) while maintaining a reasonable level of precision.
Implications
Attrition Identification: The model's ability to identify attrition is limited, as evidenced by the low recall. This means the organization may be missing many potential cases of employee attrition, which could affect planning and retention strategies.

## Recommendations:

### Improve Recall: 
Focus on improving the model's recall to ensure that more actual attrition cases are identified. This can be achieved by addressing class imbalance, adjusting the classification threshold, and exploring advanced models.
### Feature Engineering: 
Enhance the feature set to better capture the factors contributing to attrition. This could involve adding new features or refining existing ones based on domain knowledge.
### Model Enhancement:
Consider experimenting with different algorithms and hyperparameter tuning to improve the model's performance metrics.
## Strategic Recommendations:

### Proactive Measures:
Implement strategies to address the factors contributing to attrition more effectively, using insights gained from refining the model.
### Advanced Techniques:
Explore ensemble methods or other machine learning techniques to achieve better performance in predicting employee attrition.


### From our plot, we can conclude that the F1 score and accuracy of the Logistic Regression model is better compared to the Decision Tree model, making it the better model to use in the Dibetes Risk Prediction

# Conclusion
### In this project, we analyzed the Diabetes Health Indicators Dataset using various machine learning techniques(Logistic Regression and Decision Trees). We created predictive models for diabetes risk and analyzed the feature importance in the dataset. The results of this analysis can be used to identify individuals at risk for diabetes and to develop targeted interventions to prevent or manage the disease.
