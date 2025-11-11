# -K-Nearest-Neighbors-KNN-Diabetes-Prediction-Model
Predicting diabetes from diagnostic measurements using a K-Nearest Neighbors (KNN) classifier. This project evaluates the model using accuracy, precision, recall, F1-score, Jaccard index, confusion matrix, and cross-validation.

📘 Overview

Goal: Predict whether a patient has diabetes based on medical diagnostic measurements.

Dataset: Pima Indians Diabetes dataset from the National Institute of Diabetes and Digestive and Kidney Diseases (India).

Population: All samples are women aged 21 years or older.

Methodology: Data preprocessing → Stratified split → Scaling → KNN training → Evaluation & cross-validation.


Main packages:

numpy
pandas
scikit-learn
matplotlib
seaborn


📊 Features Used

Pregnancies

Glucose

BloodPressure

SkinThickness

Insulin

BMI

DiabetesPedigreeFunction

Age

Target: Outcome (0 = Non-diabetic, 1 = Diabetic)


Evaluation results
| **Metric**        | **Score** |
| ----------------- | --------- |
| **Precision**     | 0.708     |
| **Recall**        | 0.630     |
| **F1-score**      | 0.667     |
| **Accuracy**      | 0.779     |
| **Jaccard Index** | 0.500     |


Confusion Matrix
|              | Predicted 0 | Predicted 1 |
| ------------ | :---------: | :---------: |
| **Actual 0** |      43     |      7      |
| **Actual 1** |      10     |      17     |

Cross_Validation Results
| Class | Precision | Recall | F1-score | Support |
| :---- | :-------: | :----: | :------: | :-----: |
| **0** |    0.79   |  0.82  |   0.80   |   500   |
| **1** |    0.64   |  0.60  |   0.62   |   268   |


🧠 Insights

The model achieved ~78% accuracy and 0.67 F1-score, indicating decent balance between precision and recall.

Slightly lower recall (0.63) means some diabetic cases may be missed.

Further tuning (e.g., adjusting k, using SMOTE, or feature selection) could improve performance.

Distance weighting helped handle the class imbalance better than uniform weighting.


📚 Data Source

Dataset: Pima Indians Diabetes Database

(Originally from the National Institute of Diabetes and Digestive and Kidney Diseases, India)
