# Finance Bank Loan Report [PBI]
## Introduction
### 1. About
- In order to monitor and assess our bank's lending activities and performance, Bank Loan Report provide insights into key loan-related metrics and their changes over time. The report will help manager make data-driven decisions, track loan portfolio's health, and identify trends that can inform lending strategies
### 2. Reasons for Analysing Bank Loan Data
Banks analyse loan data for several critical reasons:
- **Risk Assessment**: One of the primary purposes of analysing loan data is to assess the risk associated with lending to a particular individual or business. Banks use data to evaluate the creditworthiness of borrowers, predict default probabilities, and determine interest rates and lending terms.
- **Decision-making**: Loan data analysis supports the decision-making process when evaluating loan applications. Banks use data-driven models and algorithms to make informed lending decisions, such as approving or denying loan requests.
- **Portfolio Management**: Banks manage portfolios of loans, including mortgages, personal loans, and business loans. Data analysis helps banks monitor the health of these portfolios, identify underperforming loans, and optimize loan terms and pricing.
- **Fraud Detection**: Banks use data analysis to detect fraudulent loan applications and activities. Unusual patterns, inconsistencies, or discrepancies in loan data can trigger fraud alerts.
- **Regulatory Compliance**: Banks are subject to regulatory requirements that mandate the collection and reporting of loan data. Compliance with regulations such as the Home Mortgage Disclosure Act (HMDA) and the Know Your Customer (KYC) regulations requires data analysis and reporting.
- **Customer Insights**: Analysing loan data provides insights into customer behaviour, preferences, and needs. Banks can use these insights to tailor loan products and marketing strategies to specific customer segments.
- **Profitability Analysis**: Banks assess the profitability of their loan portfolios by analysing data related to interest income, loan origination costs, default rates, and collection efforts.
- **Market Research**: Data analysis helps banks understand market trends, competitive landscape, and customer demand. This information guides product development and market expansion strategies.
- **Credit Risk Management**: Banks continuously monitor and manage credit risk associated with their loans. Data analysis helps in setting risk management strategies, provisioning for potential losses, and stress testing loan portfolios.
- **Customer Retention**: Banks use data analysis to identify opportunities for retaining existing customers, such as offering loan refinancing options or additional financial products
### 3. Dataset
- A dataset containing information about a bank's loans
- Fields in the dataset: <br/>
  - **Loan ID:** Loan ID is a unique identifier assigned to each loan application or loan account. It serves as a primary key for tracking and managing individual loans. <br/>
  - **Address State:** Address State indicates the borrower's location. It helps in assessing regional risk factors, compliance with state regulations, and estimating default probabilities. <br/>
  - **Employee Length:** Employee Length provides insights into the borrower's employment stability. Longer employment durations may indicate greater job security.<br/>
  - **Employee Title:** Employee Title specifies the borrower's occupation or job title. It helps lenders understand the source of the borrower's income.<br/>
  - **Grade:** Grade represents a risk classification assigned to the loan based on creditworthiness. Higher grades signify lower risk.<br/>
  - **Sub Grade:** Sub Grade refines the risk assessment within a grade, providing additional risk differentiation.<br/>
  - **Home Ownership:** Home Ownership indicates the borrower's housing status. It offers insights into financial stability.<br/>
  - **Issue Date:** Issue Date marks the loan's origination date. It's crucial for loan tracking and maturity calculations.<br/>
  - **Last Credit Pull Date:** Last Credit Pull Date records when the borrower's credit report was last accessed. It helps monitor creditworthiness.<br/>
  - **Last Payment Date:** Last Payment Date marks the most recent loan payment received. It tracks the borrower's payment history.<br/>
  - **Loan Status:** Loan Status indicates the current state of the loan (e.g., fully paid, current, default). It tracks loan performance.<br/>
  - **Next Payment Date:** Next Payment Date estimates the date of the next loan payment. It assists in cash flow forecasting.<br/>
  - **Purpose:** Purpose specifies the reason for the loan (e.g., debt consolidation, education). It helps understand borrower intentions.<br/>
  - **Term:** Term defines the duration of the loan in months. It sets the repayment period.<br/>
  - **Verification Status:** Verification Status indicates whether the borrower's financial information has been verified. It assesses data accuracy.<br/>
  - **Annual Income:** Annual Income reflects the borrower's total yearly earnings. It assesses repayment capacity.<br/>
  - **DTI (Debt-to-Income Ratio):** DTI measures the borrower's debt burden relative to income. It gauges the borrower's capacity to take on additional debt.<br/>
  - **Instalment:** Instalment is the fixed monthly payment amount for loan repayment, including principal and interest.<br/>
  - **Interest Rate:** Interest Rate represents the annual cost of borrowing expressed as a percentage. It determines the loan's cost.<br/>
  - **Loan Amount:** Loan Amount is the total borrowed sum. It defines the principal amount.<br/>
## Analysis & Visualization
1. Summary Page
![summary](https://github.com/user-attachments/assets/cd615676-80e7-4ac2-9592-d020238c2fd1) <br />
- Total Loan Applications:
  - 38.6K loan applications processed.
  - The number of loan applications increased by 6.9% compared to the previous month (MoM), which shows that the demand for loans is increasing.
  - The number of loan applications in the current month (MTD) is 4.3K, which may continue to increase by the end of the month
- Good vs Bad Loans:
  - 86.2% of the loans were considered Good Loans (about 33.2K applications), showing a low NPL ratio of only 13.8% (about 5.3K applications were Bad Loans).
  - The total amount received from Good Loans was $435.8M, while the total amount received from Bad Loans was $37.3M
- Average Interest Rate:
  - Average interest rate is 12.05%, a slight increase of 3.5% compared to last month
  - This may be due to changes in banking policy or financial market conditions, but is still within acceptable levels for personal or small business loans
- Average DTI - Debt-to-Income Ratio:
  - The average DTI ratio is 13.33%, indicating that most borrowers have debt levels that are not too high compared to their income, a sign that the risk of bad debt is still under control.
- Loan Applications by Purpose:
  - The most popular loan purpose is Debt consolidation with 18K applications, indicating that many borrowers are looking to manage existing debt
  - Other purposes such as Credit card (5K), Home improvement (3K), and Small business (2K) are also notable
- Loan Applications by Term:
  - The majority of loans have a term of 60 months (73.2%) compared to 36 months (26.8%), indicating that borrowers tend to choose longer terms, possibly to reduce the pressure of monthly interest payments
2. Overview Page
![detail](https://github.com/user-attachments/assets/ba2aaef6-3f9f-4440-89bb-c58ed3a2c1bf) <br />
- Loan Applications by Month:
  - The number of loan applications increased gradually over the months of the year. From January with 2.3K applications, to December with 4.3K, showing a steady increase in loan demand
- Loan Applications by Employee Length:
  - The group with 10+ years of work experience accounted for 8.9K loan applications, the most of all groups, showing that people with stable jobs tend to borrow more.
  - The group with less than 1 year of work experience accounted for 4.6K loan applications, showing that even people who have just started working have a need for loans, possibly to pay off debts or cover living expenses.
- Analysis by Home Ownership:
  - Renters accounted for the majority of loan applications (18.4K compared to 17.2K of mortgage holders). This may indicate that renters tend to need to borrow to manage living expenses or debt, while homeowners may borrow to pay off debt or borrow to buy a home.
3. Detail Page
![overview](https://github.com/user-attachments/assets/4d78ddca-b7af-4faa-88ce-2a3cefef745f) <br />
