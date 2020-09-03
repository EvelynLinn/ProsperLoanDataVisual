# Prosper Loan Data Exploration

## Dataset
This data set contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others. The dataset can be found [here](https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv).


## Summary of Findings 
I focused on the impact from borrowers' financial situations and loans' characteristics on interest rates, by looking into the impact of borrowers' personal situations on the existing correlations between rates and loan types and statuses. The indicators of financial status include: `IsBorrowerHomeowner`, `DebtToIncomeRatio`, `IncomeRange` or `StatedMonthlyIncome`, and `AvailableBankcardCredit`.

On the other hand, as ProsperScore seems to be the strongest indicator, due to the fact that it's not a direct indicator, I tried linking its underlying variables directly to interest rates, including `DebtToIncomeRatio` and `TotalInquiries`. 


## Key Insights for Presentation 
- Within each income range group, the rate increases as amount of terms increases; overall, for the same amount of terms, people with higher income are able to be granted lower interest rate. 
- For each loan status, overall interest rates slightly decrease as income ranges increase. But once a loan is defaulted or charged off, the interest rates can expect to maintain a same level as past due, instead of keeping growing.
- The amount of available bankcard credits show a negative correlation to interest rates. In fact, low bank card creadit can be a barrier to have lowest interest rates. 
- Higher income doesn't necessarily mean lower interest rate, but in the range of below 0.10 of interest rate, most borrowers are with higher income.
