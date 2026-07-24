# Assignment_5
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
