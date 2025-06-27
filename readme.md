# Breast Cancer Classification using Logistic Regression

## Objectives

- To predict whether a tumor is Malignant (cancerous) or Benign (non-cancerous) using Logistic Regression.
- To handle multicollinearity by removing highly correlated features.
- To optimize model performance using Hyperparameter Tuning (RandomizedSearchCV).
- To evaluate the model using standard metrics like Confusion Matrix, Precision, Recall, and ROC-AUC.
- To experiment with decision threshold tuning and explain the Sigmoid function used in Logistic Regression.

## What We Did

- Loaded and cleaned the Breast Cancer Wisconsin (Diagnostic) dataset.
- Removed unnecessary columns (`Unnamed: 32` and `id`).
- Converted categorical diagnosis labels to binary (Malignant = 1, Benign = 0).
- Identified and removed highly correlated features with a threshold greater than 0.9.
- Scaled features using StandardScaler to normalize the dataset.
- Split the data into training and testing sets (75% Train, 25% Test).
- Applied Logistic Regression with Hyperparameter Tuning using RandomizedSearchCV.
- Evaluated the model using Confusion Matrix, Classification Report, ROC-AUC Score, and ROC Curve.
- Tuned classification threshold to observe its impact on model performance.
- Plotted the Sigmoid function to demonstrate probability output behavior.

## How We Did It

1. **Data Preprocessing**
   - Loaded the dataset using Pandas.
   - Dropped irrelevant columns.
   - Converted the target column (`diagnosis`) to binary values.
   - Checked for missing values.

2. **Correlation Analysis & Feature Selection**
   - Plotted a correlation heatmap.
   - Removed features with correlation greater than 0.9 to reduce multicollinearity.

3. **Feature Scaling**
   - Applied StandardScaler for feature normalization.

4. **Model Building**
   - Used `train_test_split` to divide the dataset.
   - Performed hyperparameter tuning with RandomizedSearchCV for Logistic Regression.

5. **Model Evaluation**
   - Generated Confusion Matrix to analyze prediction breakdown.
   - Produced Classification Report showing Precision, Recall, and F1-Score.
   - Calculated ROC-AUC Score and plotted the ROC Curve for model evaluation.

6. **Threshold Tuning**
   - Changed the classification threshold from the default 0.5 to other values (e.g., 0.6).
   - Observed the effect on confusion matrix and classification report.

7. **Sigmoid Function Plot**
   - Plotted the Sigmoid curve to visualize how Logistic Regression converts linear output to probability between 0 and 1.

## Why We Did This

- To develop a reliable and interpretable model for breast cancer diagnosis.
- To reduce multicollinearity for more stable and meaningful results.
- To optimize model performance through systematic hyperparameter tuning.
- To understand the practical impact of threshold tuning on real-world classification problems.
- To visualize core concepts of Logistic Regression for better theoretical understanding.

## Conclusion

A Logistic Regression model was successfully built, optimized, and evaluated for predicting breast cancer. The model is interpretable, efficient, and incorporates best practices such as feature reduction, scaling, and hyperparameter tuning. Threshold tuning and Sigmoid visualization provided deeper insights into classification behavior.

