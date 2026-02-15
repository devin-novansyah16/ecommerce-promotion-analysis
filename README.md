# Evaluasi Efektivitas Kampanye Promosi Digital E-Commerce


## 📁 Project Structure

```
├── Dataset_eCommerce.xlsx    # Raw dataset containing e-commerce customer data
├── Project Analisis.ipynb    # Jupyter notebook with full data analysis
└── README.md                 # This file
```

---

## 📋 Dataset Description

The dataset contains **1,000 records** with **11 variables** divided into three main categories:

### 1. Customer Data
| Variable | Description |
|----------|-------------|
| customer_id | Unique customer identifier |
| gender | Customer gender |
| age | Customer age |
| city | Customer city |
| customer_rating | Customer satisfaction rating |

### 2. Transaction Data
| Variable | Description |
|----------|-------------|
| total_transaction | Total transaction value |
| transaction_count | Number of transactions |
| last_purchase_days | Days since last purchase |

### 3. Promotion Data
| Variable | Description |
|----------|-------------|
| promo_type | Type of promotion |
| promo_click | Whether customer clicked on promotion |
| promo_conversion | Whether customer converted from promotion |

---

## 🔬 Analysis Methodology

### 1. Data Collection
- Identification of data types and variables
- Defining objectives for each data category

### 2. Data Understanding
- Examining dataset structure
- Identifying data types and variables
- Checking for missing values

### 3. Data Cleaning
- Handling missing values using median imputation
- Data validation after cleaning

### 4. Exploratory Data Analysis (EDA)
- Distribution analysis of customer characteristics
- Relationship analysis between promotion and conversion
- Correlation heatmap analysis

### 5. Data Modeling
- **Classification Model**: Logistic Regression for predicting promotion conversion
- **Clustering Model**: K-Means for customer segmentation

---

## 📈 Key Findings

### Model Performance
- The Logistic Regression model effectively predicts customer conversion probability
- ROC-AUC Score provides measure of model discriminative ability

### Business Insights
1. **Targeted Marketing**: Model helps identify customers likely to respond to promotions
2. **Budget Optimization**: Efficient allocation of promotional budget
3. **Personalized Strategy**: More effective promotional campaigns based on customer behavior
4. **Customer Segmentation**: K-Means clustering identifies distinct customer groups

---

## 🛠️ Tools & Libraries Used

```
python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
from sklearn.model_selection import train_test_split
from sklearn.preprocessing import LabelEncoder, StandardScaler
from sklearn.linear_model import LogisticRegression
from sklearn.cluster import KMeans
from sklearn.metrics import classification_report, confusion_matrix, roc_auc_score, roc_curve
```

---

## 📝 How to Run

1. Ensure you have Python installed with the following libraries:
   
```
bash
   pip install pandas numpy matplotlib seaborn scikit-learn openpyxl
   
```

2. Open `Project Analisis.ipynb` in Jupyter Notebook or Google Colab

3. Run the cells sequentially to see the complete analysis

---

## 📌 Conclusions

Based on the analysis, the effectiveness of digital promotional campaigns is influenced by:
- Customer interaction with promotions (promo_click)
- Previous transaction behavior
- Customer characteristics (age, transaction patterns)

The results can be used to:
- Improve promotional effectiveness
- Optimize marketing costs
- Support data-driven strategic decision making

---

## 📄 License

This project is for educational purposes.

---

*Created for Data Analytics Course*
