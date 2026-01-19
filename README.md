# Capstone Project - Bank Telemarketing campaign data analysis and conversion prediction 


## 📌 Overview
This Financial and risk analytics domain based project performs a data-driven study to predict the success of portugese bank telemarketing campaign for selling long term bank deposit to customers. The end solution supports data-driven customer segmentation , customer profiles insights to optimize campaign performance and predict success of telemarketing call based on customer profile. 

---

## 🎯 Business Objective
The key objectives of this project are to :
- Predict Whether it will be unsuccessful or successful contact
- Understand key factors impacting the preformance of telemarketing campaign
- Identify right customer segments for future marketing campaigns
- Propose improvements in marketing campaign for future campaigns
- Recommend exactly which customer to target

---

## 📂 Dataset
The dataset is based on bank marketing UCI dataset which was enriched with social and economic features and published by banco de portugal and publicaly available at https://www.bportugal.pt/estatisticasweb
It contains 21 features including 
- Bank Client data (Age , Job , Marital , Education , Default? , Loan , contact communication type ,Last concated Month-Day, contact duration in seconds)
- Previous Campaign Data ( Number of contacts performed during campaign , Number of contacts performed previous campaign, Number of days passed after last contacted from previous campaign , outcome of previous campaign
- Socio Economic data (Empolyee variation rate, Consumer Price Index , Consumer Confidence Index ,Euribor 3-Month Rate, Number of Employees in bank- Quarterly )  

The target variable indicates whether client has subscribed a term deposit 

---

## 🛠️ Tools & Technologies

- **Language:** R  
- **Libraries:** pander, MLmetrics, randomForest, caret, mice , e1071, pROC,rpart  
- **Environment:** R Studio , Tableau

---

## 🧪 Methodology

1. **Data Understanding**
   - Reviewed data structure, data types, and variable distributions by exploratory data analysis
   - Performed treatment for missing values ,inconsistent values, Duplicate values

2. **Feature Engineering**
   - Feature Aggregation , Feature Encoding , Correlation Analysis
   - Removed non-informative identifiers

3. **Model Building**
   - Developed models like Logistic Regression , Naive Bays , Support Vector Machine , Decision Tree , Random Forest , Neural Network , Xgboost
   - Chosen for interpretability and industry relevance in financial and Risk modelling domain
     
4. **Model Validation & Threshold Optimization**
   - Evaluated performance using classification metrics and ROC-AUC and Gini Coeficient
   - Optimized classification decisions to reduce risk of missing customer and considering resource utlization for campaign

6. **Customer Segmentation**
   - Segmented customer categories which could probably be added into future telemarketing campaign 

7. **Business Insights & Recommendations**
   - Translated model output into practical business insights and recommendations 

---

## 📈 Key Outcomes

- Random forest seems to be most accurate model with 96% accuracy with strong predictive performance  
- Optimized classification using pruning and importance variable to classify customer 
- Segmented customers into highly potential customers for converting in next telemarketing campaign

---

## 💼 Business Impact
The insights from this project help financial institution to:

- Use best performing Machine learning Model to predict the outcome of customer.  
- Apply budget-conversion cost optimized telemarketing campaign strategy 
- Improve success rate of telemarketing campaign  

---

## 👩‍💻 Author
** Latesh Chaudhari **  
Analytics Engineer 
