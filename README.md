# Sentiment Analysis of Tweets
────────── ✦ ──────────  
**Classifying tweets as Positive, Neutral, or Negative**

---

## 📌 Project Overview

This project focuses on performing **sentiment analysis on tweets** using the **Sentiment140 dataset**.  
The goal is to classify tweets into **Negative, Neutral, or Positive sentiments** using machine learning techniques and natural language processing (NLP).

---

## 🎯 Objectives

- Clean and preprocess raw tweet text  
- Perform exploratory data analysis (EDA)  
- Convert text into numerical features using TF-IDF  
- Train and evaluate machine learning models  
- Compare multiple models and select the best one  
- Visualize model performance  

---

## 📂 Dataset

- **Dataset Name:** Sentiment140  
- **Total Tweets:** 1,600,000  
- **Sentiment Labels:**
  - `0` → Negative  
  - `2` → Neutral  
  - `4` → Positive  

> Note: The dataset does not include column headers, so `header=None` was used while loading the data.

---

## 🛠️ Technologies Used

- **Language:** Python  
- **Libraries:**
  - pandas  
  - numpy  
  - matplotlib  
  - seaborn  
  - scikit-learn  
  - nltk  

---

## 🔄 Project Workflow

1. **Data Loading**
   - Loaded dataset using pandas
   - Checked dataset size, missing values, and duplicates  

2. **Data Cleaning**
   - Dropped unnecessary columns
   - Cleaned tweet text by:
     - Lowercasing
     - Removing URLs, mentions, hashtags
     - Removing special characters  

3. **Exploratory Data Analysis (EDA)**
   - Analyzed sentiment distribution
   - Visualized class balance using bar charts  

4. **Feature Engineering**
   - Converted text into numerical features using **TF-IDF**
   - Used `max_features = 5000`  

5. **Train-Test Split**
   - 80% training data
   - 20% testing data  

6. **Model Training**
   - Multinomial Naive Bayes
   - Logistic Regression  

7. **Model Evaluation**
   - Accuracy
   - Precision
   - Recall
   - F1-score
   - Confusion Matrix  

8. **Visualization**
   - Confusion matrices using seaborn heatmaps  

---

## 🤖 Models Used

### Multinomial Naive Bayes
- Fast and efficient for large text datasets  
- Accuracy: **76%**

### Logistic Regression
- Works well with high-dimensional TF-IDF features  
- Accuracy: **79%**

---

## 📊 Results

| Model | Accuracy |
|------|----------|
| Naive Bayes | 76% |
| **Logistic Regression** | **79%** |

---

## 🏁 Conclusion

Two machine learning models were evaluated for tweet sentiment classification.  
Naive Bayes achieved **76% accuracy**, while Logistic Regression performed better with **79% accuracy**.  
Therefore, **Logistic Regression was selected as the final model**.

a Scientist | Machine Learning Enthusiast
