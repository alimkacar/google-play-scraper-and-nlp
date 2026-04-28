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
```
### 1️⃣ Repoyu Klonlayın
```bash
git clone https://github.com/alimkacar/google-play-scraper-and-nlp.git
cd google-play-scraper-and-nlp
```
### 2️⃣ Bağımlılıkları Yükleyin
Gerekli kütüphaneleri yüklemek için requirements.txt dosyasını kullanın:
```bash
pip install -r requirements.txt

(Not: requirements.txt içinde pandas, numpy, scikit-learn, xgboost, lightgbm, matplotlib, shap, google-play-scraper gibi kütüphaneler bulunmaktadır.)
```
### 3️⃣ Projeyi Çalıştırın
Jupyter Notebook arayüzünü başlatın ve sentiment_proje_improved.ipynb dosyasını açın:
```bash
jupyter notebook sentiment_proje_improved.ipynb

```
✨ Özellikler (Features)
Bu proje, basit bir sınıflandırma modelinin ötesine geçerek modern NLP pratiklerini uygulamaktadır:
🕷️ Otomatik Veri Toplama: google-play-scraper kullanarak popüler uygulamalardan (WhatsApp, TikTok, Instagram vb.) 54.000+ yorumu otomatik çeker.
🧹 Türkçe NLP Ön İşleme: Özel stopword listesi, noktalama temizliği ve metin normalizasyonu ile ham metni modele uygun hale getirir.
⚙️ Gelişmiş Özellik Mühendisliği:
TF-IDF vektörizasyonu (Unigram & Bigram)
Duygu analizi için ek sayısal özellikler: kelime_sayisi, buyuk_harf_orani, unlem_sayisi (Örn: Büyük harf kullanımı öfke belirtisi olabilir).
🤖 Çoklu Model Eğitimi: Logistic Regression, Random Forest, XGBoost ve LightGBM modelleri eğitilmiştir.
🔍 Hiperparametre Optimizasyonu: GridSearchCV ve RandomizedSearchCV ile modellerin en iyi parametreleri otomatik bulunmuştur.
📊 Görselleştirme & Analiz:
ROC Eğrisi ile model karşılaştırması.
Confusion Matrix analizi.
Feature Importance (Önemli kelimelerin tespiti).
🧠 SHAP Açıklanabilirlik: XGBoost modelinin kararlarını SHAP (SHapley Additive exPlanations) kütüphanesi ile yorumlanabilir hale getirilmiştir.
📊 Veri Seti (Dataset)
Kaynak: Google Play Store
Uygulamalar: WhatsApp, TikTok, Instagram, Facebook, X (Twitter), Telegram
Toplam Yorum: ~12.000
Sınıf Dengesi:
✅ Pozitif (4-5 Yıldız): %52
❌ Negatif (1-3 Yıldız): %47

📈 Sonuçlar ve Tartışma (Results & Discussion)
Projede 4 farklı makine öğrenmesi algoritması karşılaştırılmış ve XGBoost (Tuned) modeli en yüksek F1 skoruna ulaşmıştır.
                      Model	Accuracy	  F1 Score	  Precision     Recall
Logistic Regression	    0.8183	         0.8432	      0.8475	    0.8390
Random Forest        	  0.8106	         0.8323	      0.8591	    0.8071
XGBoost (En İyi)	      0.8031	         0.8349	      0.8158	    0.8550
LightGBM	              0.8115	         0.8403	      0.8294	    0.8515   


🔍 SHAP Analizi Bulguları
SHAP analizi, modelin "Pozitif" tahminlerinde en çok hangi kelimelere odaklandığını göstermiştir:
  - süper, harika, mükemmel, güzel kelimeleri pozitif sınıfa güçlü katkı sağlar.
  - açılmıyor, kötü, berbat kelimeleri negatif sınıfa yönlendirir.

Önemli Keşif: çok iyi veya hiç beğenmedim gibi ifadelerin yakalanmasında Bigram (1,2) özelliğinin TF-IDF'de kullanılması başarıyı artırmıştır.


