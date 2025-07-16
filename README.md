# Student_Score_Prediction
## 📊 Student Exam Score Prediction
This project focuses on predicting students' final exam scores based on various academic, behavioral, and social factors. Using Linear Regression and Polynomial Regression, we analyze and model the relationship between features like hours studied, attendance, motivation, previous scores, and more.

## 📁 Dataset
Source: Student Performance Factors - Kaggle

Size: 6,607 rows × 20 columns

Target Variable: Exam_Score

Key Features:

Hours_Studied, Attendance, Previous_Scores

Categorical variables: Parental_Involvement, Internet_Access, School_Type, etc.

## 🎯 Project Goals
Clean and preprocess the dataset (handle missing values, encoding)

Explore relationships between features and the exam score

Train a Linear Regression model to predict Exam_Score

Evaluate the model using MSE, MAE, and R² Score

Try Polynomial Regression (degree 2 & 3) as a bonus and compare performance

## 🔧 Tools & Libraries
Python 🐍

Pandas for data handling

Matplotlib and Seaborn for visualization

Scikit-learn for modeling and evaluation

## 📈 Key Steps
1. 📊 Exploratory Data Analysis (EDA)
Checked for missing values

Plotted distributions & relationships (histograms, scatter plots, regression lines)

Correlation analysis to select top influencing features

2. 🧹 Data Cleaning
Filled missing categorical values with the mode

Applied One-Hot Encoding to categorical features

3. 🧠 Model Building
Split data into training/testing sets (80/20)

Trained Linear Regression and evaluated performance

Added Polynomial Regression (degree 2 & 3) for comparison

4. 📊 Evaluation Metrics
Mean Squared Error (MSE)

Mean Absolute Error (MAE)

R² Score

## 🧪 Results
Model Type	R² Score	Notes
Linear Regression	0.727	Performed best overall ✅

## 📘 Example Prediction Output
 (Actual_Exam_Score,  Predicted_Exam_Score)
                (65,                65.38)
                (71,                71.12)
               (64,               65.14)
                (66,                66.95)

🚀 Future Improvements
Feature interaction analysis

Try regularization (Ridge/Lasso)

Handle outliers for more robust results

Tune polynomial features selectively (not on full encoded data)

## 📄 License
This project is for educational purposes only.

