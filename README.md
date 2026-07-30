# 🩺 Thyroid Anomaly Detection using Isolation Forest & Local Outlier Factor (LOF)

## 📌 Project Overview

This project focuses on **anomaly detection** in a thyroid dataset using two popular unsupervised machine learning algorithms:

- Isolation Forest
- Local Outlier Factor (LOF)

The objective is to identify abnormal observations that may indicate unusual thyroid conditions. The detected anomalies are visualized using Principal Component Analysis (PCA), making it easier to understand the distribution of normal and anomalous data points.

---

# 🎯 Problem Statement

Detecting anomalies in medical datasets is an important task because unusual patient records may represent rare diseases, measurement errors, or high-risk cases.

This project applies unsupervised learning techniques to automatically identify these abnormal observations without relying on labeled training data.

---

# 📊 Dataset Information

Dataset: **thyroid_dataset.csv**

The dataset contains patient records with multiple numerical features related to thyroid health.

Target Column:

- **Outlier_label**
  - Normal = 1
  - Outlier = -1

For model training, only the feature columns are used. The target column is kept for comparison and evaluation.

---

# ⚙️ Project Workflow

1. Load the thyroid dataset
2. Separate features and target labels
3. Standardize numerical features using StandardScaler
4. Train an Isolation Forest model
5. Detect anomalies
6. Reduce dimensions using PCA
7. Visualize detected anomalies
8. Apply Local Outlier Factor (LOF)
9. Compare anomaly detection results

---

# 🔧 Data Preprocessing

Before training the models, the following preprocessing step was performed:

- Feature Scaling using **StandardScaler**

Standardization ensures that all numerical features contribute equally to the anomaly detection algorithms.

---

# 🤖 Machine Learning Algorithms

## 1️⃣ Isolation Forest

Isolation Forest detects anomalies by randomly partitioning the feature space.

### Advantages

- Fast on large datasets
- Works well with high-dimensional data
- Requires no labeled training data

---

## 2️⃣ Local Outlier Factor (LOF)

Local Outlier Factor detects anomalies by comparing the local density of each observation with that of its neighbors.

### Advantages

- Effective at detecting local anomalies
- Captures density-based outliers
- Suitable for complex datasets

---

# 📉 Data Visualization

Principal Component Analysis (PCA) is used to reduce the feature space to **two principal components**.

The transformed data is visualized using scatter plots where:

- Normal observations
- Detected anomalies

are displayed in different colors for easier interpretation.

---

# 📈 Results

Both anomaly detection algorithms were successfully applied to the thyroid dataset.

### Isolation Forest

- Detected anomalous observations
- Visualized anomalies using PCA
- Reported the number of normal and anomalous samples

### Local Outlier Factor

- Detected anomalous observations
- Visualized anomalies using PCA
- Reported the number of normal and anomalous samples

### Comparison

| Algorithm | Purpose |
|-----------|---------|
| Isolation Forest | Tree-based anomaly detection |
| Local Outlier Factor | Density-based anomaly detection |

Both models successfully identified abnormal observations using different detection strategies.

---

# 🔍 Key Findings

- Feature scaling significantly improves anomaly detection performance.
- PCA provides a clear visualization of high-dimensional data.
- Isolation Forest efficiently isolates anomalous observations.
- LOF identifies anomalies by comparing local neighborhood density.
- Different algorithms may detect different sets of anomalies due to their underlying approaches.

---

# 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

---

# 📂 Project Structure

```text
thyroid-anomaly-detection/
.
├── .gitignore
├── IsolationForest & LOF.ipynb
├── README.md
└── thyroid_dataset.csv
```

---

# 📚 Key Learnings

Through this project, I gained hands-on experience with:

- Unsupervised Machine Learning
- Anomaly Detection
- Isolation Forest
- Local Outlier Factor (LOF)
- Feature Scaling
- Principal Component Analysis (PCA)
- Data Visualization

---


---

# 💡 Conclusion

This project demonstrates how unsupervised machine learning techniques can detect anomalous observations in healthcare data without requiring labeled training data. By combining feature scaling, anomaly detection algorithms, and PCA visualization, the project provides an effective workflow for identifying unusual patterns in thyroid patient records.

---

# 👨‍💻 Author

**Amaan Shaikh**

Aspiring Data Science Engineer | Machine Learning Enthusiast

Feel free to explore the notebook and share your feedback!
