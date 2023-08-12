# Predictive-Modeling-for-Students-Drop-out-Prediction-Using-Machine-Learning-and-Data-Analysis.

## Introduction

This project aims to contribute to the reduction of dropouts in higher education by leveraging machine learning techniques. It focuses on identifying students who are at risk of dropping out early in their academic path, enabling the implementation of timely support strategies. The dataset used for this project is sourced from a higher education institution in Portugal and is available at the following link:

[Dataset Link](https://archive-beta.ics.uci.edu/ml/datasets/predict+students+dropout+and+academic+success#Papers)

The dataset contains valuable information about students at the time of enrollment, encompassing demographics, socio-economic factors, and academic performance during the first year (2 semesters). Each instance also contains the student's status (Dropout/Enrolled/Graduate). The target variable has been customized for binary classification (Drop-out or Not Drop-out).

After performing essential data cleaning and preprocessing steps, a range of classification models will be trained and evaluated using appropriate machine learning algorithms.


## Business Problem Scoping

The primary objective of this project is to develop a binary classifier capable of identifying students who are likely to drop out based on their academic performance and demographic characteristics. The scenarios that we anticipate during model training include:

- True Positives (TP): When the model predicts a student as "Drop-out," and the actual status is also "Drop-out."
- True Negatives (TN): When the model predicts a student as "Not Drop-out," and the actual status is "Not Drop-out" as well.
- False Positives (FP): When the model predicts a student as "Drop-out" when, in reality, the student is "Not Drop-out."
- False Negatives (FN): When the model predicts a student as "Not Drop-out" when, in reality, the student is "Drop-out."

The purpose of this model is to address the drop-out problem within the university. By accurately identifying potential dropouts, the university can implement interventions such as career counseling, mentorship programs, alternate class scheduling, and online classes to encourage students to complete their courses. While there is a cost associated with false positives (allocating resources to students who might not need them), this cost is significantly outweighed by the revenue loss resulting from actual dropouts.

Our approach is to minimize false negatives (FNs) to the greatest extent possible, ideally aiming for zero FNs. This translates to maximizing the "Recall Score" in our project. In cases of data imbalance, we will focus on maximizing the "F2 score," which provides a higher weightage to recall while considering both precision and recall. Ultimately, the model with the highest Recall/F2 score will be considered the best-performing model.

## Project Workflow

1. **Install and Import Necessary Packages**: Begin by installing and importing the required Python packages for data analysis, preprocessing, and model training.

2. **Preliminary Business Problem Scoping**: Define the problem scope and objectives, and outline the scenarios anticipated during model training.

3. **Load, Clean, and Prepare Data**: Load the dataset, perform necessary data cleaning, and prepare the data for analysis.

4. **Clean and Transform the Data**: Explore and preprocess the data for analysis. Two cases will be considered: Case-1 using only student attributes at enrollment, and Case-2 with all attributes except macroeconomic data.

5. **Partition Data for Model Evaluation**: Split the data into training and test sets for model evaluation.

6. **Address Data Imbalances**: Implement an oversampling technique to address data imbalances in the training set.

7. **Train the Models**: Train various classification models, including Decision Trees, Random Forest, AdaBoost, Gradient Boost, K-Nearest Neighbors, XGBoost, Logistic Regression, and Artificial Neural Networks.

8. **Performance Comparison**: Compare model performances using accuracy, precision, recall, F1 score, and F2 score metrics.

9. **Conclusion**: Summarize the analysis and findings of the project, highlighting the model with the best performance and its implications for addressing student dropouts.

## Results and Conclusion

Through comprehensive data analysis and model training, this project provides insights into identifying students at risk of dropping out from higher education institutions. By leveraging machine learning techniques, we have developed an effective binary classification model capable of distinguishing potential dropouts from enrolled students. Our analysis includes two distinct cases, emphasizing the importance of student academic performance data in achieving better predictive accuracy.

The Neural Network model emerges as the top-performing model, exhibiting a recall score of 79.4%, which implies that the model can accurately identify close to 80 out of 100 potential dropout students. This predictive capability offers universities a valuable tool for implementing timely interventions and support measures to retain at-risk students. The simplicity and low cost of this approach make it an appealing solution with significant potential to positively impact both students and institutions.

By leveraging readily available student information and applying machine learning, this project offers a strategic approach to mitigate student dropouts and foster academic success.


