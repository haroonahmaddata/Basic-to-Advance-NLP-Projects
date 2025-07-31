# 🧠 Sentiment Analysis using Machine Learning (TF-IDF + Logistic Regression)

This project focuses on building a binary **Sentiment Analysis** model using **Natural Language Processing (NLP)** techniques. The model classifies text into **positive (1)** or **negative (0)** sentiments using **TF-IDF** for feature extraction and **Logistic Regression** for classification.

---

## 📂 Project Structure

```
Sentiment_Analysis_NLP_Lv_1/
│
├── Sentiment_Analysis_NLP_Lv_1.ipynb      # Main notebook with code and results
├── README.md                              # Project documentation
```

---

## 🚀 Key Features

* **Text Preprocessing**:

  * Lowercasing, punctuation removal, stopword removal
* **TF-IDF Vectorization**:

  * Transforms text into numeric vectors
* **Model**:

  * Logistic Regression (scikit-learn)
* **Evaluation**:

  * Accuracy, Precision, Recall, F1-Score
  * Confusion Matrix and Visualizations using seaborn

---

## 📊 Results Snapshot

**Model Performance**:

```
Accuracy: 93.43%

Confusion Matrix:
[[11336  5043]
 [ 1863 86921]]

F1-Score:
- Negative: 0.77
- Positive: 0.96
```

---

## 📦 Libraries Used

* `pandas`
* `numpy`
* `matplotlib`
* `seaborn`
* `scikit-learn`
* `nltk`

---

## 💠 How to Run

1. Clone this repository:

   ```bash
   git clone [https://github.com/haroonahmaddata/NLP-Projects/]
   cd sentiment-analysis-nlp
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Run the notebook:

   * Open `Sentiment_Analysis_NLP_Lv_1.ipynb` in Jupyter or Google Colab

---

## 📌 Use Cases

* Customer feedback classification
* Review analysis (products, movies, etc.)
* Social media sentiment monitoring

---

## ✍️ Author

**Haroon Ahmad**
Bachelor of Software Engineering
Connect: [LinkedIn](https://linkedin.com)

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
