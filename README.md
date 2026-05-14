# OIBSIP-Spam-Detection
# 📧 Email Spam Detection using Machine Learning

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge\&logo=python)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange?style=for-the-badge\&logo=scikitlearn)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-black?style=for-the-badge\&logo=pandas)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

Detect whether an email or SMS message is **Spam** or **Ham (Not Spam)** using Machine Learning and Natural Language Processing techniques.

---

# 📚 Table of Contents

1. [Project Overview](#-project-overview)
2. [Dataset](#-dataset)
3. [Technologies Used](#-technologies-used)
4. [Machine Learning Pipeline](#-machine-learning-pipeline)
5. [Model Used](#-model-used)
6. [Project Workflow](#-project-workflow)
7. [Results](#-results)
8. [How to Run](#-how-to-run)
9. [Future Improvements](#-future-improvements)
10. [Conclusion](#-conclusion)

---

# 📌 Project Overview

Spam emails and messages are unwanted communications that may contain advertisements, phishing links, scams, or malicious content.

The objective of this project is to build a Machine Learning model capable of automatically classifying messages as:

* ✅ Ham (Not Spam)
* 🚨 Spam

The model is trained using labeled SMS/email data and Natural Language Processing techniques.

---

# 📂 Dataset

Dataset used:

* `spam.csv`

Dataset contains:

* `ham` → Normal message
* `spam` → Spam message

---

# 🛠 Technologies Used

* Python
* Pandas
* Scikit-learn
* NLP (Natural Language Processing)

---

# ⚙ Machine Learning Pipeline

The project follows these steps:

```text
Load Dataset
   ↓
Clean Data
   ↓
Convert Text into Numerical Features
   ↓
Train ML Model
   ↓
Test Model
   ↓
Predict Spam/Ham
```

---

# 🤖 Model Used

## Multinomial Naive Bayes

Why this model?

* Fast and efficient
* Performs very well on text classification
* Commonly used for spam filtering systems

---

# 🔄 Project Workflow

## 1. Data Loading

The dataset is loaded using Pandas.

## 2. Data Cleaning

Only required columns are selected and labels are converted:

```text
ham  → 0
spam → 1
```

## 3. Text Vectorization

TF-IDF Vectorizer converts text messages into numerical features understandable by Machine Learning models.

## 4. Model Training

The Naive Bayes model is trained on the dataset.

## 5. Prediction

The trained model predicts whether a message is spam or not.

---

# 📈 Results

The model successfully classifies spam and non-spam messages with high accuracy.

Example:

```text
Input:
"Congratulations! You won a free iPhone."

Prediction:
SPAM
```

---

# ▶ How to Run

## Install dependencies

```bash
pip install pandas scikit-learn
```

## Run the project

```bash
python spam_detector.py
```

---

# 🚀 Future Improvements

* Deploy as a web application
* Add deep learning models
* Improve preprocessing techniques
* Support multiple languages

---

# 📌 Conclusion

This project demonstrates how Machine Learning and NLP can be used to automatically detect spam messages. It highlights the practical use of text classification techniques in real-world applications like email filtering and cybersecurity.
