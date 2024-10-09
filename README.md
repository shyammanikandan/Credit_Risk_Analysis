# Credit_Risk_Analysis
Credit Risk Analysis on bank details and credit data
## Objective
To conduct a thorough exploratory data analysis (EDA) and deep analysis of a comprehensive dataset containing basic customer details and extensive credit-related information. The aim is to create new, informative features, calculate a hypothetical credit score, and uncover meaningful patterns, anomalies, and insights within the data.
## Important Links
- [Dataset](https://drive.google.com/file/d/1pljm6_3nxcFS9UMIFm124HBsjNZP6ACA/view?usp=sharing)
- [Data dictionary](https://docs.google.com/spreadsheets/d/1ZuK6o1MXFLmnhkFuDEedasDfVqu9ISPV/edit#gid=688359417)
- [Jupyter Notebooks](https://github.com/shyammanikandan/Credit_Risk_Analysis/tree/main/Jupyter%20Notebook)
- [Project Report](https://github.com/shyammanikandan/Credit_Risk_Analysis/blob/main/Credit%20Risk%20Analysis%20Report.pdf)
## About Data
This dataset is a collection of data used by financial institutions and lenders to evaluate the creditworthiness of individuals or businesses. This dataset provides comprehensive information that helps in assessing the risk of lending to a particular borrower and predicting the likelihood of a loan default or delinquency. Credit risk analysis is a critical aspect of the lending process as it allows institutions to make informed decisions about whether to approve a loan, adjust loan terms, or offer specific financial products.

### Dataset features
| Feature                      | Description |
| -----------                  | ----------- |
| ID	| Represents a unique identification of an entry|
|Customer_ID|	 Represents a unique identification of a person |
|Month|	 Represents the month of the year|
|Name	| Represents the name of a person|
|Age	| Represents the age of the person|
|SSN	| Represents the social security number of a person|
|Occupation	| Represents the occupation of the person|
|Annual_Income	| Represents the annual income of the person|
|Monthly_Inhand_Salary	| Represents the monthly base salary of a person|
|Num_Bank_Accounts	| Represents the number of bank accounts a person holds|
|Num_Credit_Card	| Represents the number of other credit cards held by a person|
|Interest_Rate	| Represents the interest rate on credit card|
|Num_of_Loan	| Represents the number of loans taken from the bank|
|Type_of_Loan	 |Represents the types of loan taken by a person|
|Delay_from_due_date	| Represents the average number of days delayed from the payment date|
|Num_of_Delayed_Payment	| Represents the average number of payments delayed by a person|
|Changed_Credit_Limit|	 Represents the percentage change in credit card limit|
|Num_Credit_Inquiries	 |Represents the number of credit card inquiries|
|Credit_Mix	| Represents the classification of the mix of credits|
|Outstanding_Debt	| Represents the remaining debt to be paid (in USD)|
|Credit_Utilization_Ratio	| Represents the utilization ratio of credit card|
|Credit_History_Age	| Represents the age of credit history of the person|
|Payment_of_Min_Amount	| Represents whether only the minimum amount was paid by the person|
|Total_EMI_per_month	| Represents the monthly EMI payments (in USD)|
|Amount_invested_monthly	| Represents the monthly amount invested by the customer (in USD)|
|Payment_Behaviour	| Represents the payment behavior of the customer (in USD)|
|Monthly_Balance	| Represents the monthly balance amount of the customer (in USD)|
## Data Cleaning

- There are 12500 Customers. Each Customer has data for 8 Months and hence we have data for 100000 rows.
- Few columns have missing values and outliers.
- Mismatch data types, inconsistencies are treated.
- Missing values are treated by mode and mean of the individual customer group.
- Outliers are treated by Inter Quartile Range.

## Concepts

- _Feature Engineering_
  - Created new features that can be leveraged for the calculation of credit scores based on domain knowledge and insights from EDA.
  - Aggregated the data on the customer level when required.
- _Hypothetical Credit Score Calculation_
  - Developed a methodology to calculate a hypothetical credit score using relevant features.
  - Considered features and their weightage
    - Delayed_Payments  - 0.25
    - Credit_Mix - 0.15
    - Credit_History_Age - 0.13
    - Credit_Inquiries - 0.11
    - Annual_Income - 0.1
    - Credit_Utilization_Ratio - 0.08
    - Outstanding_Debt - 0.07
    - Loans - 0.06
    - Credit_Cards - 0.05
- Data Visualization using Matplotlib and Seaborn

## Trends and Insights

- High Annual Income as a Strong Indicator of Creditworthiness.
- Longer Credit History Correlates with Stronger Financial Discipline.
- Minimum Payments Linked to Poor Credit Mix.
- High Credit Utilization as a Red Flag for Default and Financial Stress.
- Credit Inquiries Correlated with Debt and Borrowing Behavior

## Recommendations

- Prioritize High-Earning Customers
- Implement Income-Based Loan Limitations
- Exercise Caution with Customers Lacking Credit History
- Encourage Credit Status Improvement for Low-Risk Borrowers
- Limit Loan Amounts for Average-Risk Customers
