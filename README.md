# google-play-scraper-and-nlp
End-to-end NLP project: Scraping 54k+ reviews from Google Play Store (WhatsApp, TikTok, etc.), preprocessing Turkish text, and performing Sentiment Analysis using LSTM/Deep Learning.

# 📱 Google Play Store Sentiment Analysis

![Python](https://img.shields.io/badge/Python-3.x-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange)
![NLP](https://img.shields.io/badge/NLP-LSTM-green)

An end-to-end NLP project that scrapes user reviews from the Google Play Store, preprocesses Turkish text data, and classifies sentiments (Positive/Negative) using a Deep Learning **LSTM** model.

## 🚀 Features
* **Web Scraping:** Automates review collection using `google-play-scraper` (Data from WhatsApp, TikTok, Instagram, etc.).
* **Text Preprocessing:** Cleaning noise (URLs, emojis), removing stopwords, and tokenization.
* **Deep Learning:** Implements an **LSTM (Long Short-Term Memory)** network with Embedding layers.
* **Binary Classification:** Converts 1-5 star ratings into **Positive** (4-5) and **Negative** (1-3) classes.

## 📂 Files
* `main.ipynb`: The complete notebook for scraping, training, and testing.
* `sentiment_model.h5`: The trained LSTM model.
* `tokenizer.pickle`: Saved tokenizer for processing new text.
* `google_play_reviews_apps.csv`: The raw scraped dataset (~54k reviews).
