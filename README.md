📌 Breast Cancer Diagnosis — KNN & K-Means

This project classifies breast cancer tumors into Malignant (M) or Benign (B) using K-Nearest Neighbors (KNN) and performs clustering using K-Means.

Dataset used: Breast Cancer Wisconsin Diagnostic Dataset
(Provided in the assignment)

🚀 Objectives

The goal of this project is to:

Convert the diagnosis column:
M → 1, B → 0

Drop unnecessary columns:

id

Unnamed: 32

Apply Min-Max Normalization

Split the dataset into:

Training: 80%

Testing: 20%

Apply K-Means clustering (k=2)
to observe patterns between benign and malignant tumors

Train a KNN classifier with k = 5

Evaluate the model using:

Accuracy

Precision

Recall

F1-score

🧪 Methods Used
1. Data Preprocessing

Loaded the dataset

Encoded diagnosis labels (M = 1, B = 0)

Dropped irrelevant columns

Scaled all features using MinMaxScaler

2. Clustering (K-Means)

Applied k=2

Observed how the data groups into two clusters

3. Classification (KNN)

Used KNeighborsClassifier(k=5)

Trained on normalized training data

Evaluated predictions using standard classification metrics

📊 Model Results
Metric	Score
Accuracy	~0.96
Precision	~1.00
Recall	~0.90
F1-score	~0.95

(Your exact results may vary slightly depending on train-test split randomness.)
