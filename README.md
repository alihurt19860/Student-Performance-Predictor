## 🎓 Student Performance Predictor

**By:** M.Ali
**Course:** Machine Learning Lab Task
**Environment:** Python (Jupyter Notebook)


### 🧭 Project Overview

This project aims to predict **student academic performance** using **machine learning models**.
It integrates multiple ML techniques — **Linear Regression**, **Logistic Regression**, and **Decision Tree Classifier** — to analyze study-related factors and determine whether a student will **pass or fail**, as well as predict their **final marks**.

The project demonstrates how **data preprocessing, visualization, modeling, and evaluation** can work together to form a complete end-to-end ML pipeline.


### 🎯 Objectives

* Apply key ML concepts learned in Labs 1–6 to a real-world dataset.
* Build and compare **regression** and **classification** models.
* Implement full data preprocessing, feature scaling, and model evaluation.
* Visualize insights that explain what affects student performance

### 🧩 Dataset

**Name:** Student Performance Data Set (UCI Machine Learning Repository)
**Link:** [UCI Student Performance Dataset](https://archive.ics.uci.edu/ml/datasets/Student+Performance)

**Description:**
This dataset contains student data from secondary school, including information such as:

* Study time
* Attendance and absences
* Previous exam scores (G1, G2)
* Final grade (G3)
* Family background, parental education, and more

**Target Variables:**

* **G3** → Final marks (for regression)
* **Pass/Fail** → Derived column (1 = Pass if G3 ≥ 10, else 0)


### ⚙️ Technologies Used

* **Programming Language:** Python
* **IDE:** Jupyter Notebook
* **Libraries:**

  * `pandas`, `numpy` → Data handling
  * `matplotlib`, `seaborn` → Data visualization
  * `scikit-learn` → ML modeling, preprocessing, and evaluation


### 🔧 Project Workflow

#### 1. Data Preprocessing

* Handled missing values using mean imputation.
* Encoded categorical variables using `LabelEncoder`.
* Scaled numerical features using `StandardScaler`.
* Created a binary target column **pass_fail** based on final marks.

#### 2. Data Visualization

* Explored feature relationships with correlation heatmaps.
* Visualized study time and its effect on grades.
* Identified key factors influencing performance.

#### 3. Model Development

| Model                        | Type           | Purpose                          |
| ---------------------------- | -------------- | -------------------------------- |
| **Linear Regression**        | Regression     | Predicts final marks (G3)        |
| **Logistic Regression**      | Classification | Predicts Pass/Fail status        |
| **Decision Tree Classifier** | Classification | Alternative model for comparison |

#### 4. Model Evaluation

* **Linear Regression:** Evaluated using Mean Squared Error (MSE) and R² Score.
* **Classification Models:** Evaluated using Accuracy, Precision, Recall, and Confusion Matrix.
* Compared Logistic Regression vs Decision Tree results.

### 📊 Results Summary

| Model               | Accuracy | Precision | Recall |
| ------------------- | -------- | --------- | ------ |
| Logistic Regression | ~0.85    | ~0.83     | ~0.80  |
| Decision Tree       | ~0.88    | ~0.85     | ~0.87  |

*(Values may vary depending on random state and preprocessing choices.)*

**Key Insight:**
Decision Tree slightly outperformed Logistic Regression in this dataset, while Linear Regression provided a reasonable estimation of final marks. Study time and previous grades (G1, G2) were the most influential features

### 📈 Visual Outputs

* **Correlation Heatmap** — Displays relationships between numeric features.
* **Study Time vs Final Marks Plot** — Shows positive correlation between study hours and performance.
* **Confusion Matrix** — Visualizes model classification performance.

### 🏁 Conclusion

* Successfully built an end-to-end ML system combining **regression** and **classification** models.
* Showed how multiple ML techniques can complement each other in analyzing academic outcomes.
* Demonstrated the importance of data preprocessing and model evaluation.

This project integrates **theoretical concepts** from earlier labs into a **practical, real-world ML solution**.

### 📎 Deliverables

* Jupyter Notebook: `StudentPerformancePredictor.ipynb`
* Dataset: `student-mat.csv`


### 🧠 Future Improvements

* Add Random Forest or Gradient Boosting for enhanced accuracy.
* Include hyperparameter tuning with GridSearchCV.
* Build an interactive dashboard for prediction visualization.
