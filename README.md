# (Prosper Loan Data)
## by (Neepam Goel)


## Dataset

> The Prosper loan dataset comprises of 113937 loan entries with 81 attributes on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others, from the year 2009-2014. There are two main categories:
  
    - Borrower information: Basic attributes of the borrowers such as annual income, condition of employment, interest rate, loan status, etc.
    
    - Loan performance information: Metrics evaluating the risk associated with the loans such as -Prosper score and bank card utilization, etc. There were some elements that need to be fixed, in order to create interesting and trustworthy analyses and visualizations.

>
> Features of interest:
      - **LoanStatus** - The current status of the loan: Cancelled, Chargedoff, Completed, Current, Defaulted, FinalPaymentInProgress, PastDue. The PastDue status will be accompanied by a delinquency bucket.
     - **BorrowerAPR** - The Borrower's Annual Percentage Rate (APR) for the loan.

## Summary of Findings

### Data Cleaning

> To clean our dataset-

    - We made a subset of required features
    - Filtered rows which has no null values of Prosper Score since it is the most important feature to be studied
    - Filled remaining null values with median as data might have outliers.
    - Filled not given occupations with 'Unknown'as it is a categorical variable


### Data Exploration

> Loan Status

    - Most of the Loans taken(around 80%) can be labelled as good(Current/Completed)
    - Most number of customers(around 7500) have been charged around 36% APR rate.Very less borrowers have been charged more than 40% or 0.4 APR
    - The company prefers to give loans to people on an average amount of prosper score rating(4 to 8) rather than very low ones or high ones who might not need it in the first place.
    - Higher prosper scores generally relate to the Loan being current(on schedule) or Completed. So the lower the prosper score, more is the probability of having a bad loan status
    - Higher credit score average relate borrowers to being in the good loan status(current,completed, final payment in progress) while being in the deliquient status(Defaulted, Due) when having a lower credit score.
>
> APR rate
    
    - 63% of borrowers have credit score average between 670 to 730
    - People who are unemployed/no salary are given the highest APR rate while it decreases as the income increases.
    - Higher Prosper rating means lower APR rate
    - APR rate is inversely proportional to credit score
    -  If a person is a home owner he can expect to recieve lower APR rate.
    - when prosper score is high(7-11), borrower apr rate is directly proportional to loan term
    - when prosper score is medium(4-7), borrower apr rate is inversely proportional to loan term
    - when prosper score is low(1-4), borrower apr rate is equivalent to loan term
 


## Key Insights for Presentation

> Key insights we want to highlight in our presentation are-

    - How higher prosper score relates to a good loan status.
    - How higher credit score and prosper rating relates to a lower APR rate.
    - How being a homeowner affects the APR rate.
