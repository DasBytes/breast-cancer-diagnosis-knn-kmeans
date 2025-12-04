# Breast Cancer Diagnosis Prediction using KNN and K-Means

## 📌 Objective
To classify breast cancer diagnoses into two categories:
- **Malignant (M)**
- **Benign (B)**

using the **K-Nearest Neighbors (KNN)** and **K-Means Clustering** algorithms.

---

## 📂 Dataset
The dataset was provided as an Excel file.  
Target column:
- `diagnosis`
  - `M` → 1
  - `B` → 0

Unnecessary columns removed:
- `id`
- `Unnamed: 32`

---

## ⚙️ Methodology

### 1. File Upload in Google Colab  
The dataset is uploaded directly into Google Colab.

### 2. Handling Missing Values (Deletion Method)  
Rows with missing values are removed using:
```python
df = df.dropna()
