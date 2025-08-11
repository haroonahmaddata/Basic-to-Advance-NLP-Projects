# Fake News Detection Using Machine Learning

## Overview  
This project classifies news articles as **fake** or **real** using machine learning models: Logistic Regression and Support Vector Machine (SVM). Text data is preprocessed with TF-IDF vectorization.

---

## Dataset  
- Labeled news articles with `0` for fake and `1` for real  
- Source: Kaggle Fake and Real News Dataset  

---

## Methodology  
1. Load and clean text data  
2. Vectorize text using TF-IDF  
3. Split data into training (80%) and testing (20%) sets  
4. Train Logistic Regression and SVM classifiers  
5. Evaluate using accuracy and F1-score  

---

## Results  

| Model                 | Accuracy | F1 Score |  
|-----------------------|----------|----------|  
| Logistic Regression    | 98.50%   | 98.41%   |  
| Support Vector Machine | 99.39%   | 99.35%   |  

---

## Visualizations  
- Word clouds for fake vs. real news  
- Histograms of article length distributions  
- Word frequency analyses  

---

## Tools & Libraries  
- Python 3.x  
- scikit-learn  
- pandas  
- matplotlib  
- wordcloud  

---

## Installation  
To install required packages, run:  
```bash
pip install scikit-learn pandas matplotlib wordcloud
