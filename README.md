# Bank Loan Portfolio Analysis

End-to-end analysis of a bank's loan portfolio (2007-2011) using **Power Query, MySQL, Excel, Power BI and Tableau**.

## Project Overview
This project analyses a loan portfolio of **39,717 loans worth ₹446M**, issued between 2007 and 2011. It looks at loan growth, borrower grades, verification status, home ownership, state-wise loans and repayment performance. Two finance datasets were merged and then analysed with SQL and three dashboard tools.

**Data:** `Finance_1` and `Finance_2`, merged into one table (`MERGE_FINANCE_TABLES`).

## Key Metrics
| Total Loans | Total Loan Amount | Total Last Payment | Avg Interest Rate | Good Loans | Bad Loans |
|---|---|---|---|---|---|
| 39,717 | 446M | 106M | 12.02% | 85.83% | 14.17% |

Power BI also shows total payment of 482.70M, made up of 388.96M principal recovered and 89.91M interest received.

## Tools Used
| Tool | What was done |
|---|---|
| Power Query | Combined the two finance datasets into one |
| MySQL | Wrote queries for year-wise loans, grade and sub grade balances, verification status, state-wise loan status and home ownership, including a stored procedure |
| Excel | Pivot tables, charts, KPI cards and slicers (year, grade, verification status, home ownership) |
| Power BI | Dashboard with KPI cards, 6 charts, a state map and slicers |
| Tableau | Dashboard with KPI tiles, 5 charts, a state-wise top 10 and filters |

## Dashboards
# Excel Dashboard
![Excel Dashboard](Presentation/Excel_Dashboard(BA).png)

# Power BI Dashboard
![Power BI Dashboard](Presentation/PowerBI_Dashboard(BA).png)

# Tableau Dashboard
![Tableau Dashboard](Presentation/Tableau_Dashboard(BA).png)

Each dashboard covers year-wise loan amount, grade and sub grade revolving balance, verified vs not verified, state-wise loan status, and home ownership vs payments.

All three dashboards are in the project presentation: [View the full project presentation (PDF)](presentation/Bank Analysis.pdf)

## SQL Queries
| Query | Purpose |
|---|---|
| Q1 | Year-wise total loans, total, average, minimum and maximum loan amount |
| Q2 | Grade and sub grade wise revolving balance |
| Q3 | Verified vs not verified total payment (stored procedure) |
| Q4 | State-wise and last credit pull date wise loan status (fully paid, charged off, current) |
| Q5 | Home ownership vs last payment date, total loans and total last payment |

SQL concepts used: GROUP BY, aggregate functions, date functions (`STR_TO_DATE`, `YEAR`), conditional counting, `TRIM`, stored procedures.

## Key Insights
1. **Loans grew every year:** from 2M in 2007 to about 261M in 2011. 2011 alone is roughly 58% of the total loan amount.
2. **Healthy repayment:** 85.83% of loans are good (fully paid or current) and 14.17% are bad (charged off). Of 39,717 loans, 32,950 are fully paid, 1,140 are current and 5,627 are charged off.
3. **Grade B carries the highest revolving balance** (about 160M), followed by grades A and C. Risky grades E, F and G have much smaller balances.
4. **Verified loans lead payments:** verified loans account for about 45.5% of total payment, not verified 31.8% and source verified 22.6%.
5. **Home ownership:** borrowers with a mortgage (56M) and renters (42M) make most of the last payments, while owners contribute about 8M.
6. **State-wise:** California has the most loans, followed by NY, FL, TX and NJ.

## Repository Structure
```
Bank_loan_analysis/
├── data/           Finance_1 and Finance_2 datasets
├── images/         dashboard screenshots
├── presentation/   final project presentation (PDF)
├── sql/            SQL queries
└── README.md
```

## Project Team (DA - P1435)
- Posibabu
- Jagadeesh
- Bhaskar Sai Charan
- Srushti Vikas Sakhare
- Soniya
- Vandana
- Lakshmi Mithra

## Author
**Menni Posibabu**, 
Aspiring Data Analyst | Excel, MySQL, Power BI, Tableau
LinkedIn: (www.linkedin.com/in/posibabumenni)
GitHub: [posi19babu](http://github.com/posi19babu)
email: posibabu414@gmail.com
