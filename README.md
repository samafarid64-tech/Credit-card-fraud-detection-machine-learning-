# 💳 Credit Card Fraud Detection

## 📌 Project Overview

This project focuses on detecting fraudulent credit card transactions using Machine Learning. It involves analyzing transaction data, handling imbalanced classes using Under-Sampling, and building a Logistic Regression model to classify transactions as normal or fraudulent.

## 🎯 Project Objectives

- Analyze credit card transaction data.
- Explore the distribution of normal and fraudulent transactions.
- Handle imbalanced data using Under-Sampling.
- Train a Logistic Regression classification model.
- Evaluate model performance using multiple evaluation metrics.

## 🛠️ Technologies & Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook / Google Colab

## 📊 Dataset

The dataset contains credit card transactions classified into two categories:

- **Class 0:** Normal transactions.
- **Class 1:** Fraudulent transactions.

The original dataset contains a significantly larger number of normal transactions than fraudulent transactions, resulting in an imbalanced dataset.

## 🔍 Project Workflow

### 1. Data Exploration and Analysis
- Loaded and explored the dataset.
- Analyzed the distribution of normal and fraudulent transactions.
- Compared the average feature values for both transaction classes.

### 2. Handling Imbalanced Data
Applied **Under-Sampling** to reduce the number of normal transactions and create a balanced dataset.

The resulting sample contains:
- 492 normal transactions.
- 492 fraudulent transactions.
- **Total: 984 transactions.**

### 3. Model Training
Trained a **Logistic Regression** model to classify transactions into normal and fraudulent categories.

### 4. Model Evaluation
Evaluated the model using the following metrics:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

## 🤖 Model Performance

The Logistic Regression model achieved the following results on the test dataset:

| Evaluation Metric | Score |
|---|---:|
| Training Accuracy | 94.28% |
| Testing Accuracy | 92.39% |
| Precision (Fraud Class) | 93.68% |
| Recall (Fraud Class) | 90.82% |
| F1-score (Fraud Class) | 92.23% |

### Confusion Matrix

```text
[[93  6]
 [ 9 89]]
```

The model correctly classified:
- **93** normal transactions.
- **89** fraudulent transactions.

The model incorrectly classified:
- **6** normal transactions as fraudulent.
- **9** fraudulent transactions as normal.

## 📝 Conclusion

This project demonstrates a basic Machine Learning workflow for credit card fraud detection, including data exploration, handling class imbalance, model training, and evaluation.

The Logistic Regression model achieved 92.39% test accuracy on the under-sampled test dataset. Precision, Recall, and F1-score were also used to provide a more detailed evaluation of fraud detection performance.

Since Under-Sampling was used, the evaluation results may not represent performance on the original dataset, where fraudulent transactions are much less common.

## 🚀 How to Run the Project

1. Clone or download this repository.
2. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```

3. Open the Jupyter Notebook.
4. Make sure the dataset is available at the path specified in the notebook.
5. Run the notebook cells in order.

## 👩‍💻 Author

Created as a Machine Learning practice project to develop skills in data analysis, data preprocessing, classification, and model evaluation.
