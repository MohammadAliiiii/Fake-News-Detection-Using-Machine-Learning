# 📰 Fake News Detection using Machine Learning

A machine learning project that detects whether a news article is fake or real based on its content.  
Built in Google Colab using scikit-learn and custom text preprocessing.

---

## 🔍 Overview

This project applies Natural Language Processing (NLP) and Machine Learning to classify news articles as **FAKE** or **REAL**.  

It includes:
- Regex-based text cleaning
- Vectorization with TF-IDF
- Models: Logistic Regression, Random Forest, Gradient Boosting
- Evaluation using accuracy, precision, recall, F1-score

---

## 📁 Dataset

The dataset used was the **Fake and Real News Dataset** available on Kaggle.  
**Columns used:** `text` (main content), `label` (REAL or FAKE)  
Other columns like `title`, `subject`, and `date` were dropped.

---

## 🛠️ Features

| Component              | Description                                                                 |
|------------------------|-----------------------------------------------------------------------------|
| ✅ Text Cleaning        | Removed URLs, HTML tags, punctuation, digits using regex                   |
| ✅ Vectorization        | TF-IDF with `TfidfVectorizer` from sklearn                                 |
| ✅ Model Training       | Trained 3 classifiers (LR, RFC, GBC) on the processed data                 |
| ✅ Manual Testing       | Custom input function to test any text against trained models              |
| ✅ Evaluation           | `classification_report` used to show performance metrics                   |

---

## 🚀 How to Run

1. Open the project in **Google Colab**  
2. Run all cells **in order** (use "Runtime > Run all")
3. Use the `manual_testing()` function to test your own headlines or articles

---

## 🔧 Tech Stack

- Python 🐍  
- pandas 🧮  
- scikit-learn ⚙️  
- re (Regex for text cleaning)  
- Google Colab ☁️

---

## 🧠 Key Learning (80/20 Principle Applied)

- **20% of the pipeline (cleaning + vectorization + model)** delivers **80% of the classification performance**
- Fitting vectorizers only once and reusing them prevents 100% of vector mismatch errors
- Restarting runtime and rerunning in sequence fixes most runtime issues efficiently

---

