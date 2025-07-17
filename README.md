# ✈️ British Airways Data Science Virtual Internship

This repository includes two data science tasks completed as part of the **British Airways Data Science Virtual Internship** on the [Forage](https://www.theforage.com/) platform:

- **Task 1:** Web Scraping & Sentiment Analysis  
- **Task 2:** Predictive Modeling of Customer Bookings

---

## 📌 Task Overview

| Task       | Description                                                                      | Tools & Libraries Used                                   |
|------------|----------------------------------------------------------------------------------|----------------------------------------------------------|
| **Task 1** | Collected and analyzed customer reviews from Skytrax using sentiment analysis   | `BeautifulSoup`, `NLTK`, `TextBlob`, `VADER`, `WordCloud` |
| **Task 2** | Developed ML models to predict whether users would complete a flight booking    | `pandas`, `scikit-learn`, `RandomForest`, `matplotlib`, `seaborn` |

---

## 🛠️ Task 1 – Web Scraping & Sentiment Analysis

### 🎯 Objective
Scrape British Airways customer reviews from Skytrax and perform sentiment analysis to identify customer satisfaction patterns.

### 🔍 Key Steps
- Collected ~1000 reviews using `requests` and `BeautifulSoup`.
- Preprocessed text using `NLTK` (tokenization, stopwords, POS tagging).
- Applied sentiment analysis:
  - `VADER` SentimentIntensityAnalyzer
  - `TextBlob` polarity scoring
- Created visual summaries with word clouds and frequency charts.

### 📊 Key Results
- **VADER:** ~61% positive reviews  
- **TextBlob:** ~67% positive sentiment  
- Common keywords: *service*, *flight*, *crew*, *food*

---

## 🤖 Task 2 – Predictive Modeling of Customer Bookings

### 🎯 Objective
Build a machine learning model to predict whether a user will complete a flight booking.

### 🔍 Key Steps
- Performed EDA and feature engineering (e.g., `days_to_flight`, `length_of_stay`)
- Addressed class imbalance and outliers.
- Evaluated feature importance using `mutual_info_classif`.

### 📈 Model Performance
- **Model:** Random Forest Classifier  
- **Train Accuracy:** 99.98%  
- **Test Accuracy:** 88.05%  
- ROC AUC and confusion matrix used for evaluation.

### ✅ Recommendations
- Use `class_weight='balanced'` to address class imbalance
- Consider improving with `SMOTE`, `XGBoost`, or hyperparameter tuning via `GridSearchCV`.

---

## 📂 Directory Structure

```plaintext
├── Task 1/
│   └── Task1_british_airways_web_scraping.ipynb
├── Task 2/
│   └── Task2_Predictive_modeling_of_customer_bookings.ipynb
├── requirements.txt
└── README.md
```

---

## ⚙️ Installation

```bash
# Install the required packages
pip install -r requirements.txt

# Launch the Jupyter Notebook interface
jupyter notebook
```

---

## 👩‍💻 Author

**Ece Yavuzyilmaz**  
Participant, British Airways Data Science Virtual Internship  
🔗 [GitHub Profile](https://github.com/eceyy)
