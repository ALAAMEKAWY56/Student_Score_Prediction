
# 📊 Student Exam Score Prediction using Regression

This project focuses on predicting students' final exam scores using various performance-related features such as study hours, attendance, previous scores, and socio-academic factors.

The dataset used is the **Student Performance Factors** dataset from Kaggle, with 6,600+ records and 20 features.

---

## 🔧 Tools & Libraries Used

- Python (Jupyter Notebook)
- Pandas, NumPy
- Scikit-learn (Linear & Polynomial Regression)
- Matplotlib & Seaborn for Visualization

---

## 📌 Project Steps

1. **Data Cleaning**
   - Handled missing values (filled with mode).
   - Applied **outlier capping** using the IQR method (with a relaxed multiplier of `2.0`) to preserve extreme but realistic scores.

2. **Exploratory Data Analysis**
   - Correlation heatmap for feature selection.
   - KDE, histogram, and line plots for variable trends.
   - Categorical feature distributions using pie charts and bar plots.

3. **Feature Engineering**
   - One-hot encoding for categorical variables.
   - Standardization for numerical features like `Hours_Studied`, `Attendance`, and `Previous_Scores`.

4. **Modeling**
   - **Linear Regression** (Baseline)
   - **Polynomial Regression** (Degree 2 & 3) for comparison

5. **Evaluation Metrics**
   - Mean Squared Error (MSE)
   - Mean Absolute Error (MAE)
   - R² Score

6. **Cross-Validation (5-Fold)**

---

## 📈 Cross-Validation Results (5 Folds)

| Metric | Fold 1 | Fold 2 | Fold 3 | Fold 4 | Fold 5 | Mean |
|--------|--------|--------|--------|--------|--------|------|
| **MSE** | 0.490 | 0.441 | 0.488 | 0.464 | 0.471 | **0.471** |
| **MAE** | 0.565 | 0.535 | 0.569 | 0.555 | 0.556 | **0.556** |
| **R²**  | 0.952 | 0.960 | 0.957 | 0.958 | 0.959 | **0.957** |

✅ These results show **high consistency** across all folds, indicating that the model is **generalizing well** and **not overfitting**.

---

## 🔍 Actual vs Predicted (Sample Output)

| Actual_Exam_Score | Predicted_Exam_Score |
|-------------------|----------------------|
| 68                | 68.78                |
| 64                | 63.47                |
| 71                | 70.29                |
| 64                | 65.23                |
| 66                | 66.29                |
| 66                | 65.20                |
| 69                | 69.43                |
| 68                | 68.67                |
| 62                | 62.01                |
| 71                | 71.45                |

✅ As seen above, predictions are **very close to actual scores** with minimal error.

---

## 📌 Bonus
- Polynomial Regression (Degree 2) improved R² slightly.
- Degree 3 introduced overfitting with a **lower R²**, so Degree 2 was chosen.

---

## 📤 How to Use

1. Clone this repo
2. Run the Jupyter Notebook
3. Modify or add student records in the input cell to get predictions

---

## 🤖 Future Improvements

- Add decision trees or ensemble models
- Deploy via Flask web app
- Predict categorical performance level (e.g., Pass / Fail)

---

## 📁 Dataset
> Source: [Kaggle - Student Performance Factors](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams)

---

## 📬 Contact
For any inquiries or feedback, feel free to reach out via GitHub Issues.
