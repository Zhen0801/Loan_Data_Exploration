# Exploration of Prosper Loan Data
## By Zhen


## Date created
- README file: Aug-08-2019

- Project: July-20-2019

## Dataset

- The original data set (Last updated 03/11/2014) contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others.

- From all those variables, I selected 12 of them that I am most interested in:  ListingNumber, ListingCreationDate, CreditGrade (pre-July 2009), ProsperRatingAlpha (post-July 2009), LoanOriginalAmount, LoanStatus, BorrowerRate, ListingCategory, BorrowerState, Occupation, EmploymentStatus and IncomeRange.


## Files used

- prosperLoanDatacsv   
_*[Loan Data from Prosper](https://www.google.com/url?q=https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv&sa=D&ust=1554486256021000) with [Prosper Data Dictionary](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0) to Explain Dataset's Variables_

- output_toggle.tpl  
_*This file was taken from this [page](http://ww12.oquanta.info), written by one of the contributors to the nbconvert project._



## Summary of Findings

In this project, I went through the dataset in the order of univariate, bivariate and then multivariate Exploration.

My main finding is that before July 2009, actually the borrowing rate is not really as expected : decrease as the loan amount increase. While the credit grade still effects a lot on the borrowing rate. After July 2009, borrower rate significantly decreases as the loan amount increases while rating plays a bigger role in borrower rate that with a high rating can people get a really low borrower rate.

It's quite interesting to see that things do changed with time passing by. It plays a very crucial roles in the relationship between borrower rate, loan amount and credit rating. It is very interesting that nowadays credit rating actually plays a very crucial role in our life. With a high standard credit evaluation system, you can borrow a lot of money with a very low borrowing rate. The original dataset has more than 80 variables, although in this project I mainly focused on how credit rating influence the loan, maybe later we can explore how credit rating is affected by other factors.


## Key Insights for Presentation

For Credit Grade and Borrower State , I used a count plot which can be thought of as a histogram across a categorical or a bar chart.   
Sequential palette was used to make the classification(Credit Grade clearer and a histogram was used for the distribution of Loan Original Amount.    
After calculate the mean of the Borrower Rate, Loan Original Amount and Simplified Loan Status by Credit Grade, I used  count plots to display them all. Afterwards, I chose the box plot to further investigate the relationship between Borrower Rate and Credit Grade.
In the end, Loan Original Amount and Borrower Rate by Credit Grade, two quantitative variables and a categorical
variable, using scatter plots with Sequential palette for the credit grade.


## Credits
The data files and programming instructions are provided by Udactiy's [Data Analyst Nanodegree Program](https://eu.udacity.com/course/data-analyst-nanodegree--nd002). :bowtie:
