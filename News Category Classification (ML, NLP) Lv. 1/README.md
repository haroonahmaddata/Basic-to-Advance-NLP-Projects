# News Category Classification

This project demonstrates a multiclass text classification pipeline using the AG News dataset (Kaggle). It automatically categorizes news articles into four classes: World, Sports, Business, and Sci/Tech.

---

## 📋 Description

* **Dataset**: AG News (CSV format) with three columns:

  * `Class Index` (1=World, 2=Sports, 3=Business, 4=Sci/Tech)
  * `Title`
  * `Description`
* **Objective**: Clean and preprocess text, convert into numeric features, train a classifier to predict the news category, and visualize the most frequent words per category.

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

---

## ⚙️ Setup & Usage

1. **Download the AG News dataset** from Kaggle and place `ag_news.csv` in the project root.

2. **Run preprocessing and model training**:

   ```bash
   python run_classification.py
   ```

   This script will:

   * Load the CSV
   * Clean `Title` and `Description` (tokenization, stopword removal, lemmatization)
   * Combine cleaned text into a single `text` column
   * Zero-base labels (`0`–`3`)
   * Split into train/test (80/20, stratified)
   * Vectorize with TF‑IDF (top 5,000 features)
   * Train a Logistic Regression model
   * Evaluate and print accuracy, precision, recall, F₁-score
   * Generate bar plots and word clouds of top words per class

3. **Inspect outputs**:

   * Performance metrics printed to console
   * Plots displayed (bar charts & word clouds)

---

## 📈 Results

* **Accuracy**: 0.91
* **Precision**: 0.92
* **Recall**:    0.90
* **F₁-Score**: 0.91

The model shows strong baseline performance on a straightforward TF‑IDF + Logistic Regression pipeline.

---

## 🔍 Visualization

* **Bar Plots**: Top 10 most frequent words per category
* **Word Clouds**: Visual representation of category-specific vocabulary

These visuals help confirm that each class’s vocabulary aligns with domain-specific terms (e.g., "game"/"season" for Sports, "reuters"/"company" for Business).


## 🔗 License

This project is released under the MIT License. Feel free to use and modify!
