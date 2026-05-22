# 💬 Sentiment Analysis

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![NLP](https://img.shields.io/badge/NLP-Sentiment-yellow.svg)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-orange.svg)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen.svg)

## 📌 Project Overview

This project develops a machine learning model to analyze the **sentiment of text data** — classifying it as **Positive**, **Neutral**, or **Negative**. It uses Twitter airline reviews as the dataset and compares three NLP-based classification algorithms.

---

## 🎯 Objectives

- Develop a model to analyze text sentiment (positive, negative, neutral)
- Use customer/social media data (Twitter Airline Sentiment)
- Preprocess text (remove stopwords, URLs, mentions, cleaning)
- Apply basic NLP techniques (TF-IDF, Lemmatization)
- Display predicted sentiment with confidence

---

## 📂 Project Structure

```
sentiment_analysis/
│
├── Tweets.csv                    # Dataset (Twitter Airline Sentiment)
├── sentiment_analysis.ipynb      # Main Jupyter Notebook
├── sentiment_distribution.png    # Sentiment class distribution
├── tweet_length.png              # Tweet length by sentiment
├── wordcloud.png                 # WordClouds for each sentiment
├── model_comparison.png          # Accuracy comparison chart
├── confusion_matrices.png        # Confusion matrices for all models
└── README.md                     # Project documentation
```

---

## 📊 Dataset

- **Source:** [Twitter US Airline Sentiment - Kaggle](https://www.kaggle.com/datasets/crowdflower/twitter-airline-sentiment)
- **Size:** ~14,000 tweets
- **Classes:** Positive, Neutral, Negative
- **Domain:** US Airline customer reviews on Twitter

---

## 🛠️ Technologies Used

| Library | Purpose |
|--------|---------|
| `pandas` | Data loading and manipulation |
| `numpy` | Numerical operations |
| `nltk` | Stopwords, Lemmatization |
| `scikit-learn` | TF-IDF, ML models, evaluation |
| `wordcloud` | Word frequency visualization |
| `matplotlib` | Plotting and charts |
| `seaborn` | Heatmaps and visuals |

---

## ⚙️ Installation

```bash
pip install pandas numpy scikit-learn matplotlib seaborn nltk wordcloud
```

---

## 🔄 Workflow

```
Raw Tweet Data
    ↓
Text Preprocessing (lowercase, remove URLs, mentions, hashtags, stopwords)
    ↓
Lemmatization
    ↓
TF-IDF Vectorization (7000 features, bigrams)
    ↓
Train/Test Split (80% / 20%)
    ↓
Model Training (Naive Bayes + Logistic Regression + Linear SVM)
    ↓
Evaluation (Accuracy, Precision, Recall, F1-Score)
```

---

## 🧹 Text Preprocessing Steps

1. Convert to lowercase
2. Remove URLs (`http://...`)
3. Remove mentions (`@username`) and hashtags (`#tag`)
4. Remove special characters and numbers
5. Tokenization
6. Remove stopwords
7. Apply WordNet Lemmatization

---

## 🤖 Models Used

### 1. Multinomial Naive Bayes
- Probabilistic classifier for text data
- Fast and lightweight

### 2. Logistic Regression
- Strong multi-class classifier
- High interpretability

### 3. Linear SVM (Support Vector Machine)
- Best performer for text classification
- Handles high-dimensional TF-IDF features excellently

---

## 📈 Results

| Model | Accuracy |
|-------|----------|
| Naive Bayes | ~75% |
| Logistic Regression | ~79% |
| Linear SVM | ~80% |

---

## 🧪 Sample Predictions

```python
predict_sentiment("I absolutely love this airline! Best flight ever!")
# → 😊 Positive

predict_sentiment("The flight was delayed and customer service was terrible.")
# → 😡 Negative

predict_sentiment("Flight was okay, nothing special about it.")
# → 😐 Neutral
```

---

## 📉 Visualizations

- **Sentiment Distribution** — Class balance bar chart
- **Tweet Length by Sentiment** — Histogram comparison
- **WordCloud** — Most frequent words per sentiment class
- **Model Accuracy Comparison** — Bar chart
- **Confusion Matrices** — Heatmaps for all 3 models

---

oses only.
