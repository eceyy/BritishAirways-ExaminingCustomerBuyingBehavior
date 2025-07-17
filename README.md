# ✈️ British Airways Data Science Virtual Internship

This repository contains two completed tasks (Task 1 & Task 2) from the **British Airways Data Science Virtual Internship** available on the [Forage](https://www.theforage.com/) platform:

- **Task 1:** Web Scraping & Sentiment Analysis  
- **Task 2:** Predictive Modeling of Customer Bookings

---

## 📌 Task Overview

| Task   | Description                                                  | Technologies                          |
|--------|--------------------------------------------------------------|------------------------------------|
| **Task 1** | Scraping British Airways passenger reviews from Skytrax and performing sentiment analysis | `BeautifulSoup`, `VADER`, `TextBlob`, `NLTK`, `WordCloud` |
| **Task 2** | Building a machine learning model to predict completion of flight bookings                | `Pandas`, `Random Forest`, `scikit-learn`, `matplotlib`, `seaborn` |

---

## 📂 Directory Structure


---

## 🛠️ Task 1 – Web Scraping & Sentiment Analysis

### 🎯 Objective
Collect British Airways passenger reviews from the Skytrax website and analyze customer sentiment by classifying reviews as positive or negative.

### 🔍 Steps
- Scraped approximately 1000 user reviews using `requests` and `BeautifulSoup`.
- Cleaned text data with `NLTK` (removing stopwords, lemmatization, POS tagging).
- Applied two sentiment analysis techniques:
  - **VADER Sentiment Analyzer**
  - **TextBlob** polarity scoring
- Created visualizations including word clouds and most common words.

### 📊 Results
- About 61% of reviews were positive according to VADER.
- TextBlob sentiment analysis showed a 67% positive ratio.
- Common themes identified: "service," "food," "flight," "crew."

---

## 🧠 Task 2 – Predictive Modeling of Bookings

### 🎯 Objective
Predict whether a customer will complete a flight booking.

### 🔍 Steps
- Conducted exploratory data analysis and engineered features such as `continent`, `days_to_flight`, and `length_of_stay`.
- Performed outlier removal, label encoding, and feature engineering.
- Evaluated feature importance using `mutual_info_classif`.

### 📈 Model Details
- Model: **Random Forest Classifier**
- Training accuracy: 99.98% (possible overfitting)
- Test accuracy: 88.05%
- Noted class imbalance in the dataset.

### 📌 Evaluation and Recommendations
- Suggested balancing classes with `class_weight='balanced'`.
- Visualized model performance with ROC curve and confusion matrix.
- Recommended advanced techniques such as SMOTE, XGBoost, and GridSearchCV for improvement.

---

## 📊 Sample Visualizations

<details>
<summary><b>Task 1 - Word Cloud</b></summary>
<img src="https://user-images.githubusercontent.com/example/wordcloud.png" width="500"/>
</details>

<details>
<summary><b>Task 2 - Confusion Matrix</b></summary>
<img src="https://user-images.githubusercontent.com/example/confusion_matrix.png" width="400"/>
</details>

---

## 🔧 Libraries Used

- **Web Scraping:** `requests`, `BeautifulSoup`
- **NLP:** `nltk`, `vaderSentiment`, `TextBlob`, `wordcloud`
- **Visualization:** `matplotlib`, `seaborn`
- **Machine Learning:** `scikit-learn`, `RandomForestClassifier`
- **Utilities:** `pycountry_convert`, `numpy`, `pandas`

---

## 🚀 Setup & Execution

```bash
# Install required packages
pip install -r requirements.txt

# Launch Jupyter Notebook
jupyter notebook


## Author

**Ece Yavuzyilmaz**  
Participant of the British Airways Data Science Virtual Internship  
🔗 [GitHub Profile](https://github.com/eceyy)
