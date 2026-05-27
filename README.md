# OIBSIP — Data Analytics Internship

## Oasis Infobyte | Data Analytics Track

This repository contains all project submissions for my Data Analytics internship at Oasis Infobyte.

---


## Task 1 — Exploratory Data Analysis (EDA) on Retail Sales Data

**Folder:** `Task-1_EDA-Retail-Sales/`

### Objective
Analyze retail sales transactions and McDonald's menu nutritional data to extract actionable insights for business decision-making.

### Steps Performed
- Loaded and inspected datasets (retail sales, McDonald's menu)
- Handled missing values, checked data types, and removed duplicates
- Performed univariate and bivariate analysis on customer demographics and spending
- Analyzed monthly sales trends and category-wise revenue
- Examined nutritional profiles across menu categories
- Generated correlation heatmaps and visual summaries

### Tools Used
Python, Pandas, NumPy, Matplotlib, Seaborn

### Outcome
- Electronics and Clothing drive highest revenue; female customers spend more
- Peak sales in Nov-Dec holiday season; age group 30–50 has highest per-transaction value
- Breakfast items are highest in calories and fat
- Strong correlation between serving size and total calories

**Notebooks:** `1_retail_sales_analysis.ipynb`, `2_mcdonalds_menu_analysis.ipynb`

---

## Task 2 — Customer Segmentation

**Folder:** `Task-2_Customer-Segmentation/`

### Objective
Segment e-commerce customers based on spending behavior, demographics, and campaign responses to enable targeted marketing.

### Steps Performed
- Loaded and explored customer data (2,205 records, 39 features)
- Standardized features using StandardScaler
- Applied PCA for dimensionality reduction and 2D visualization
- Implemented K-Means clustering with Elbow Method and Silhouette Score
- Profiled each cluster to derive business insights

### Tools Used
Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn (PCA, K-Means)

### Outcome
- Identified 4 customer segments: Premium High-Spenders, Budget-Conscious Shoppers, Occasional Buyers, Loyal Regulars
- Premium segment has highest income ($80K+) and campaign acceptance rate
- Loyal Regulars have lowest spend but highest web visits — potential for engagement

**Notebook:** `customer_segmentation.ipynb`

---

## Task 3 — Data Cleaning

**Folder:** `Task-3_Data-Cleaning/`

### Objective
Comprehensively clean NYC Airbnb listings data to make it ready for reliable downstream analysis.

### Steps Performed
- Loaded and inspected 48,895 Airbnb listings
- Detected and handled missing values in key columns
- Converted data types (datetime parsing for `last_review`)
- Removed outliers using IQR method on `price` and `minimum_nights`
- Handled duplicate records
- Engineered new features and saved cleaned dataset

### Tools Used
Python, Pandas, NumPy, Matplotlib, Seaborn

### Outcome
- Reduced dataset from 48,895 to 39,728 rows (~18.7% reduction)
- Zero duplicates retained; cleaned data saved as `AB_NYC_2019_cleaned.csv`
- Manhattan has highest average prices; Brooklyn second
- Most listings are Entire home/apt type

**Notebook:** `data_cleaning_complete.ipynb`

---

## Task 4 — Sentiment Analysis

**Folder:** `Task-4_Sentiment-Analysis/`

### Objective
Classify tweet sentiment as Positive, Neutral, or Negative using lexicon-based and machine learning approaches.

### Steps Performed
- Loaded and explored 162,980 labeled tweets
- Preprocessed text (lowercasing, regex cleanup, stopword removal)
- Applied VADER lexicon-based sentiment scoring
- Vectorized text using TF-IDF and Bag-of-Words
- Trained Logistic Regression and Linear SVM classifiers
- Evaluated models with confusion matrices and accuracy scores

### Tools Used
Python, Pandas, NumPy, NLTK (VADER), Scikit-learn (TF-IDF, Logistic Regression, Linear SVM), Matplotlib, Seaborn

### Outcome
- Linear SVM + TF-IDF achieved highest accuracy: **94.30%**
- Logistic Regression + TF-IDF: **92.62%**
- VADER lexicon: ~56.8% agreement with true labels
- Common positive words: modi, vote, win, support; negative: fail, corruption, hate

**Notebook:** `sentiment_analysis.ipynb`

---

## Task 5 — House Price Prediction

**Folder:** `Task-5_House-Price-Prediction/`

### Objective
Predict house prices using linear regression based on structural and locational features.

### Steps Performed
- Loaded and explored housing dataset (545 records, 13 columns)
- Encoded binary categorical variables (yes/no → 1/0)
- One-hot encoded furnishing status
- Scaled features using StandardScaler
- Split data into 80% training and 20% testing
- Trained Linear Regression model
- Evaluated using MSE and R² Score
- Visualized predictions vs actual values, residuals, and feature importance

### Tools Used
Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn (Linear Regression, StandardScaler, train_test_split)

### Outcome
- Test R² Score: ~0.65–0.70
- Top predictors: area, parking, bedrooms, airconditioning
- Furnished homes command higher prices than unfurnished
- Residual analysis shows some heteroscedasticity for expensive homes

**Notebook:** `House_Price_Prediction.ipynb`

---

## Task 6 — Wine Quality Prediction

**Folder:** `Task-6_Wine-Quality-Prediction/`

### Objective
Predict wine quality (on a scale of 0–10) based on its chemical characteristics using multiple classification models.

### Steps Performed
- Loaded and explored wine quality dataset (1,143 records, 12 chemical features + quality label)
- Performed Exploratory Data Analysis (EDA) with visualizations of feature distributions and correlations
- Scaled features using StandardScaler
- Split data into 80% training and 20% testing
- Trained three classifier models: Random Forest, Stochastic Gradient Descent (SGD), and Support Vector Classifier (SVC)
- Evaluated models using accuracy, precision, recall, F1-score, and confusion matrices

### Tools Used
Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn (Random Forest, SGD, SVC, StandardScaler)

### Outcome
- **Random Forest** achieved the highest accuracy: **68.56%**
- Support Vector Classifier: **65.94%**
- Stochastic Gradient Descent: **55.46%**
- Random Forest emerged as the best performer for wine quality prediction due to its ability to capture complex non-linear patterns
- Alcohol content, volatile acidity, and sulphates were among the strongest predictors of quality

**Notebook:** `Wine_qua_pred.ipynb`

---

## Repository Structure

```
OIBSIP/
├── Task-1_EDA-Retail-Sales/
├── Task-2_Customer-Segmentation/
├── Task-3_Data-Cleaning/
├── Task-4_Sentiment-Analysis/
├── Task-5_House-Price-Prediction/
├── Task-6_Wine-Quality-Prediction/
├── Task-7_Fraud-Detection/
└── README.md
```
