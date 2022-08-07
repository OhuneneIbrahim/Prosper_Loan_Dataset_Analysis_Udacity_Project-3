# (Prosper Loan Data)
## by (Rabiat Ohunene IBRAHIM)


## Dataset

> The project explore the Prosper loan loan data set. The data set contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others.

### What is prosper loan ?
>For a better understanding of the data set we are working with, lets breifly explain what the prosper loan platform is about.
> Propser loan is an online loaning network involving peer-to-peer lending using the platform prosper.com. This platform allows borrowers to make post listings of loans requests. Interested lenders make their bids on these listings which becomes a loan when the lender invest his/her money by funding the full amount requested by borrower. Some of the informations contains are the time at which the loan originated, the amount requested, the loan status, the credit grade or rating of the borrower, the lender rate and the borrower rate. see http://konect.cc/networks/prosper-loans/ .

> The data set contains 81 features or columns and 113936 of observations or rows. The data types of the features present are bool(3), float64(50), int64(11), object(17). Some of the features contains significant missing values which are due to one of the followings:
>1. The borrower not having prio loans when the listing was made. For example we have features like `TotalProsperLoans`, `TotalProsperPaymentsBilled`, `OnTimeProsperPayments`,`ProsperPaymentsLessThanOneMonthLate`, `ProsperPaymentsOneMonthPlusLate`,`ProsperPrincipalBorrowed`,`ProsperPrincipalOutstanding`,`ScorexChangeAtTimeOfListing`. 

>2. Features that are only applicable after July 2009. For example, `EstimatedEffectiveYield`, `EstimatedLoss`, `EstimatedReturn`, `ProsperRating (numeric)`, `ProsperRating (Alpha)`, `ProsperScore`.

> From the 81 features of the dataset we had selected 30 for wrangling and analysis. Some of the cleaning carried out was
(a) Convert `ListingCategory (numeric)` to string datatype (b) Covert `ProsperScore` to cathegorical data type, (c) Convert observation: `Not employed` to income range of 0 in the income variable (d) Convert the income range variable to cathegorical data.


## Summary of Findings

> The feature of interest for the analysis was the `BorrowerAPI` and the `Loanstatus`. The goal was to investigate which of the features affects the borrower's APR and the outcome of the loan. 

> The featues in the dataset I think will support my chosen features of interest are `IncomeRange`, `BorrowerAPR`, `DebtToIncomeRatio`, `ProsperScore`, `CreditScoreRangeLower` and `CreditScoreRangeUpper`. 

>Some of our findings were:

> Our analysis shows are moderate negative correlation between a BorrowerAPR and his credit score. However, there seem to be a weak correlation with the BorrowerAPR and the debt to income ratio. 

> We also observe good connection between the BorrowerAPR and the loanstatus. We saw that people who did not default in their loan servicing are more likely to have a lower BorrowerAPR.

> The prosper score showed a strong variation with the Borrower APR as well as the Loanstatus. We saw that people with higher prosper score appear to have lower borrowerAPR. The people with higher prosper score seem to be more likely not to default in their loan payment.

>The income range is another feature that appeared to influence the Borrower APR and the loan status. We saw that higher income range are associated with lower BorrowerAPR and less default loan payment.

>We also observed that having a high prosper score and credit score will drastically reduce the borrower's APR.

> These are the major findings from the analysis which I plan to discuss in the explanatory presentation


## Key Insights for Presentation

>  The prosper score has strong variation with the Borrower APR and the Loanstatus. We saw that people with higher prosper score have lower borrowerAPR. The people with higher prosper score are more likely not to default in their loan payment.

>We also observed that having a high prosper score and credit score will drastically reduce the borrower's APR
