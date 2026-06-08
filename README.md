# 🎓 Binary Classification — Student Exam Performance

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.0-150458?logo=pandas&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-0.12-4C72B0)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1.3-F7931E?logo=scikit-learn&logoColor=white)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)
![ML](https://img.shields.io/badge/ML-Classification-blueviolet)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

A complete Binary Classification project predicting whether a student will **Pass or Fail** their exam using Logistic Regression — covering the full ML workflow from raw data to model evaluation.

\---

## 📌 Objective

To build a machine learning model that predicts student exam outcomes based on:

* Study habits (hours per day, attendance, assignment completion)
* Academic scores (math, reading, writing, science, final exam)
* Demographic and background info (parental education, family income, tutoring)
* Lifestyle factors (sleep hours, social media usage)

\---

## 📂 Dataset Overview

|Feature|Details|
|-|-|
|**File**|`student\_exam\_performance\_dataset.csv`|
|**Rows**|10,000 students|
|**Columns**|23 features|
|**Target**|`pass\_fail` (Pass / Fail)|
|**Missing Values**|None|
|**Class Balance**|\~50% Pass, \~50% Fail|

\---

## 🔍 Key Findings

* **`final\_exam\_score`** is the strongest single predictor of passing — shows the biggest gap between Pass and Fail groups
* **`attendance\_rate`** has the highest mean value (\~84.7) across the dataset
* The dataset is **perfectly balanced** (\~50/50) — no resampling or class weighting needed
* **`grade\_category`** was intentionally dropped before training to avoid **data leakage** (it's derived from scores)
* After leakage fix, model achieves **realistic and honest accuracy** instead of an inflated 99%+
* **StandardScaler** was applied — important for Logistic Regression to give all features equal weight
* **Units Sold correlation pattern** mirrors real-world behavior: engagement metrics (attendance, study hours) drive outcomes more than demographic factors

\---

## 📊 Analysis Performed

|#|Section|
|-|-|
|1|Library Imports \& Setup|
|2|Load Dataset \& Preview (head, tail, shape)|
|3|Dataset Understanding (dtypes, nulls, statistics)|
|4|Exploratory Data Analysis — 5 visualizations|
|5|Data Preprocessing — Encoding + Scaling + Leakage fix|
|6|Train-Test Split (80/20, stratified)|
|7|Logistic Regression Training + Coefficients|
|8|Predictions (class labels + probabilities)|
|9|Evaluation — Accuracy, Precision, Recall, F1|
|10|Confusion Matrix + Metrics Chart + ROC Curve|
|11|Final Conclusion \& Improvements|

\---

## 📈 Model Results

|Metric|Score|
|-|-|
|**Accuracy**|\~85%|
|**Precision**|\~85%|
|**Recall**|\~85%|
|**F1-Score**|\~85%|
|**AUC**|\~0.92|

> Run the notebook to see the exact values printed in the final summary cell.

\---

## 🛠️ Tools \& Libraries

* **Python 3.11**
* **Pandas** — data manipulation
* **NumPy** — numerical operations
* **Matplotlib** — plotting
* **Seaborn** — statistical visualizations
* **Scikit-learn** — preprocessing, model training, evaluation

\---

## 📐 Skills Demonstrated

* Exploratory Data Analysis (EDA)
* Data Cleaning \& Preprocessing
* Label Encoding \& Feature Scaling
* Identifying and fixing Data Leakage
* Binary Classification with Logistic Regression
* Model Evaluation (Accuracy, Precision, Recall, F1, AUC)
* Confusion Matrix \& ROC Curve interpretation
* Data Visualization with Matplotlib \& Seaborn

\---

## 🚀 How to Run

1. Clone this repository

```bash
   git clone https://github.com/Deepanshugahlot/Student-Exam-Performance-Classification.git
   cd Student-Exam-Performance-Classification
   ```

2. Install dependencies

```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```

3. Add the dataset — place `student\_exam\_performance\_dataset.csv` in the same folder as the notebook
4. Launch the notebook

```bash
   jupyter notebook Binary\_Classification\_Assignment.ipynb
   ```

Run all cells top to bottom: `Kernel → Restart \& Run All`

\---

## 📁 Repository Structure

```
Binary-Classification-Student-Exam/
│
├── Binary\_Classification\_Assignment.ipynb   # Main notebook
├── Binary\_Classification\_Assignment.pdf     # PDF export of notebook
├── student\_exam\_performance\_dataset.csv     # Dataset
└── README.md                                # Project overview

```

\---

## 💡 What I Learned

* EDA before modeling saves a lot of debugging later
* Data leakage is easy to miss — `grade\_category` looked like a normal feature but was secretly the answer
* The difference between accuracy, precision, recall, and F1, and when each one matters
* How StandardScaler affects Logistic Regression training
* How to read and explain a confusion matrix and ROC curve

\---

## 👤 Author

**Deepanshu Gahlot**

Aspiring Data Analyst | Building skills in Python, Statistics, EDA, Data Visualization \& Machine Learning

🔗 [LinkedIn](https://www.linkedin.com/in/deepanshugahlot001) · [GitHub](https://github.com/Deepanshugahlot)

\---

*If you found this useful, feel free to ⭐ star the repo!*

