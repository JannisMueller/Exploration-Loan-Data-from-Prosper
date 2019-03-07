---
jupyter:
  jupytext:
    text_representation:
      extension: .md
      format_name: markdown
      format_version: '1.0'
      jupytext_version: 0.8.6
  kernelspec:
    display_name: Python 3
    language: python
    name: python3
---

# Exploration of Loan Data from Prosper 
## by Jannis Müller


## Dataset

This data set contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others


## Summary of Findings

The huge dataset with a lot of informaton (81 variables) allowed me to have deeper look at the question what factors affect a loan’s outcome status (Cancelled, Chargedoff, Completed, Current, Defaulted, FinalPaymentInProgress, PastDue)

This is a very critical question for banks and loan companies in order to minimize the default risk and and to set the right interest rate (including setting a proper risk premium).
This investigation might help to find out what factors predict the outcome of a loan best.

Throughout the investigation I focused on the the following factors that might have the most influence on predicting the outcome of a loan and therefore are of most interest to me:
 - Term (The length of the loan expressed in months)
 - ProsperScore (custom risk score)
 - EmploymentStatus (The employment status of the borrower)
 - MonthlyLoanPayment (The scheduled monthly loan payment)
 - IncomeRange (The income range of the borrower at the time the listing was created)
 - BorrowerRate (The Borrower's interest rate for this loan)
 - LoanOriginalAmount (The origination amount of the loan)
 - OpenCreditLines (Number of open credit line)
 - TotalProsperPaymentsBilled (number of on time payments the borrower made on Prosper loans at the time they created this listing)
 - Recommendations (Number of recommendations the borrower had at the time the listing was created)

#### In summary, I could find the following observations in the dataset:

- relationship between the monthly payments and the negative outcome of the loan for Prosper: loans that are charged-   off, loans with past due payments and defaulted loans have in average higher monthly payments
- loans that are charged-off, loans with past due payments and defaulted loans have in average higher interest rates   than loans that are completed
- the highest interest rates are asscociated with loans that are charged-off and with loans that have past due payments
- original loan amount does not have an impact with the final status of the loan: the original loan amount is about the same in average for loans that are completed, charged-off or defaulted. However, loans with past due payments have in average an higher orginal loan amount
- The Prosper Score seem to affect the outcome of the loan: so have the most borrower an Prosper Score of 8 when a loan is completed, while most borrower with defaulted and charged-off loans have an Prosper Score of 6.  Furthermore, the most comon Prosper Score for borrowers with loans that have past due payments is 4.
- the higher the Prosper Score, the lower the interest rate, the lower the risk for Prosper that the loan will be defaulted, charged-off or has past due payments. So, borrower with a low Prosper Score get a lower interest rate due to the lower risk that the loan will be defaulted

In my presentation I will focus on the relationships I found and which are mentioned above



## Key Insights for Presentation

The exploration of the data showed that monthly payments and higher interest rate affect the risk that loans are defaulted, charged-off or have that loans have past due payments: the higher the payments or the interest rate, the higher is the risks of an negative outcome of the loan. This make sense since borrower with higher risks usually get higher interest rates (risk premium)

The Prosper Score seem also to affect the outcome of the loan: so have the most borrower an Prosper Score of 8 when a loan is completed, while most borrower with defaulted and charged-off loans have an Prosper Score of 6.  Furthermore, the most comon Prosper Score for borrowers with loans that have past due payments is 4. This shows that the Prosper Score seems to be a valid tool to set the risk premium (interest rate) or to evaluate if a borrower should get a loan or not. 

I could further detect the following relationsship between Loan status, Prosper Score and interest rate: the higher the Prosper Score, the lower the interest rate, the lower the risk for Prosper that the loan will be defaulted, charged-off or has past due payments. So, borrower with a higher Prosper Score get a lower interest rate due to the lower risk that the loan will be defaulted.



```python

```
