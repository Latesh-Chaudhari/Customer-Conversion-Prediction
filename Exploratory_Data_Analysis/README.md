<h1 align="center"> :large_orange_diamond:#Exploratory Data Analysis :large_orange_diamond: </h1>

#### A. Target Variable Distribution
![Subscription Rate](images/Subscribed_target_variable.png)

The target variable shows the subscription distribution across all customers. In the given data set, 11.27% of customers subscribed for term deposit.

#### B.Features
**<ins>Age:</ins>**
![Age Distribution](images/Histogram_Age_Group.png)

- Age binned into 7 categories (0-25, 25-35, 35-45, 45-55, 55-65, 65-75, 75-85, 85+)
- Majority of customers fall in 25-45 age bracket 

![Customer Response by Age Group](images/Subscribed_vs_Age_Group.png)

**Interpretation** : Customers of age group 35-55 (working class) are likely not to subscribe to term deposit products.

**<ins>Job:</ins>**
![Job Distribution](images/Subscribed_vs_Job_Category.png)

25% of customers in job group “Retired” and 31% of the customers in “Student” category have responded positively for subscription and this observation lies in sync with our analysis of customers responses based on Age group. An interesting observation is 14% of “Unemployed” customers responded positively as well.

**Interpretation**: Customers with blue collar jobs are likely not to subscribe to term deposit products.

**<ins>Marital:</ins>**
![Marital Status Distribution](images/Subscribed_vs_Marital_Status.png)

Distribution- Married (60%), Single (28%), Divorced (12%)  
**Interpretation**: Overall Balanced representation of subscription within categories

**<ins>Default:</ins>**  
![Default vs Subscription](images/Subscribed_vs_default.png)

**Interpretation**: Customers with no defaults have higher subscription rates

**<ins>Contact:</ins>**  
![Contact Type vs Subscription](images/Subscribed_vs_contact_type.png)

**Interpretation**
   - **Critical Finding:** Cellular contact shows dramatically higher subscription rates (~18-20%)
   - **Telephone contact:** Much lower subscription rates (~5-8%)
**Recommendation:** Prioritize cellular contact channels

**<ins>Call Duration:</ins>**
![Duration vs Subscription](images/Subscribed_vs_Contact_Duration.png)

 **Interpretation**  
    - **Strong Positive Correlation:** Longer calls significantly increase subscription probability
    - **180+ seconds:** > 30% subscription rate  
 **Insight:** Call quality and engagement crucial for conversion 

**<ins>Campaign Contact:</ins>**
![Campaign Contacts vs Subscription](images/Subscribed_vs_No_of_Contacts.png)

**Interpretation**
   - 1-3 contacts show highest conversion
   - 5+ contacts show diminishing returns/negative impact
**Insight:** Optimal contact frequency exists

**<ins>Consumer Confidence:</ins>**
![Consumer Confidence vs Subscription](images/Subscribed_vs_consumer_confidence_index.png)

Consumer confidence, measured by the Consumer Confidence Index (CCI), is defined as the degree of optimism about the state of the economy that consumers are expressing through their activities of saving and spending.  
**Interpretation**
  - Strong positive correlation: Higher confidence → higher subscriptions
  - Economic sentiment critical factor


###Correlation Matrix:



