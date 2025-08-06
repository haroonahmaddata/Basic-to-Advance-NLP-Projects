# Basic to Advanced NLP & ML Projects

Welcome to the **Basic to Advanced NLP & ML Projects** repository! This collection of projects is designed to showcase a step-by-step journey through Natural Language Processing (NLP) and Machine Learning (ML), from foundational concepts to practical applications.

> ⭐ If you find this helpful, consider giving it a star!

---

## 🚀 Project Highlights

### 1. **Sentiment Analysis (NLP Level 1)**

* **Goal:** Classify text data into positive/negative sentiments.
* **Tech Stack:** Python, Pandas, Scikit-learn, Matplotlib, Seaborn
* **Techniques Used:**

  * Text Preprocessing (Lowercasing, Removing stopwords, Punctuation removal)
  * Feature Extraction using TF-IDF
  * Logistic Regression Model
  * Evaluation: Accuracy, Precision, Recall, F1-Score
  * Confusion Matrix & Visualizations

> 📈 Achieved **93% Accuracy** on test data

---

### 2. **News Category Classification (NLP Level 1)**

This project demonstrates a multiclass text-classification pipeline using the AG News dataset (Kaggle). It automatically categorizes news articles into four classes: World, Sports, Business, and Sci/Tech.

**Overview**:

* **Dataset:** AG News CSV with columns `Class Index` (1=World, 2=Sports, 3=Business, 4=Sci/Tech), `Title`, and `Description`.
* **Preprocessing:** Combined and cleaned `Title` & `Description` (tokenization, stopword removal, lemmatization).
* **Feature Engineering:** TF-IDF vectorization (top 5,000 features).
* **Model:** Logistic Regression (Accuracy: **91.0%**, Precision: 0.92, Recall: 0.90, F1-Score: 0.91).
* **Visualization:** Bar plots and word clouds of the top 10 words per category.

---

## 🛠️ Requirements

* Python 3.7+
* pandas
* numpy
* nltk
* scikit-learn
* matplotlib
* wordcloud

Install dependencies via:

```bash
pip install pandas numpy nltk scikit-learn matplotlib wordcloud
```

## 🔗 License

This repository is released under the MIT License. Feel free to use, modify, and contribute!
