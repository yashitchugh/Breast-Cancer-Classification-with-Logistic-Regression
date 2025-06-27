
# 🧠 Breast Cancer Classification with Logistic Regression

This project demonstrates a complete pipeline for binary classification using **Logistic Regression** on the **Breast Cancer Wisconsin (Diagnostic) Dataset**. We perform preprocessing, model training, evaluation (confusion matrix, precision, recall, ROC-AUC), and threshold tuning.

---

## 📁 Project Structure

```

breast-cancer-logistic-regression/
├── README.md
├── breast\_cancer\_classification.ipynb  # Jupyter notebook or script
└── requirements.txt                   # Dependencies

````

---

## 📊 Dataset

- **Name**: Breast Cancer Wisconsin (Diagnostic) Dataset
- **Source**: Built into `scikit-learn`
- **Features**: 30 numerical features from digitized images of fine needle aspirates
- **Target**:  
  - `0`: malignant  
  - `1`: benign  

---

## 🚀 Pipeline Overview

### 1. Load & Split Data
- Use `train_test_split` with 80/20 split
- Stratified to preserve class balance

### 2. Feature Standardization
- Use `StandardScaler` to normalize the data

### 3. Model Training
- Fit a `LogisticRegression` model (`max_iter=1000`)

### 4. Evaluation Metrics
- **Accuracy**
- **Confusion Matrix**
- **Precision & Recall**
- **ROC-AUC Score**
- **ROC Curve Visualization**

### 5. Threshold Tuning
- Use predicted probabilities from sigmoid function
- Adjust decision threshold to improve precision or recall
- Plot precision vs. recall vs. threshold

---

## 📈 Sample Results (default threshold = 0.5)

| Metric     | Score   |
|------------|---------|
| Accuracy   | ~0.96   |
| Precision  | ~0.97   |
| Recall     | ~0.94   |
| ROC-AUC    | ~0.99   |

---

## 📦 Requirements

Install dependencies:

```bash
pip install -r requirements.txt
````

### `requirements.txt` example:

```
scikit-learn
matplotlib
numpy
```

---

## 📚 Learnings

* How logistic regression uses the **sigmoid** function to model probabilities
* Importance of **feature scaling**
* Trade-off between **precision and recall**
* How to **tune classification thresholds** for real-world use cases

---

## ✅ Next Steps

* Try other classifiers (Random Forest, SVM)
* Perform cross-validation
* Deploy model with a web app (e.g., Streamlit)

---

