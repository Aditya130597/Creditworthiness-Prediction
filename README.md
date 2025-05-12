# Creditworthiness-Prediction

# About the company
LoanTap is at the forefront of offering tailored financial solutions to millennials.
Their innovative approach focuses on leveraging data science to enhance and refine the credit underwriting process. 
By adopting tech-enabled strategies, LoanTap aims to deliver faster and smarter personal lending experiences.

# Problem statement
This project centers around the Personal Loan segment. Through in-depth analysis of borrower data, the goal is to uncover meaningful patterns in creditworthiness and financial behavior.
These insights will support data-driven decisions in personal loan approvals, helping LoanTap streamline its lending process while mitigating default risk.

# Data set
•	loan_amnt: Amount borrower applied for.

•	term: Loan duration (36 or 60 months).

•	int_rate: Interest rate on loan.

•	installment: Monthly repayment amount.

•	grade: LoanTap assigned loan grade (Risk ratings by LoanTap.)

•	sub_grade: LoanTap assigned loan grade (Risk ratings by LoanTap.)

•	emp_title: Borrower's job title.

•	emp_length: Duration of borrower's employment (0-10 years).

•	home_ownership: Borrower's housing situation (own, rent, etc.).

•	annual_inc: Borrower's yearly income.

•	verification_status: Whether borrower's income was verified.

•	issue_d: Loan issuance month.

•	loan_status: Current status of the loan.

•	purpose: Borrower's reason for the loan.

•	title: The loan's title provided by the borrower.

•	dti (Debt-to-Income ratio): Monthly debt vs. monthly income ratio.

•	earliest_cr_line: Date of borrower's oldest credit account.

•	open_acc: Number of borrower's active credit lines.

•	pub_rec: Negative records on borrower's public credit profile.

•	revol_bal: Total credit balance.

•	revol_util: Usage percentage of 'revolving' accounts like credit cards.

•	total_acc: Total number of borrower's credit lines.

•	initial_list_status: Loan's first category ('W' or 'F').

•	application_type: Individual or joint application.

•	mort_acc: Number of borrower's mortgages.

•	pub_rec_bankruptcies: Bankruptcy records for borrower.

•	Address: Borrower's location.


# Key concepts and objectives
1. Exploratory Data Analysis (EDA):
Checking dataset structure, missing values, and outliers.
Visualization of relationships between features and the target variable (using count plots, box plots, heatmaps).
Checking correlations among independent variables.

2. Feature Engineering:
Creation of flag features: Convert categorical data to binary values for features like pub_rec, mort_acc, and pub_rec_bankruptcies.

3. Missing Value & Outlier Treatment:
Imputation of missing values and handling of outliers.

4. Encoding and Scaling:

	Encoding using LabelEncoder, OneHotEncoder and TargetEncoder.

	Normalization using MinMaxScaler or StandardScaler.

5. Modeling:
Logistic Regression for predicting loan approval.

6. Evaluation of results using: Classification Report, ROC AUC Curve, Precision-Recall Curve

# Trade-off Chanllenges
● Minimizing False Positives: Detecting real defaulters is crucial to avoid non-performing assets (NPAs), ensuring we only disburse loans to creditworthy individuals.

● Precision vs Recall: Optimizing the balance between precision (minimizing false positives) and recall (identifying true positives).

# Results
The model's performance will be evaluated based on:

● Accuracy: Overall accuracy of the model.

● ROC AUC: The area under the ROC curve to evaluate classification performance.

● Precision-Recall Tradeoff: Assessing the balance between precision and recall to minimize financial risk.

# Requirements
● Python 3.x

● Libraries: pandas, numpy, matplotlib, seaborn, category_encoders, scikit-learn, statsmodels

