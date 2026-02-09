# 📩 Spam vs Ham Message Detection using Machine Learning

## 📌 Overview

Spam messages are a common problem in email and SMS communication, leading to wasted time, security risks, and poor user experience.
This project focuses on building a **machine learning-based text classification system** to automatically detect **spam** messages and distinguish them from **legitimate (ham)** messages using Natural Language Processing (NLP).

---

## 🎯 Business Problem

Manually filtering spam messages is inefficient and unreliable.
The objective of this project is to develop an automated solution that:

* Accurately identifies spam messages
* Minimizes false positives (important messages marked as spam)
* Works efficiently on real-world text data

---

## 🛠️ Tech Stack

* **Python**
* **Pandas, NumPy**
* **NLTK**
* **Scikit-learn**
* **Matplotlib, Seaborn**
* **SMOTE (Imbalanced-learn)**

---

## 🔄 Project Workflow

### 1️⃣ Data Understanding

* Dataset contains labeled messages categorized as **Spam** or **Ham**
* Significant class imbalance observed (more ham messages than spam)

---

### 2️⃣ Text Preprocessing

To improve data quality and model performance:

* Converted text to lowercase
* Removed punctuation and stopwords
* Applied **lemmatization** (preferred over stemming for meaningful normalization)
* Transformed text into numerical features using **count-based vectorization**

---

### 3️⃣ Exploratory Data Analysis (EDA)

Key observations:

* **Spam messages** are dominated by promotional and urgency-driven words such as *free, call, now, new*
* **Ham messages** contain conversational and contextual words like *ok, meeting, deal, contract*
* Spam vocabulary is more repetitive, while ham messages show greater linguistic diversity

#### Message Length Analysis:

* Spam messages tend to be **longer and more consistent in length**
* Ham messages are usually **shorter**, with a few extreme long outliers

These patterns confirmed that **word frequency and message length** are strong distinguishing features.

---

### 4️⃣ Handling Class Imbalance

* Applied **SMOTE (Synthetic Minority Oversampling Technique)**
* Improved the model’s ability to correctly identify spam messages

---

### 5️⃣ Model Building

* Used **Multinomial Naive Bayes**
* Chosen for its effectiveness with count-based text features and interpretability

---

### 6️⃣ Model Evaluation

Model performance was evaluated using:

* **Precision**
* **Recall**
* **F1-score**

These metrics provided a more reliable assessment than accuracy alone, especially for imbalanced data.

---

## 📊 Key Insights

* Spam messages rely heavily on repetitive, keyword-driven language
* Ham messages reflect natural human communication
* Message length is a useful feature for spam classification
* Proper preprocessing significantly improves feature quality and model performance

---

## ✅ Final Conclusion

* Lemmatization produced better results than stemming
* SMOTE effectively handled class imbalance
* Multinomial Naive Bayes delivered strong, interpretable performance
* The final model achieved a good balance between accuracy and reliability

📌 This solution is suitable for **real-world spam detection scenarios**.

---

## 🚀 Future Improvements

* Experiment with TF-IDF and word embeddings
* Try advanced models like Logistic Regression or XGBoost
* Deploy the model as a web application or API

---

## 📎 Author

**Anand Pathak**
Aspiring Data Analyst | Machine Learning Enthusiast

