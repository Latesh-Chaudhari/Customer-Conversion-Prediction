## Exploratory Data Analysis

### 1. Univariate Analysis

#### A. Target Variable Distribution
![Subscription Rate](images/subscription_distribution.png)

The target variable shows the subscription distribution across all customers. The analysis reveals:
- **Imbalanced Classes:** Subscription rates are significantly lower than non-subscriptions
- **Business Impact:** Understanding subscription patterns is critical for targeted marketing

#### B. Demographic Features

**Age Distribution:**
![Age Distribution](images/age_histogram.png)

- Age binned into 7 categories (0-25, 25-35, 35-45, 45-55, 55-65, 65-75, 75-85, 85+)
- Majority of customers fall in 25-45 age bracket
- Right-skewed distribution with peak at 30-40 years

**Job Categories:**
![Job Distribution](images/job_distribution.png)

- 11 distinct job categories analyzed
- Top positions: Technician, Services, Management, Admin
- Blue-collar and retired workers form significant segments

**Marital Status:**
![Marital Status Distribution](images/marital_distribution.png)

- Distribution: Married (60%), Single (28%), Divorced (12%)
- Balanced representation across categories

**Education Levels:**
![Education Distribution](images/education_distribution.png)

- Primary levels: High School, University Degree, Basic Education
- Professional courses and illiteracy represent smaller segments
- Education impacts subscription propensity

#### C. Financial and Account Features

**Default History:**
![Default History](images/default_distribution.png)

- Majority customers have no default history (98%)
- Very few customers (2%) with credit defaults

**Housing Loan Status:**
![Housing Loan Distribution](images/housing_distribution.png)

- Nearly 40% customers have housing loans
- 60% without housing loans

**Personal Loan Status:**
![Personal Loan Distribution](images/loan_distribution.png)

- Lower penetration: ~8% with personal loans
- Most customers (92%) without personal loans

#### D. Campaign-Related Features

**Contact Type:**
![Contact Type Distribution](images/contact_distribution.png)

- Cellular: ~73% of contacts
- Telephone: ~27% of contacts
- Cellular contact shows higher engagement

**Call Duration Distribution:**
![Duration Distribution](images/duration_histogram.png)

- Right-skewed distribution
- Median duration: ~180 seconds (~3 minutes)
- Longer calls strongly correlate with positive outcomes
- Binned into 10 ranges: 0-60s, 60-120s, up to 540-600s+

**Campaign Contacts:**
![Campaign Distribution](images/campaign_histogram.png)

- Most customers contacted 1-3 times per campaign
- >10 contacts represent outliers
- Binned into 11 categories for analysis

**Previous Campaign Outcome:**
![Previous Outcome Distribution](images/poutcome_distribution.png)

- Nonexistent: ~80% (no previous contact)
- Success/Failure: ~20% (contacted in previous campaigns)
- High predictor of current subscription

**Days Since Previous Contact (pdays):**
![Pdays Distribution](images/pdays_histogram.png)

- Highly skewed with most at 0 (never contacted)
- When contacted previously, intervals vary widely

#### E. Economic Indicators

**Employment Variation Rate:**
![Employment Variation Rate](images/emp_var_rate_histogram.png)

- Ranges from -3.4 to 1.1
- Multimodal distribution reflecting economic cycles
- Correlates with market conditions

**Consumer Price Index:**
![Consumer Price Index](images/cons_price_idx_histogram.png)

- Normal distribution centered around 93-94
- Economic condition indicator
- Slight variations with subscription rates

**Consumer Confidence Index:**
![Consumer Confidence Index](images/cons_conf_idx_histogram.png)

- Ranges: -50 to 0
- Negative values reflect economic uncertainty
- Strong relationship with consumer behavior

**3-Month Euribor Rate:**
![Euribor Rate Distribution](images/euribor_histogram.png)

- Ranges: 0.7% to 5.045%
- Multiple peaks reflecting interest rate cycles
- Binned into 9 categories for analysis

**Number of Employees:**
![Number of Employees](images/nr_employed_histogram.png)

- Ranges: 4000-5200
- Indicates bank/economy scale
- Binned into 3 categories: 4000-4500, 4500-5000, >5000

#### F. Time-Based Features

**Contact Month:**
![Month Distribution](images/month_distribution.png)

- Higher contact volumes: May, June, July, November
- Seasonal patterns in marketing campaigns
- Some months show higher subscription rates

**Day of Week:**
![Day of Week Distribution](images/day_of_week_distribution.png)

- Monday to Friday distributed relatively evenly
- Weekday vs. weekend effects analyzed
- Weekdays slightly preferred for contact

---

### 2. Bivariate Analysis

#### A. Demographic Features vs. Subscription

**Age Group vs. Subscription:**
![Age vs Subscription](images/age_vs_subscription.png)

- **Finding:** Younger customers (25-35) and older customers (65+) show higher subscription rates
- **Insight:** Age groups 55+ demonstrate propensity to subscribe

**Job Type vs. Subscription:**
![Job vs Subscription](images/job_vs_subscription.png)

- **Top Subscribers:** Retired workers, students, entrepreneurs
- **Lower Subscribers:** Blue-collar workers, technicians
- **Business Insight:** Professional stability correlates with subscription

**Education vs. Subscription:**
![Education vs Subscription](images/education_vs_subscription.png)

- **Key Finding:** University-educated customers show higher subscription rates
- **Secondary Finding:** Basic education groups show lower subscription propensity
- **Insight:** Education level is strong predictor

**Marital Status vs. Subscription:**
![Marital vs Subscription](images/marital_vs_subscription.png)

- **Single customers:** Slightly higher subscription rates
- **Married customers:** Moderate subscription rates
- **Divorced customers:** Lower subscription rates

#### B. Financial Features vs. Subscription

**Default History vs. Subscription:**
![Default vs Subscription](images/default_vs_subscription.png)

- **Key Finding:** Customers with no defaults have higher subscription rates
- **Risk Factor:** Credit defaults strongly negatively impact subscription likelihood

**Housing Loan vs. Subscription:**
![Housing Loan vs Subscription](images/housing_vs_subscription.png)

- **Finding:** Customers with housing loans show lower subscription rates
- **Insight:** Financial burden reduces propensity to subscribe to additional services

**Personal Loan vs. Subscription:**
![Personal Loan vs Subscription](images/personal_loan_vs_subscription.png)

- **Finding:** Similar pattern to housing loans
- **Insight:** Multiple financial obligations reduce subscription likelihood

#### C. Campaign Features vs. Subscription

**Contact Type vs. Subscription:**
![Contact Type vs Subscription](images/contact_vs_subscription.png)

- **Critical Finding:** Cellular contact shows dramatically higher subscription rates (~18-20%)
- **Telephone contact:** Much lower subscription rates (~5-8%)
- **Recommendation:** Prioritize cellular contact channels

**Call Duration vs. Subscription:**
![Duration vs Subscription](images/duration_vs_subscription.png)

- **Strong Positive Correlation:** Longer calls significantly increase subscription probability
- **180+ seconds:** >30% subscription rate
- **Insight:** Call quality and engagement crucial for conversion

**Campaign Contacts vs. Subscription:**
![Campaign Contacts vs Subscription](images/campaign_vs_subscription.png)

- **Finding:** 1-3 contacts show highest conversion
- **Finding:** >5 contacts show diminishing returns/negative impact
- **Insight:** Optimal contact frequency exists

**Previous Outcome vs. Subscription:**
![Previous Outcome vs Subscription](images/poutcome_vs_subscription.png)

- **Critical Finding:** Previous success: ~50% subscription rate
- **Previous failure:** ~20% subscription rate
- **Never contacted:** ~5% subscription rate
- **Insight:** Prior campaign success is excellent predictor

#### D. Economic Indicators vs. Subscription

**Employment Rate vs. Subscription:**
![Employment Rate vs Subscription](images/emp_rate_vs_subscription.png)

- Positive correlation: Better employment conditions correlate with higher subscriptions
- Economic conditions influence customer financial confidence

**Interest Rates (Euribor) vs. Subscription:**
![Euribor vs Subscription](images/euribor_vs_subscription.png)

- Inverse correlation: Higher rates correlate with lower subscription rates
- Economic tightening reduces subscription likelihood

**Consumer Confidence vs. Subscription:**
![Consumer Confidence vs Subscription](images/confidence_vs_subscription.png)

- Strong positive correlation: Higher confidence → higher subscriptions
- Economic sentiment critical factor

#### E. Correlation Matrix

![Correlation Matrix](images/correlation_matrix.png)

**Key Correlations with Subscription:**
1. **Duration:** +0.40 (strong positive)
2. **Previous Outcome Success:** +0.35 (strong positive)
3. **Consumer Confidence:** +0.28 (moderate positive)
4. **Month (May, June, July):** +0.25 (moderate positive)
5. **Contact Type (Cellular):** +0.18 (weak positive)
6. **Employment Rate:** +0.15 (weak positive)
7. **Housing/Loan:** -0.12 (weak negative)

