# Breast Cancer Diagnosis Prediction

## Overview
This project classifies breast cancer tumors into **Malignant (M)** and **Benign (B)** categories using **K-Nearest Neighbors (KNN)** and **K-Means clustering**. The dataset used is the [Wisconsin Breast Cancer Dataset](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data).

## Approach

1. **Data Loading:** Read Excel file into a pandas DataFrame.  
2. **Preprocessing:**  
   - Encode `diagnosis`: M → 1, B → 0  
   - Drop unnecessary columns: `id` and `Unnamed: 32`  
   - Normalize features using Min-Max scaling  
3. **Train-Test Split:** Split dataset into 80% training and 20% testing.  
4. **K-Means Clustering:**  
   - Unsupervised clustering into 2 clusters  
   - Compare cluster assignments with actual diagnosis  
5. **KNN Classification:**  
   - Train KNN (k=5) on training set  
   - Predict on testing set  
6. **Evaluation Metrics:**  
   - Accuracy, Precision, Recall, F1-score  
   - Confusion Matrix and Classification Report  
7. **Visualization:**  
   - PCA plot to visualize clusters  
   - Confusion matrix heatmap  

## Results

- **KNN Model Performance:**  
  - Accuracy: ~96.5%  
  - Precision: 1.0  
  - Recall: 0.905  
  - F1-score: 0.95  

- **K-Means Clustering:**  
  - Rough separation of malignant and benign tumors, useful for visualization.

## Files

- `Breast_Cancer_KNN_KMeans.ipynb` – Jupyter/Colab Notebook with full code.  

## Conclusion

The KNN model achieved excellent performance in classifying tumors, making it reliable for early breast cancer diagnosis. K-Means clustering provides an unsupervised view of the natural groupings.
