# 🇹🇷 Turkish Sentiment Analysis (Google Play Reviews)

**An End-to-End NLP Project: Turkish Text Classification using Machine Learning & SHAP Explainability**

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1.3-orange)
![XGBoost](https://img.shields.io/badge/XGBoost-Lightning-green)
![SHAP](https://img.shields.io/badge/SHAP-Explainable_AI-red)
![License](https://img.shields.io/badge/License-MIT-yellow)

## 📋 Project Overview

This project aims to classify user reviews from the Google Play Store into **Positive** and **Negative** sentiments using Natural Language Processing (NLP) and Machine Learning techniques. The dataset consists of **54,000+ Turkish user reviews** scraped from popular applications.

The project covers the complete data science lifecycle:
1.  **Data Collection:** Automated scraping of reviews.
2.  **Preprocessing:** Custom Turkish text cleaning and normalization.
3.  **Feature Engineering:** TF-IDF vectorization with N-grams.
4.  **Modeling:** Comparison of Logistic Regression, Random Forest, XGBoost, and LightGBM.
5.  **Evaluation:** Precision, Recall, F1-Score, and Confusion Matrix analysis.
6.  **Explainability:** SHAP (SHapley Additive exPlanations) analysis for model interpretability.

## ✨ Features

*   🕷️ **Smart Scraping:** Automates review collection using `google-play-scraper`.
*   🧹 **Turkish NLP Pipeline:** Specialized cleaning for Turkish characters, stopwords, and noise removal.
*   ⚙️ **Feature Engineering:** TF-IDF vectorization with unigram and bigram support (`ngram_range=(1, 2)`).
*   🤖 **Model Comparison:** Rigorous comparison of 4 different algorithms (LR, RF, XGB, LGB).
*   🎛️ **Hyperparameter Tuning:** GridSearchCV and RandomizedSearchCV for optimization.
*   🔍 **Explainability:** SHAP analysis to understand which words drive the sentiment predictions.

## 📂 Project Structure

```bash
.
├── 📓 sentiment_analysis.ipynb       # Main analysis notebook
├── 📄 requirements.txt               # Dependencies
├── 📄 google_play_reviews.csv        # Raw scraped dataset
├── 📂 models/                        # Saved trained models
├── 📂 visuals/                       # Generated plots (SHAP, ROC, Confusion Matrix)
└── 📄 README.md


## 🛠️ Installation & Setup

Projeyi yerel ortamınızda çalıştırmak için aşağıdaki adımları izleyin:

### 1️⃣ Repoyu Klonlayın
```bash
git clone https://github.com/alimkacar/google-play-scraper-and-nlp.git
cd google-play-scraper-and-nlp

### 2️⃣ Bağımlılıkları Yükleyin
Gerekli kütüphaneleri yüklemek için requirements.txt dosyasını kullanın:
```bash
pip install -r requirements.txt

(Not: requirements.txt içinde pandas, numpy, scikit-learn, xgboost, lightgbm, matplotlib, shap, google-play-scraper gibi kütüphaneler bulunmaktadır.)

### 3️⃣ Projeyi Çalıştırın
Jupyter Notebook arayüzünü başlatın ve sentiment_proje_improved.ipynb dosyasını açın:
```bash
jupyter notebook sentiment_proje_improved.ipynb

