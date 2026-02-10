**Credit Dataset Exploratory Data Analysis (EDA)**
 
**Project Overview**
 
This project focuses on exploratory data analysis (EDA) of a credit dataset to understand customer credit behavior, loan characteristics, and repayment patterns. The goal was to clean, explore, and visualize the data before any predictive modeling, while gaining insights that could inform lending decisions.
 
 
**Dataset Description**
 
The dataset contains customer-level credit and loan information used to analyze borrowing behavior and loan performance. The key columns include:
 
	•	Loan ID
 
	•	Customer ID
 
	•	Loan Status (Fully Paid, Charged Off)
 
	•	Current Loan Amount
 
	•	Term (Short-Term, Long-Term)
 
	•	Credit Score
 
	•	Annual Income
 
	•	Years in Current Job
 
	•	Home Ownership
 
	•	Purpose (e.g., Debt Consolidation, Other)
 
	•	Monthly Debt
 
	•	Years of Credit History
 
	•	Months Since Last Delinquent
 
	•	Number of Open Accounts
 
	•	Number of Credit Problems
 
	•	Current Credit Balance
 
	•	Maximum Open Credit
 
	•	Bankruptcies
 
	•	Tax Liens
 
This dataset provides a comprehensive view of customer credit profiles, financial stability, and loan repayment outcomes.
 
 
**Data Cleaning & Preparation**
 
Key preprocessing steps included:
 
	•	Importing the dataset from Google Drive
 
	•	Inspecting data structure, shape, and column data types
 
	•	Checking for and summarizing duplicate records
 
	•	Identifying missing values in key fields such as:
 
	•	Credit score
 
	•	Annual income
 
	•	Years in current job
 
	•	Months since last delinquency
 
	•	Bankruptcy
 
	•	Dropping non-informative identifier columns (Loan ID, Customer ID) since they contained only unique values
 
	•	Removing duplicate records to ensure data quality
 
These steps helped establish a clean and reliable dataset for analysis.
 
 
**Exploratory Data Analysis**
 
The EDA focused on understanding loan behavior and repayment patterns:
 
	•	Loan Purpose Analysis
 
	•	Examined the distribution of loan purposes
 
	•	Observed that debt consolidation was the most common reason for taking loans
 
	•	Compared loan purposes across loan status categories
 
	•	Loan Status by Loan Term
 
	•	Analyzed loan status across short-term and long-term loans
 
	•	Found that short-term loans had a higher proportion of fully paid loans, while long-term loans showed more charge-offs
 
	•	This insight highlights potential risk differences based on loan duration
 
	•	Income Analysis
 
	•	Compared annual income across loan terms
 
	•	Calculated mean and median income values to understand income distribution and stability
 
	•	Home Ownership vs Loan Status
 
	•	Explored loan outcomes based on home ownership categories (Rent, Mortgage, Own)
 
	•	Visualized how ownership status relates to loan repayment behavior
 
	•	Implemented the analysis using multiple approaches to demonstrate flexibility in EDA techniques
 
 
**Key Insights**
 
	•	Debt consolidation is the dominant reason for loan requests
 
	•	Short-term loans tend to perform better than long-term loans
 
	•	Income and home ownership show meaningful relationships with loan outcomes
 
	•	Proper data cleaning significantly improves interpretability and analysis quality
 
 
**Tools & Libraries**
 
	•	Python
 
	•	pandas
 
	•	numpy
 
	•	matplotlib
 
	•	seaborn
 
 
**Conclusion**
 
This project demonstrates a structured approach to data cleaning, exploratory analysis, and visualization, laying a strong foundation for future modeling or credit risk analysis. It reflects practical experience in understanding real-world financial data and extracting actionable insights.
