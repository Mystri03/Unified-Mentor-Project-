# Unified-Mentor-Project-

# 🧪 Data Science Internship Projects — Unified Mentor

**Intern:** Mahi Mistry &nbsp;|&nbsp; 📧 mistrymahi3@gmail.com &nbsp;|&nbsp; ⏳ 3-Month Internship

> A collection of **4 end-to-end Data Science projects** completed during my internship at **Unified Mentor**, covering Machine Learning, NLP, Time Series Forecasting, Data Analysis, and Anomaly Detection.

---

## 📁 Table of Contents

1. [🌍 Climate Change Modeling](#-project-1-climate-change-modeling)
2. [☕ Coffee Sales Analysis](#-project-2-coffee-sales-analysis)
3. [📸 Instagram Fake Account Detection](#-project-3-instagram-fake-spammer--genuine-account-detection)
4. [🚬 Tobacco Use & Mortality Analysis](#-project-4-tobacco-use--mortality-analysis-2004--2015)
5. [🛠️ Tech Stack](#️-tech-stack)

---

## 🌍 Project 1: Climate Change Modeling

### Overview
Analyzed long-term climate data including **global temperatures, CO₂ emissions, and sea levels** to understand how climate patterns are shifting over time. Applied statistical and predictive models to forecast future climate scenarios and highlight the link between human activity and environmental change.

### Key Objectives
- 📊 **Part 1 — Sentiment Analysis:** Analyzed public comments on climate change using NLP to classify sentiments (Neutral: 46%, Positive: 37.2%, Negative: 16.9%)
- 🤖 **Part 2 — Climate Indicator Prediction:** Used Gradient Boosting & Random Forest to predict social media engagement metrics (likes) related to climate content
- 📈 **Part 3 — Time Series Trend:** Applied KMeans Clustering (K=3/4) to segment climate-related posts into low-engagement, high-discussion, and viral categories

### Key Findings
- Neutral sentiment dominates public discourse on climate change
- Random Forest (R²=0.25) and Gradient Boosting (R²=0.30) both showed under-prediction bias for high engagement posts
- KMeans clustering effectively separated viral content from low-activity posts
- Word cloud showed "earth", "climate", "temperature" as dominant discussion terms

### 🔧 Tools & Technologies
| Category | Tools |
|---|---|
| Language | Python |
| IDE | Jupyter Notebook |
| Data Analysis | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn, WordCloud |
| Machine Learning | Scikit-learn (Random Forest, Gradient Boosting, KMeans) |
| NLP | NLTK, TextBlob |
| Dataset | NASA Climate Data (`climate_nasa.csv`), YouTube Comments |

### Methodologies
`Machine Learning` · `NLP / Sentiment Analysis` · `Time Series Forecasting` · `KMeans Clustering`

---

## ☕ Project 2: Coffee Sales Analysis

### Overview
Examined transactional sales data to uncover **purchasing behaviors, seasonal demand, and regional preferences**. Identified top-performing products and customer segments to support business decision-making on inventory and marketing strategy.

### Key Objectives
- 📅 **Part 1 — Sales Trends & Customer Behavior:** Analyzed monthly, weekly, and hourly sales patterns; payment method breakdown
- 🛒 **Part 2 — Product Popularity & Demand Forecasting:** Identified top revenue products and attempted Random Forest-based sales forecasting
- 👥 **Part 3 — Customer Segmentation & Anomaly Detection:** Applied KMeans clustering to segment customers; used Isolation Forest for anomaly detection in daily sales

### Key Findings
- Revenue is stable (₹7,200–₹8,200/month) with peaks in May 2024
- Two clear daily peaks: **9–11 AM** (morning rush) and **7 PM** (evening)
- Latte, Americano with Milk, and Cappuccino are the top 3 revenue drivers
- **92.1% of sales** are card payments — business is nearly cashless
- Isolation Forest detected anomaly spikes in daily revenue (₹500–₹600 range)
- KMeans Cluster 0 (high-value customers) overwhelmingly prefers Latte & Cappuccino

### 🔧 Tools & Technologies
| Category | Tools |
|---|---|
| Language | Python |
| IDE | Jupyter Notebook |
| Data Analysis | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn (Random Forest, KMeans, Isolation Forest) |
| Dataset | Coffee Sales Transactions (`index.csv`) |

### Methodologies
`Exploratory Data Analysis (EDA)` · `Time Series Forecasting` · `Customer Segmentation` · `Anomaly Detection`

---

## 📸 Project 3: Instagram Fake Spammer & Genuine Account Detection

### Overview
Applied machine learning to **classify Instagram accounts** as genuine, fake, or spam using behavioral and profile features like follower ratios, posting activity, and engagement levels.

### Key Objectives
- 🔍 Detect fake and spam accounts using profile-based features
- 📊 Feature engineering: `log_followers`, `follower_following_ratio`, `username_len_ratio`
- 🤖 Train classification models and evaluate using SHAP for feature importance
- 📉 Analyze behavioral patterns distinguishing real vs. fake accounts

### Key Findings
- `log_followers` and `follower_following_ratio` are the **strongest predictors** of account authenticity
- Real accounts hold all extreme follower outliers (up to 15M followers)
- Fake accounts are almost exclusively concentrated in the low-engagement cluster
- Account privacy status showed minimal predictive power
- SHAP analysis confirmed `username_len_ratio` as a significant secondary feature

### 🔧 Tools & Technologies
| Category | Tools |
|---|---|
| Language | Python |
| IDE | Jupyter Notebook |
| Data Analysis | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn (Classification Models) |
| Explainability | SHAP (Feature Importance) |
| Dataset | Instagram Train/Test CSVs (`train.csv`, `test.csv`) |

### Methodologies
`Binary Classification` · `Feature Engineering` · `SHAP Explainability` · `Exploratory Data Analysis`

---

## 🚬 Project 4: Tobacco Use & Mortality Analysis (2004–2015)

### Overview
Analyzed tobacco use and associated mortality patterns in India over an 11-year period. Explored **smoking prevalence across age groups**, household expenditure on tobacco, affordability trends, and relationships between tobacco consumption and mortality rates to inform public health policy.

### Key Objectives
- 📈 **Part 1 — Smoking Trends & Mortality Risk:** Correlation analysis between tobacco-related factors and mortality using heatmaps; smoking prevalence by age group over time
- 🏥 **Part 2 — Smoking-Related Disease Classification:** Classified hospital admissions using SVM, Logistic Regression, and KMeans; analyzed top 10 smoking-related diagnoses

### Key Findings
- **35–49 age group** has the highest smoking prevalence (30%), followed by 50–59 (25%)
- Overall smoking rates show a **declining trend** from 2006–2014 across all age groups
- Strong positive correlation between tobacco price/retail indexes and mortality in older age groups (60+)
- SVM and Logistic Regression achieved ~100% accuracy but failed on minority class due to **severe class imbalance**
- Chronic Obstructive Lung Disease among top smoking-related diagnoses with ~7,600 admissions
- KMeans clustering achieved ~67% accuracy as an unsupervised baseline

### 🔧 Tools & Technologies
| Category | Tools |
|---|---|
| Language | Python |
| IDE | Jupyter Notebook |
| Data Analysis | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn (SVM, Logistic Regression, KMeans) |
| Dataset | `tobacco_mortality.xls`, `admissions.csv`, `fatalities.csv`, `smokers.csv` |

### Methodologies
`Exploratory Data Analysis` · `Correlation Analysis` · `Classification` · `Clustering` · `Public Health Analytics`

---

## 🛠️ Tech Stack

```
Languages        →  Python
IDE              →  Jupyter Notebook
Data Analysis    →  Pandas, NumPy
Visualization    →  Matplotlib, Seaborn, WordCloud
Machine Learning →  Scikit-learn
  Algorithms     →  Random Forest, Gradient Boosting, SVM,
                    Logistic Regression, KMeans, Isolation Forest
NLP              →  NLTK, TextBlob
Explainability   →  SHAP
File Formats     →  CSV, XLS, XLSX, IPYNB
```

---

## 📊 Skills Demonstrated

- ✅ Exploratory Data Analysis (EDA)
- ✅ Data Cleaning & Preprocessing
- ✅ Feature Engineering
- ✅ Supervised Machine Learning (Classification & Regression)
- ✅ Unsupervised Learning (Clustering)
- ✅ Natural Language Processing (Sentiment Analysis)
- ✅ Time Series Analysis & Forecasting
- ✅ Anomaly Detection
- ✅ Model Evaluation & Interpretation (SHAP)
- ✅ Data Visualization & Storytelling
- ✅ Public Health & Business Domain Analytics

---

## 🏢 About the Internship

**Organization:** Unified Mentor  
**Duration:** 3 Months  
**Role:** Data Science Intern  
**Projects Completed:** 4

---

*Thank you for visiting! Feel free to explore the project notebooks for full code, visualizations, and detailed analysis.* 🙏
