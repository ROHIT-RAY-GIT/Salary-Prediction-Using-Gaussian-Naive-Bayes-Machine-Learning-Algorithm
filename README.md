# 📊 Gaussian Naive Bayes Classification on Adult Income Dataset

Welcome to the **Gaussian Naive Bayes Classification** project! This application leverages machine learning to predict whether an individual earns more or less than $50,000 annually based on various demographic attributes. The dataset used is the renowned [Adult Income Dataset](https://archive.ics.uci.edu/ml/datasets/adult), which includes a variety of features related to individuals' demographics.

## 🌟 Project Overview:

In this project, we aim to develop a user-friendly web application using **Streamlit**, allowing users to input their demographic data and receive immediate predictions regarding their income category. This project is an excellent example of how machine learning can be applied to real-world data and help in understanding income distribution based on various factors.

## 📊 Dataset Overview:

The **Adult Income Dataset** consists of approximately **32,561** instances with **14** attributes. The dataset includes both numerical and categorical features. The main goal is to classify individuals based on their income levels into two categories: `<=50K` or `>50K`.

### Features:

The dataset contains the following attributes:

1. **age**: Continuous variable representing the age of the individual.
2. **workclass**: Categorical variable indicating the type of employment.
3. **fnlwgt**: Continuous variable representing the final weight, which indicates how representative the sample is of the population.
4. **education**: Categorical variable representing the highest level of education attained.
5. **education-num**: Continuous variable representing the number of years of education.
6. **marital-status**: Categorical variable indicating marital status.
7. **occupation**: Categorical variable indicating the type of occupation.
8. **relationship**: Categorical variable indicating the individual's relationship status.
9. **race**: Categorical variable indicating the individual's race.
10. **sex**: Categorical variable indicating the individual's gender.
11. **capital-gain**: Continuous variable representing capital gains.
12. **capital-loss**: Continuous variable representing capital losses.
13. **hours-per-week**: Continuous variable indicating the number of hours worked per week.
14. **native-country**: Categorical variable indicating the individual's country of origin.
15. **income**: Target variable (<=50K or >50K).

## 🔍 Data Preprocessing:

Data preprocessing is a crucial step in machine learning, ensuring that the data is clean and suitable for training the model. Here’s how the preprocessing was handled in this project:

1. **Loading the Data**:
   - The dataset was loaded using the Pandas library.

2. **Handling Missing Values**:
   - Any missing values were addressed by replacing them with the most common values (mode) for categorical features and the mean for numerical features.

3. **Encoding Categorical Variables**:
   - Categorical variables were converted into numerical format using **One-Hot Encoding**. This process transforms categorical variables into binary variables for better compatibility with the Gaussian Naive Bayes algorithm.

4. **Scaling Numerical Features**:
   - Numerical features were scaled to have a mean of 0 and a standard deviation of 1 using the **StandardScaler**. This normalization ensures that all features contribute equally to the distance calculations in the model.

5. **Splitting the Dataset**:
   - The dataset was divided into training and testing sets, with **80%** of the data used for training and **20%** for testing.

## 🚀 Features:

- **User Input**: 
  - The application allows users to enter all required features directly into the web interface, including:
    - Age
    - Work Class
    - Education
    - Marital Status
    - Occupation
    - Relationship
    - Race
    - Sex
    - Hours per week
    - Native Country

- **Model Accuracy**: 
  - The application displays the accuracy of the Gaussian Naive Bayes classifier.

- **Streamlit Frontend**: 
  - A clean and professional user interface designed for ease of use and efficiency.

## 📈 Model Performance:

The Gaussian Naive Bayes model has been trained and evaluated on the Adult Income dataset with the following performance metrics:

- **Overall Accuracy Score**: 80.36%
- **Training Set Accuracy**: 80.04%
- **Testing Set Accuracy**: 80.36%
- **Null Accuracy Score**: 76.25%

### Confusion Matrix:

The confusion matrix below illustrates the model's performance in detail:

|                | Predicted <=50K | Predicted >50K |
|----------------|------------------|----------------|
| **Actual <=50K** |       4005       |      961       |
| **Actual >50K**  |       318        |      1229      |

- **True Positives (TP)**: 1229
- **True Negatives (TN)**: 4005
- **False Positives (FP)**: 961
- **False Negatives (FN)**: 318

### Classification Metrics:

- **Precision**: 0.5607
- **Recall**: 0.7933
- **F1 Score**: 0.6610

These metrics help evaluate the model's performance in predicting income levels accurately.

## ⚙️ Technologies Used:

This project utilizes the following technologies:

- **Python**: The primary programming language for data analysis and machine learning.
- **Streamlit**: An open-source app framework for Machine Learning and Data Science projects.
- **Pandas**: For data manipulation and analysis.
- **NumPy**: For numerical operations on data arrays.
- **Scikit-learn**: A powerful library for machine learning in Python.
- **Matplotlib & Seaborn**: Libraries for data visualization.

