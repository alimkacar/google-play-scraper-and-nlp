🚀 Turkish App Review Sentiment Analysis

Google Play Scraper + Advanced NLP + ML Models

Bu proje, Google Play Store’daki uygulama yorumlarını otomatik olarak toplayıp gelişmiş NLP teknikleri ve makine öğrenmesi modelleri ile duygu analizi (sentiment analysis) yapan uçtan uca bir sistemdir.

📌 Proje Özeti

📥 Google Play’den otomatik veri toplama

🇹🇷 Türkçe metinler için özel NLP pipeline

🤖 Birden fazla ML modeli ile karşılaştırmalı analiz

📊 Model performans değerlendirme ve görselleştirme

🧠 SHAP ile model açıklanabilirliği

⚙️ Kullanılan Teknolojiler

-Python

-scikit-learn

-XGBoost

-LightGBM

-SHAP

-Google Play Scraper

-Pandas / NumPy / Matplotlib

✨ Özellikler

🔹 Veri Toplama

Google Play Scraper ile:

WhatsApp

TikTok

Instagram

Facebook

X (Twitter)

Telegram

10.000+ yorum otomatik çekilir


🔹 Türkçe NLP Ön İşleme

Stopword temizleme (özel liste)

Noktalama temizleme

Küçük/büyük harf normalizasyonu

Tokenization

🔹 Feature Engineering

TF-IDF (Unigram + Bigram)

Ek özellikler:

-kelime sayısı

-büyük harf oranı

-ünlem sayısı

🔹 Model Eğitimi

Logistic Regression

Random Forest

XGBoost

LightGBM


🔹 Hiperparametre Optimizasyonu

GridSearchCV

RandomizedSearchCV


🔹 Analiz & Görselleştirme

ROC Curve

Confusion Matrix

Feature Importance


🔹 Model Açıklanabilirliği

SHAP (Shapley Values) ile model kararlarını analiz etme


📊 Model Performans Karşılaştırması
| Model               | Accuracy | F1 Score | Precision | Recall |
| ------------------- | -------- | -------- | --------- | ------ |
| Logistic Regression | 0.8183   | 0.8432   | 0.8475    | 0.8390 |
| Random Forest       | 0.8106   | 0.8323   | 0.8591    | 0.8071 |
| XGBoost (Best)      | 0.8031   | 0.8349   | 0.8158    | 0.8550 |
| LightGBM            | 0.8115   | 0.8403   | 0.8294    | 0.8515 |

🧠 SHAP Analizi
| Pozitif Kelimeler | Negatif Kelimeler |
| ----------------- | ----------------- |
| süper             | açılmıyor         |
| harika            | kötü              |
| mükemmel          | berbat            |
| güzel             |                   |
📌 Modelin pozitif ve negatif tahminlerde hangi kelimelere odaklandığı açıkça görülmektedir.

📂 Veri Seti
| Özellik         | Değer       |
| --------------- | ----------- |
| Toplam Yorum    | ~12.000     |
| Pozitif (4-5 ⭐) | %53         |
| Negatif (1-3 ⭐) | %47         |
| Kaynak          | Google Play |

🔍 Önemli Bulgular

-Bigram kullanımı (“çok iyi”, “hiç beğenmedim”) performansı artırdı

-Büyük harf kullanımı ve ünlem işaretleri duygu için önemli sinyal

-XGBoost modeli en dengeli sonucu verdi


🚀 Kurulum
```bash
git clone https://github.com/alimkacar/Turkish_App_Review_Sentiment_Analysis_with_Google_Play_Scrapper.git

cd Turkish_App_Review_Sentiment_Analysis_with_Google_Play_Scrapper

pip install -r requirements.txt
```
▶️ Kullanım
```bash
jupyter notebook
```

Notebook dosyasını açıp adım adım çalıştırabilirsiniz.
