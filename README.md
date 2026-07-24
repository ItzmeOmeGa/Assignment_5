# Assignment_5
# 👨‍💼 Employee Attrition Prediction using Decision Tree and Random Forest

## 📌 Objective

The objective of this project is to predict whether an employee is likely to leave the organization using machine learning classification algorithms. Two models, **Decision Tree** and **Random Forest**, are implemented and compared to determine which provides better predictive performance.

---

## 📂 Dataset Link

**Dataset:** IBM HR Analytics Employee Attrition & Performance Dataset

https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset

---

## 🛠️ Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- KaggleHub

---

## ⚙️ Methodology

1. Loaded the dataset using KaggleHub.
2. Performed data understanding and exploratory analysis.
3. Checked for missing values.
4. Removed unnecessary columns.
5. Encoded categorical variables using LabelEncoder.
6. Split the dataset into training (80%) and testing (20%).
7. Built a Decision Tree classifier.
8. Built a Random Forest classifier with 100 estimators.
9. Evaluated both models using Accuracy, Precision, Recall, and F1-Score.
10. Generated Confusion Matrices.
11. Visualized Feature Importance for the Random Forest model.
12. Compared both models.

---

---

## 📈 Model Comparison

- Random Forest generally achieves higher accuracy.
- Decision Tree is easier to interpret.
- Random Forest reduces overfitting through ensemble learning.
- Feature Importance identifies the most influential employee attributes.

---

## ✅ Conclusion

Random Forest outperformed Decision Tree by producing more accurate and stable predictions. Decision Trees are simple and interpretable but tend to overfit. Random Forest combines multiple trees, resulting in better generalization and improved predictive performance. Although Random Forest requires greater computational resources, it is a better choice for employee attrition prediction on this dataset.

---

## 📁 Project Structure

```
Assignment-5
│── Assignment-5.ipynb
│── README.md
```

---

## ▶️ How to Run

1. Open the notebook in Google Colab.
2. Install KaggleHub:

```bash
pip install kagglehub[pandas-datasets]
```

3. Run all notebook cells.
4. View the evaluation metrics, confusion matrices, and feature importance plot.

---

## 👨‍💻 Author

**Name:** Arpan Samanta

**Course:** B.Tech CSE (AI & ML)

**University:** VIT Bhopal University
## 📊 Results

Both **Decision Tree** and **Random Forest** classifiers were trained and evaluated on the **IBM HR Analytics Employee Attrition & Performance Dataset**.

---

### 🌳 Decision Tree Performance

| Metric | Score |
|---------|------:|
| **Accuracy** | **79.93%** |
| **Precision** | **23.68%** |
| **Recall** | **23.08%** |
| **F1-Score** | **23.38%** |

#### Classification Report

| Class | Precision | Recall | F1-Score | Support |
|------|----------:|-------:|---------:|--------:|
| **No Attrition (0)** | 0.88 | 0.89 | 0.88 | 255 |
| **Attrition (1)** | 0.24 | 0.23 | 0.23 | 39 |

**Overall Accuracy:** **79.93%**

---

### 🌲 Random Forest Performance

| Metric | Score |
|---------|------:|
| **Accuracy** | **88.10%** |
| **Precision** | **83.33%** |
| **Recall** | **12.82%** |
| **F1-Score** | **22.22%** |

#### Classification Report

| Class | Precision | Recall | F1-Score | Support |
|------|----------:|-------:|---------:|--------:|
| **No Attrition (0)** | 0.88 | 1.00 | 0.94 | 255 |
| **Attrition (1)** | 0.83 | 0.13 | 0.22 | 39 |

**Overall Accuracy:** **88.10%**

Both models were evaluated using **Accuracy, Precision, Recall, F1-Score, and Confusion Matrix**.

---

## 📈 Model Comparison

| Metric | Decision Tree | Random Forest |
|---------|--------------:|--------------:|
| **Accuracy** | **79.93%** | **88.10%** |
| **Precision** | 23.68% | **83.33%** |
| **Recall** | **23.08%** | 12.82% |
| **F1-Score** | **23.38%** | 22.22% |

### 🔍 Key Observations

- The **Random Forest** model achieved a higher overall **accuracy (88.10%)** than the **Decision Tree (79.93%)**, making it the better-performing model in terms of overall prediction accuracy.
- Random Forest achieved a much higher **precision (83.33%)**, meaning that when it predicted employee attrition, those predictions were more likely to be correct.
- The **Decision Tree** achieved a higher **recall (23.08%)** than the Random Forest (**12.82%**), indicating it detected more employees who actually left the company.
- Both models had relatively low F1-scores for the attrition class, suggesting that predicting employee attrition is challenging due to the imbalance between employees who stayed and those who left.
- Overall, **Random Forest** provided more reliable and stable performance because it combines multiple decision trees, reducing overfitting and improving generalization.
