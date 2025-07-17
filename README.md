# ✈️ British Airways Data Science Virtual Internship

Bu repoda, [Forage](https://www.theforage.com/) platformu üzerinden gerçekleştirilen **British Airways Sanal Veri Bilimi Stajı** kapsamında tamamlanan iki görev (Task 1 & Task 2) yer almaktadır:

- **Task 1:** Web Scraping & Sentiment Analysis  
- **Task 2:** Predictive Modeling of Customer Bookings

---

## 📌 Görev Özeti

| Görev | Açıklama | Teknolojiler |
|-------|----------|--------------|
| **Task 1** | Skytrax web sitesinden British Airways yolcu yorumlarının çekilmesi ve duygu analizi yapılması | `BeautifulSoup`, `VADER`, `TextBlob`, `NLTK`, `WordCloud` |
| **Task 2** | Rezervasyon tamamlanma durumunu tahmin etmek için makine öğrenimi modeli oluşturulması | `Pandas`, `Random Forest`, `sklearn`, `matplotlib`, `seaborn` |

---

## 📂 Dizin Yapısı

📁 Task 1
└── Task1_british_airways_web_scraping.ipynb
📁 Task 2
└── Task2_Predictive_modeling_of_customer_bookings.ipynb
📄 README.md

markdown
Kopyala
Düzenle

---

## 🛠️ Task 1 – Web Scraping & Sentiment Analysis

### 🎯 Amaç
Skytrax web sitesinden British Airways yolcu yorumlarını çekip, pozitif/negatif sınıflandırmalar yaparak müşteri memnuniyetini analiz etmek.

### 🔍 Adımlar
- `requests` ve `BeautifulSoup` ile 1000'e yakın kullanıcı yorumu toplandı.
- Metin temizliği (stopword kaldırma, lemmatization, POS tagging) `NLTK` kullanılarak yapıldı.
- **Duygu analizi** için iki farklı yöntem kullanıldı:
  - **VADER Sentiment Analyzer**
  - **TextBlob** polarite skoru
- Kelime bulutu ve en sık geçen kelimelerle metin görselleştirmeleri yapıldı.

### 📊 Sonuçlar
- VADER’a göre yorumların yaklaşık %61’i pozitif.
- TextBlob analizinde pozitif oran %67’ye ulaşıyor.
- "Service", "food", "flight", "crew" gibi temalar ön planda.

---

## 🧠 Task 2 – Predictive Modeling of Bookings

### 🎯 Amaç
Müşterinin uçuş rezervasyonunu tamamlayıp tamamlamayacağını tahmin etmek.

### 🔍 Adımlar
- Veri seti analiz edilerek `continent`, `days_to_flight`, `length_of_stay` gibi değişkenler oluşturuldu.
- Aykırı değer temizliği, label encoding ve feature engineering işlemleri gerçekleştirildi.
- Özellik önemi `mutual_info_classif` ile değerlendirildi.

### 📈 Model
- Model: **Random Forest Classifier**
- Eğitim doğruluğu: 99.98% (overfitting işareti)
- Test doğruluğu: 88.05%
- Denge problemi gözlendi (class imbalance)

### 📌 Değerlendirme ve Öneriler
- `class_weight='balanced'` ile iyileştirme önerildi.
- ROC eğrisi ve confusion matrix ile model performansı görselleştirildi.
- Gelişmiş modelleme için SMOTE, XGBoost, GridSearchCV tavsiye edildi.

---

## 📊 Örnek Görselleştirmeler

<details>
<summary><b>Task 1 - WordCloud</b></summary>
<img src="https://user-images.githubusercontent.com/example/wordcloud.png" width="500"/>
</details>

<details>
<summary><b>Task 2 - Confusion Matrix</b></summary>
<img src="https://user-images.githubusercontent.com/example/confusion_matrix.png" width="400"/>
</details>

---

## 🔧 Kullanılan Kütüphaneler

- Web Scraping: `requests`, `BeautifulSoup`
- NLP: `nltk`, `vaderSentiment`, `TextBlob`, `wordcloud`
- Görselleştirme: `matplotlib`, `seaborn`
- ML: `scikit-learn`, `RandomForestClassifier`
- Yardımcılar: `pycountry_convert`, `numpy`, `pandas`

---

## 🚀 Kurulum & Çalıştırma

```bash
# Gerekli kütüphaneleri kurun
pip install -r requirements.txt

# Jupyter Notebook ile çalıştırın
jupyter notebook
