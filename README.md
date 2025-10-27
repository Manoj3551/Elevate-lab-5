# 🌳 Task 5 - Decision Trees and Random Forests

## 🎯 Objective
The goal of this task is to understand and implement **Decision Tree** and **Random Forest** algorithms for classification.  
We analyze model performance, interpret feature importance, and explore overfitting control using depth and cross-validation.

---

## 🧰 Tools & Libraries
- **Python 3**
- **Pandas, NumPy** – Data manipulation
- **Scikit-learn** – ML model building
- **Matplotlib, Seaborn** – Data visualization
- **Graphviz** (optional) – Tree visualization

---

## 📂 Dataset
Dataset used: [Heart Disease Dataset](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)  
Download and rename the file as `heart.csv` in the project folder.

---

## ⚙️ Steps Performed

### 1️⃣ Load Dataset
Read data and check for missing values using `pandas`.

### 2️⃣ Split Data
Divide into features (`X`) and target (`y`), then split using `train_test_split()`.

### 3️⃣ Decision Tree Model
- Trained using `DecisionTreeClassifier`
- Controlled overfitting using `max_depth`
- Evaluated with `accuracy_score` and `classification_report`
- Visualized using `plot_tree()`

### 4️⃣ Random Forest Model
- Trained using `RandomForestClassifier`
- Compared accuracy with Decision Tree
- Displayed **feature importances** graphically
- Evaluated via **cross-validation**

### 5️⃣ Evaluation Metrics
- Accuracy
- Confusion Matrix
- Classification Report
- Cross-validation mean score

---

## 📊 Results Summary

| Model | Accuracy | CV Accuracy | Notes |
|--------|-----------|--------------|-------|
| Decision Tree | ~80% | ~78% | Slight overfitting when depth not controlled |
| Random Forest | ~86% | ~84% | More stable and robust |

**Random Forest** performs better due to ensemble averaging, which reduces variance.

---

## 🧠 Interview Questions & Answers

**1. How does a Decision Tree work?**  
It splits data based on feature thresholds to create branches that minimize impurity, classifying samples at leaf nodes.

**2. What is Entropy and Information Gain?**  
- **Entropy** measures data impurity.  
- **Information Gain** is the reduction in entropy after a feature split.

**3. How is Random Forest better than a single tree?**  
It combines multiple trees (bagging), reducing variance and overfitting.

**4. What is Overfitting and how do you prevent it?**  
Overfitting happens when the model learns noise. Prevent using `max_depth`, `min_samples_split`, or Random Forest.

**5. What is Bagging?**  
Bootstrap Aggregation — training multiple models on random samples and averaging results.

**6. How do you visualize a Decision Tree?**  
Using `plot_tree()` from sklearn or external tools like Graphviz.

**7. How do you interpret Feature Importance?**  
It shows how much each feature contributes to model prediction accuracy.

**8. Pros and Cons of Random Forest**
| Pros | Cons |
|------|------|
| Reduces overfitting | Computationally expensive |
| Handles missing values | Less interpretable |
| Works well on large data | Slower predictions |

---

## 📁 Folder Structure
task5_decision_randomforest/
│
├── heart.csv
├── task5_decision_randomforest.py
├── README.md
└── screenshots/ (optional visualization outputs)

yaml
Copy code

---

## 🚀 How to Run
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
python task5_decision_randomforest.py
✅ Output
Decision Tree and Random Forest accuracy comparison

Tree visualization

Feature importance bar chart

Confusion matrix heatmap

Author: Manoj Kumar
Internship Program: AI & ML Internship
Task 5: Decision Trees and Random Forests '''

