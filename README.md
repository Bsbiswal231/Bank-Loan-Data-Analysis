# Bank Loan Report Dashboard (Excel, SQL & Power BI Project).

### Project Overview:

- This project analyzes Bank Loan Data using Excel, SQL, and Power BI to evaluate loan performance, borrower behavior, and portfolio quality. It tracks key KPIs such as total applications, funded amounts, repayments, and interest rates. The interactive dashboards provide insights into good vs. bad loans, regional trends, and borrower demographics, enabling data-driven decisions to improve loan management and reduce financial risk.

### Dataset Used:
<a href="https://github.com/Bsbiswal231/Bank-Loan-Data-Analysis/blob/main/bank_loan.csv"> Bank Loan Data </a>

### Questions (KPIs) / Requirement:

#### KPI Requirements:

##### 1. Total Loan Applications Analysis.
          - Calculate the total number of loan applications.
          - Determine Month-to-Date (MTD) and Month-over-Month (MoM) changes.
          - Identify trends over time to measure loan demand.

##### 2. Total Funded Amount.
          - Calculate the total loan amount disbursed.
          - Analyze MTD and MoM funded amounts.
          - Track growth or decline in loan disbursements.

##### 3. Total Amount Received.
          - Track the total amount received from borrowers (repayments).
          - Measure MTD and MoM changes to assess repayment flow.

##### 4. Average Interest Rate.
          - Compute the average interest rate across all issued loans.
          - Monitor MTD and MoM variations to identify cost trends.

##### 5. Average Debt-to-Income Ratio (DTI).
          - Evaluate borrowers’ financial health through DTI ratio.
          - Analyze monthly changes to understand credit risk levels.

##### 6. Good vs. Bad Loans.
           - Categorize loans as: 
                 - Good Loans → Fully Paid / Current.
                 - Bad Loans → Charged Off.
           - KPIs for each category:
                - % of total loan applications.
                - Total funded amount.
                - Total received amount.

##### 7. Loan Status Grid.
           - Display detailed metrics by loan status: 
                  - Total Applications.
                  - Total Funded Amount.
                  - Total Amount Received.
                  - Avg Interest Rate.
                  - Avg DTI.
                  - MTD metrics.

SQL Queries: <a href="https://github.com/Bsbiswal231/Bank-Loan-Data-Analysis/blob/main/SQL%20Queries.docx"> SQL Queries </a>

### Dashboard Requirements & Visuals:
#### DASHBOARD 1: Summary.
       - Focus: Overall portfolio health and KPI performance.
##### Visuals:
       - KPI Cards: Total Applications, Funded Amount, Amount Received, Avg Interest, Avg DTI.
       - Good vs. Bad Loan breakdown (Donut Chart).
       - Grid view of loan status (Fully Paid, Charged Off, Current).
       - Filters: Loan Type, Grade, Purpose.
##### Insights:
       - Total Loan Applications: 38.6K.
       - Total Funded Amount: $435.8M.
       - Total Amount Received: $473.1M.
       - Avg Interest Rate: 12%.
       - Avg DTI: 13.3%.
       - Good Loans: 86.2%.
       -Bad Loans: 13.8%.
 Dashboard 1: <img width="1435" height="754" alt="Dashboard-1" src="https://github.com/user-attachments/assets/05ebf0e1-c65b-474b-bead-650d711452d8" />

#### DASHBOARD 2: Overview.
       - Focus: Loan trends, borrower demographics, and regional insights.
##### Visuals:
       - Line Chart: Monthly trend of Amount Received (steady growth).
       - Filled Map: Loan distribution by State.
       - Donut Chart: Loan Term Analysis (36-month vs 60-month).
       - Bar Chart: Funded Amount by Employment Length (10+ years highest).
       - Bar Chart: Loan Purpose (Debt Consolidation dominates).
       - Tree Map: Home Ownership (Mortgage largest share).
#### Insights:
       - 60-month loans form 62% of total portfolio.
       - Borrowers with longer employment histories have better repayment consistency.
       - Most loans are taken for Debt Consolidation and Credit Card purposes.
       - Mortgage holders receive the highest funding.
Dashboard 2:<img width="1430" height="754" alt="Dashboard-2" src="https://github.com/user-attachments/assets/857d0d97-9e9a-4266-a15e-fe9520c53d22" />

#### DASHBOARD 3: Details.
       - Focus: Granular, record-level view of all loan transactions.
##### Visuals:
       - Detailed table with Loan ID, Purpose, Grade, Term, Interest Rate, Funded Amount, Amount Received.
       - Filters for State, Grade, Loan Type, and Purpose.
       - Enables easy drill-down and data validation.
Dashboard 3: <img width="1433" height="753" alt="Dashboard-3" src="https://github.com/user-attachments/assets/1e16a02f-d41b-4557-97db-8cf6760f06b3" />

### Process:
#### 1. Data Collection (Excel):
          - Imported raw data into Excel and verified data quality.
          - Understood fields such as Loan ID, Amount, Interest Rate, Term, DTI, and Status.

#### 2. Data Cleaning (Excel & SQL):
          - Removed missing, duplicate, and invalid records.
          - Standardized loan statuses and categorical fields.
          - Ensured proper formatting for dates and numeric values.

#### 3. Data Preparation (SQL):
         - Created calculated fields for:
                - Month, Quarter, and Year from Issue Date.
                - MTD and MoM comparisons.
                - Good vs Bad Loan categorization.
         - Aggregated data using SQL for efficiency before Power BI import.
         
#### 4. Data Modeling (Power BI):
         - Built relationships and data model between loan tables.
         - Developed DAX measures for:
              - Total Applications, Funded Amount, Amount Received.
              - MTD, MoM Growth.
              - Average Interest Rate and DTI.
              - Good vs Bad Loan KPIs.

#### 5. Dashboard Development (Power BI):
         - Designed 3 dashboards (Summary, Overview, Details).
         - Added filters and slicers for dynamic interactivity.
         - Used consistent formatting and color themes for readability.

#### 6. Insights Generation:
         - 86% of loans performing well; only 14% are at risk.
         - Funded and received amounts show strong MoM growth (13–16%).
         - Debt Consolidation is the top loan purpose.
         - Borrowers with long employment and mortgage ownership show higher repayment discipline.

### Final Conclusion:

- The Bank Loan Report efficiently transformed raw loan data into actionable insights using Excel, SQL, and Power BI. It highlights loan performance, repayment trends, and borrower behavior—helping identify risks, optimize funding decisions, and improve overall portfolio management.
