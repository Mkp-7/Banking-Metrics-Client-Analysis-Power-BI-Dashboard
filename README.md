# Banking Metrics & Client Analysis Power BI Dashboard

![Dashboard Preview](Images/Dashboard_Overview.png)

## Project Overview
The **Banking Metrics & Client Analysis Power BI Dashboard** provides actionable insights into client portfolios, banking relationships, and financial performance.  

This dashboard demonstrates strong skills in **data modeling, DAX calculations, and visualization**. It allows analysts and decision-makers to:
- Explore key banking metrics
- Understand client demographics
- Monitor financial trends efficiently

---

## Data Description

The dashboard integrates **four primary tables**:

### 1. Banking Relationship
Captures core banking relationships between clients and their banking services.  
- **Columns**:  
  - `BRID`: Banking Relationship ID  
  - `Banking Relationship`: Type of banking relationship  

### 2. Clients - Banking
Contains detailed client and banking contract information.  
- **Columns**:  
  - `Banking Contracts`: Details of banking contracts  
  - `BRID`: Banking Relationship ID (Foreign Key)  
  - `ClientID`: Unique client identifier  
  - `Fee Structure`: Banking fee structure  
  - `GenderID`: Gender identifier (Foreign Key)  
  - `IAID`: Investment Advisor ID (Foreign Key)  
  - `Name`: Client’s name  
  - `Nationality`: Client’s nationality  
  - `Occupation`: Client’s occupation  

### 3. Gender
Provides gender details of clients.  
- **Columns**:  
  - `GenderID`: Unique identifier  
  - `Gender`: Gender description  

### 4. Investment Advisor
Contains information about investment advisors.  
- **Columns**:  
  - `IAID`: Unique identifier  
  - `Investment Advisor`: Name of the advisor  

---

## Key Metrics and DAX Calculations

The dashboard uses **DAX formulas** to calculate essential financial metrics:

| Metric | DAX Formula |
|--------|-------------|
| Savings Account Amount | `SavingAccountAmount = SUM('Clients - Banking'[Savings Accounts])` |
| Total Credit Card Amount | `TotalCCAmount = SUM('Clients - Banking'[Credit Card Balance])` |
| Total Bank Deposits | `TotalDeposit = SUM('Clients - Banking'[Bank Deposits])` |
| Total Loans | `TotalLoan = SUM('Clients - Banking'[Bank Loans])` |
| Total Business Lending | `TotalBusinessLending = SUM('Clients - Banking'[Business Lending])` |
| Total Checking Accounts | `TotalCheckingAccounts = SUM('Clients - Banking'[Checking Accounts])` |
| Total Estimated Income | `TotalEstimatedIncome = SUM('Clients - Banking'[Estimated Income])` |
| Total Foreign Currency Account | `TotalForeignCurrencyAccount = SUM('Clients - Banking'[Foreign Currency Account])` |
| Total Superannuation Savings | `TotalSuperannuationSavings = SUM('Clients - Banking'[Superannuation Savings])` |

These metrics provide **insights into financial accounts, client wealth distribution, and banking performance**.

---

## Dashboard Features
- **Interactive filtering** by client demographics, banking relationships, and financial metrics  
- **Dynamic visualizations** including bar charts, line charts, pie charts, and tables  
- **Insights delivered**:  
  - Banking relationship trends  
  - Client portfolio summaries  
  - Investment advisor performance  
  - Financial distribution across products  

---

## Usage Instructions
1. Open the Power BI file: `Banking_Analysis_Dashboard.pbix`  
2. Load the dataset: `Banking_Data.xlsx`  
3. Explore dashboard visuals using slicers and filters  
4. Analyze key metrics and trends for banking decision-making  

---

## Files in this Repository
- `Banking_Analysis_Dashboard.pbix`: Power BI dashboard file  
- `Banking_Data.xlsx`: Dataset with all tables  
- `Images/`: Folder containing screenshots of the dashboard  
  - `Dashboard_Overview.png`  
  - `Client_Demographics.png`  
  - `Financial_Metrics.png`  
- `README.md`: This file  

---

## Conclusion
This dashboard is a **powerful tool for data-driven banking insights**, combining **data modeling, DAX analytics, and visualization best practices**.  

It demonstrates the ability to:
- Analyze complex datasets  
- Generate actionable insights  
- Support strategic decision-making  
