# Heart Disease Analysis and Prediction
This project analyzes and cleans data from the UCI Heart Disease repository, using 14 key attributes to uncover patterns. It then builds machine learning models to predict heart disease likelihood and classify its severity (1-4). The goal is to aid early diagnosis and deepen understanding of heart disease.

# About the Data
This is a multivariate type of dataset which means providing or involving a variety of separate mathematical or statistical variables, multivariate numerical data analysis. It is composed of 14 attributes which are age, sex, chest pain type, resting blood pressure, serum cholesterol, fasting blood sugar, resting electrocardiographic results, maximum heart rate achieved, exercise-induced angina, oldpeak — ST depression induced by exercise relative to rest, the slope of the peak exercise ST segment, number of major vessels and Thalassemia. This database includes 76 attributes, but all published studies relate to the use of a subset of 14 of them. The Cleveland database is the only one used by ML researchers to date. One of the major tasks on this dataset is to predict based on the given attributes of a patient that whether that particular person has heart disease or not and other is the experimental task to diagnose and find out various insights from this dataset which could help in understanding the problem more.

## Features

#### **The dataset contains 16 features which are:**

**id**: Unique id for each patient

**age**: Age of the patient in years

**origin**: place of study

**sex**: Male/Female

**cp chest pain type**: typical angina, atypical angina, non-anginal, asymptomatic

**trestbps resting blood pressure**: resting blood pressure (in mm Hg on admission to the hospital)

**chol**: serum cholesterol in mg/dl

**fbs**: if fasting blood sugar > 120 mg/dl

**restecg**: resting electrocardiographic results -- Values: [normal, stt abnormality, lv hypertrophy]

**thalach**: maximum heart rate achieved

**exang**: exercise-induced angina (True/ False)

**oldpeak**: ST depression induced by exercise relative to rest

**slope**: the slope of the peak exercise ST segment

**ca**: number of major vessels (0-3) colored by fluoroscopy

**thal**: normal; fixed defect; reversible defect

**num**: the predicted attribute

# Analysis Insights 📊

# Model Performances 📈

The performance evaluation across multiple models—Logistic Regression, Random Forest, XGBoost, Naive Bayes, and Support Vector Machine (SVM)—reveals varied outcomes when dealing with this dataset.

**Logistic Regression** demonstrated reasonable performance on the majority class (class 0), achieving a high F1-score of 0.82 and an overall accuracy of 0.59. However, it struggled with the minority classes, especially classes 2, 3, and 4, where the F1-scores were notably low. This highlights its limitations in handling imbalanced data.

**Random Forest** showed a similar pattern, with an accuracy of 0.54. It performed slightly worse than Logistic Regression across most classes, indicating that while it can handle complex relationships in the data, it also faces challenges with imbalanced class distributions.

**XGBoost** performed comparably to Logistic Regression, achieving an accuracy of 0.58. It slightly outperformed the other models in handling minority classes, reflected in its macro F1-score of 0.37, making it one of the better models in this comparison.

**Naive Bayes** struggled the most, particularly with the minority classes, resulting in a low overall accuracy of 0.49. This outcome is expected given Naive Bayes' simplicity and its tendency to underperform when faced with imbalanced or complex datasets.

**Support Vector Machine (SVM)** performed similarly to Logistic Regression, with an accuracy of 0.57. While it handled the majority class relatively well, it also faced challenges with the minority classes, resulting in lower F1-scores for these groups.

In summary, XGBoost emerged as the best-performing model in this comparison, with Logistic Regression and SVM following closely behind. However, all models struggled significantly with minority classes, indicating the need for further refinement, such as hyperparameter tuning or more sophisticated sampling techniques, to improve performance across all classes.
