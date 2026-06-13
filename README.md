# 💳 Credit Card Fraud Detection using Machine Learning

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Scikit--Learn-orange)
![Status](https://img.shields.io/badge/Status-Completed-success)
![Platform](https://img.shields.io/badge/Platform-Google%20Colab-yellow)

## 📌 Project Overview

Credit card fraud has become one of the major concerns in the digital payment ecosystem. Fraudulent transactions result in significant financial losses for banks and customers every year.

This project aims to build a **Machine Learning-based Credit Card Fraud Detection System** that can accurately classify transactions as:

- ✅ Legitimate Transaction (0)
- 🚨 Fraudulent Transaction (1)

The project demonstrates the complete Machine Learning workflow, including:

- Data Collection
- Data Exploration
- Handling Imbalanced Data
- Under-Sampling Technique
- Feature Selection
- Model Training
- Model Evaluation

---

## 🎯 Objective

The primary objective of this project is to develop an intelligent system capable of identifying fraudulent credit card transactions and reducing financial risks using Machine Learning techniques.

---

## 📊 Dataset Information

The dataset contains anonymized credit card transaction records.

### Features

The dataset contains:

- Time
- V1 to V28 (PCA-transformed features)
- Amount
- Class (Target Variable)

### Target Variable

| Value | Meaning |
|-------|----------|
| 0 | Legitimate Transaction |
| 1 | Fraudulent Transaction |

---

## 📈 Dataset Statistics

### Original Dataset Distribution

| Transaction Type | Count |
|-----------------|--------|
| Legitimate Transactions | 11,906 |
| Fraudulent Transactions | 52 |

The dataset is **highly imbalanced**, making fraud detection a challenging classification problem.

---

## ⚙️ Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Scikit-Learn

---

## 🔄 Project Workflow

### 1️⃣ Data Collection

The credit card transaction dataset is loaded into a Pandas DataFrame for analysis.

---

### 2️⃣ Data Exploration

Performed:

- Dataset Inspection
- Missing Value Analysis
- Fraud Distribution Analysis
- Statistical Analysis

---

### 3️⃣ Handling Imbalanced Data

Since fraudulent transactions were extremely rare compared to legitimate transactions, **Under-Sampling** was used.

### After Sampling

| Transaction Type | Count |
|-----------------|--------|
| Legitimate Transactions | 492 |
| Fraudulent Transactions | 52 |

The new balanced dataset improves the model's ability to learn fraud patterns effectively.

---

### 4️⃣ Feature Selection

Input Features:

- Time
- V1 to V28
- Amount

Target Feature:

- Class

---

### 5️⃣ Train-Test Split

Dataset Split:

- Training Data: 80%
- Testing Data: 20%

```python
random_state = 2
```

---

### 6️⃣ Model Training

The project uses **Logistic Regression** for binary classification.

```python
from sklearn.linear_model import LogisticRegression
```

---

## 🤖 Machine Learning Model

### Logistic Regression

Logistic Regression is a supervised Machine Learning algorithm widely used for binary classification problems such as fraud detection.

---

## 📊 Model Performance

### Training Accuracy

```text
98.85%
```

### Testing Accuracy

```text
100.00%
```

| Metric | Score |
|--------|--------|
| Training Accuracy | 98.85% |
| Testing Accuracy | 100.00% |

---

## 📁 Project Structure

```text
codsoft-Credit-Card-Fraud-Detection/
│
├── Credit_Card_Fraud_Detection.ipynb
├── creditcard.csv
├── README.md
└── requirements.txt
```

---

## 🚀 Installation and Usage

### Clone Repository

```bash
git clone https://github.com/nigamkumar3435-spec/codsoft-Credit-Card-Fraud-Detection.git
```

### Navigate to Project Folder

```bash
cd codsoft-Credit-Card-Fraud-Detection
```

### Install Dependencies

```bash
pip install pandas numpy scikit-learn
```

### Open in Google Colab

1. Open Google Colab
2. Upload the notebook file
3. Upload `creditcard.csv`
4. Run all cells sequentially

---

## 🔍 Key Insights

✔ Credit card fraud datasets are extremely imbalanced.

✔ Under-Sampling can help improve fraud detection performance.

✔ Logistic Regression performs effectively for binary classification tasks.

✔ Fraudulent transactions exhibit significantly different feature patterns compared to legitimate transactions.

✔ Machine Learning can assist financial institutions in detecting suspicious activities automatically.

---

## 🎓 Learning Outcomes

Through this project, I gained practical experience in:

- Data Preprocessing
- Exploratory Data Analysis (EDA)
- Handling Imbalanced Datasets
- Under-Sampling Techniques
- Logistic Regression
- Model Evaluation
- Fraud Detection Systems
- Machine Learning Workflow

---

## 🔮 Future Improvements

- Feature Scaling
- SMOTE Oversampling
- Random Forest Classifier
- XGBoost Classifier
- Hyperparameter Tuning
- Real-Time Fraud Detection System
- Flask Deployment
- Streamlit Web Application

---

## 👨‍💻 Author

**Nigam Kumar**

🔗 GitHub: https://github.com/nigamkumar3435-spec

---

## 🙏 Acknowledgements

This project was developed as part of the **CodSoft Machine Learning Internship Program** and demonstrates the application of Machine Learning techniques in detecting fraudulent financial transactions.

---

## ⭐ If you found this project useful, please consider giving it a Star!
