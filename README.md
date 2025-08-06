# Predictive-Analysis-on-Student-Performance

# 📊 Data-Driven Insights into Student Achievement: A Predictive Modeling Approach
**Contributors**: Saumya Joshi, Nishka Srikanth, Pavani Narala, Erica L. Williams

---

## 📌 Project Overview

This project applies machine learning to predict student performance based on factors like parental education, lunch type, and school location. Using Weka for data mining and modeling, the goal is to understand how demographic and contextual variables influence academic success, and how these insights can support data-driven educational interventions.

---

## 🎯 Objectives

- Identify key factors affecting student performance
- Build and evaluate classification models (Random Tree, Naive Bayes, MultiClass Classifier)
- Segment students using clustering to identify meaningful profiles
- Offer insights to improve educational equity and support systems

---

## 🗃️ Dataset

- **Source**: Kaggle (modified and cleaned for research)
- **Size**: 1,000 student records
- **Key Features**:
  - Gender
  - Location (school ranking)
  - Parental education
  - Lunch type (regular or free/reduced)
  - Test preparation course
  - Scores: Math, Reading, Writing
  - Derived field: `Pass/Fail`

---

## 🛠️ Data Preprocessing

- Replaced ambiguous `ethnicity` field with `location`
- Standardized education levels (e.g., "Some High School" → "GED")
- Created binary `Pass/Fail` label (cutoff score: 68)
- Removed redundant columns and normalized numerical fields
- Encoded categorical variables for Weka compatibility

---

## 🤖 Models Used

| Model                  | Accuracy | Kappa  | ROC AUC | Notes                                  |
|-----------------------|----------|--------|---------|----------------------------------------|
| Random Tree           | 99.4%    | 0.9875 | 0.993   | High interpretability and precision    |
| Naive Bayes           | 97.5%    | 0.948  | 0.999   | Fast and scalable, handles large features well |
| MultiClass Classifier | 98.8%    | 0.9748 | 0.997   | Robust for multi-class predictions     |

**Validation**: 10-fold stratified cross-validation for all models  
**Metrics Used**: Accuracy, F1-Score, Kappa Statistic, ROC AUC, Confusion Matrix

---

## 📊 Clustering Analysis

Used **K-Means Clustering** to identify 7 distinct student groups:

1. **Steady Students** – Consistent, mid-level scores  
2. **Young Professionals’ Students** – Mixed scores, high parental education  
3. **Average Students** – Baseline performance  
4. **Underserved High Performers** – High scores, low support  
5. **Consistent Students** – Gradual improvement with test prep  
6. **Top Performers** – High scores, high support  
7. **Under Performers** – Low scores, low support and prep

---

## 📈 Key Insights

- Students with **higher parental education** tend to perform better
- **Lunch type** correlates with performance, indicating SES impact
- **Location (school ranking)** significantly affects outcomes
- Some students succeed despite disadvantages, highlighting **resilience**

---

## 🔮 Future Work

- Incorporate real-time behavioral and engagement data
- Explore deep learning for non-linear patterns
- Build early-warning systems for at-risk students
- Expand dataset with household income and regional indicators

---

## 🧾 References

This work is based on research from peer-reviewed journals and educational data mining studies. A complete bibliography is available in the project report.


## 📬 Contact



Let me know if you'd like this content as a downloadable `.md` file or want to publish it to your GitHub repository — I can help format or upload it.
```
