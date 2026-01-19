# Capstone Project - Bank Telemarketing Campaign Data Analysis and Conversion Predictionn 


## 📌 Overview
This project, within the Financial and Risk Analytics domain, presents a data-driven analysis to predict the success of a Portuguese bank’s telemarketing campaign aimed at selling long-term bank deposits. The solution supports customer segmentation, customer profile insights, and campaign optimization by predicting the likelihood of success for telemarketing calls based on customer characteristics.

---

## 🎯 Business Objective
The key objectives of this project are to:
- Predict whether a telemarketing contact will be successful or unsuccessful
- Identify key factors influencing telemarketing campaign performance
- Determine the most suitable customer segments for future marketing campaigns
- Propose data-driven improvements to optimize marketing strategies
- Recommend specific customers to target for higher conversion rates

---

## 📂 Dataset
The dataset is based on the UCI Bank Marketing Dataset, enriched with social and economic indicators, and published by Banco de Portugal. It is publicly available through official statistical sources.
The dataset contains 21 features, including:

- Bank Client Data: Age, job, marital status, education, credit default, housing loan, personal loan, contact communication type, last contacted month/day, and call duration (seconds)
- Previous Campaign Data: Number of contacts during the current and previous campaigns, days since last contact, and outcome of the previous campaign
- Socioeconomic Indicators: Employee variation rate, Consumer Price Index (CPI), Consumer Confidence Index (CCI), 3-month Euribor rate, and quarterly number of employees

The target variable indicates whether the client subscribed to a term deposit.

---

## 🛠️ Tools & Technologies

- **Language:** R  
- **Libraries:** pander, MLmetrics, randomForest, caret, mice , e1071, pROC,rpart  
- **Environment:** RStudio , Tableau

---

## 🧪 Methodology

1. **Data Understanding**
   - Performed exploratory data analysis (EDA) to understand data structure, distributions, and patterns
   - Handled missing values, inconsistencies, and duplicate records
     
2. **Feature Engineering**
   - Conducted feature aggregation, encoding, and correlation analysis
   - Removed non-informative and redundant features

3. **Model Building**
   - Developed multiple classification models including Logistic Regression, Naive Bayes, Support Vector Machine, Decision Tree, Random Forest, Neural Network, and XGBoos
   - Selected models based on interpretability and relevance to financial risk modeling
     
4. **Model Validation & Threshold Optimization**
   - Evaluated models using classification metrics, ROC-AUC, and Gini Coefficient
   - Optimized decision thresholds to balance customer acquisition risk and campaign resource utilization

6. **Customer Segmentation**
   - Identified high-potential customer segments for future telemarketing campaigns

7. **Business Insights & Recommendations**
   - Translated model outputs into actionable business insights and strategic recommendations

---

## 📈 Key Outcomes

- Random Forest was identified as the most accurate model, achieving 96% accuracy with strong predictive performance 
- Feature importance and pruning techniques improved customer classification accuracy 
- Customers were segmented into high-probability conversion groups for future campaigns

---

## 💼 Business Impact
The insights from this project help financial institution to:

- Apply the best-performing machine learning model to predict customer responses
- Optimize telemarketing campaigns by balancing budget and conversion costs 
- Improve overall telemarketing success rates through data-driven targeting

---

## 👩‍💻 Author
** Latesh Chaudhari **  
Analytics Engineer 
