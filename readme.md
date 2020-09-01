# Project 4 - Data visualization

## Prosper Loan Data

The data set consists of information pertaining 113,937 loans, including loan amount, borrower rate, investors and many others. This data set can be found on https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv with detailed explanation of each column on https://www.google.com/url?q=https://docs.google.com/spreadsheet/ccc?key%3D0AllIqIyvWZdadDd5NTlqZ1pBMHlsUjdrOTZHaVBuSlE%26usp%3Dsharing&sa=D&ust=1554484977407000.

## Summary of Findings

Once I read and cleaned data set, I explored the main variables of interest as well as other that I brought into relationship with them. 

The first part of exploratory part was to investigate each variable separately - LoanStatus, Occupation, IncomeRange, BorrowerState, EmploymentStatus (all categorical variables), then BorrowerRate, Investors, and LoanOriginalAmount (all numerical variables).

After that, I wanted to investigate relationship between different variables.
I used the violin graph to see the relationship between BorrowerRate and IncomeRange variables. It seems that the higher the income range the smaller the borrower rate.
I used seaborn countplot to see the relationship between IncomeRange and LoanStatus. The majority of people with current loan fall in between 25k and 75k income range. The highest number of completed loans falls into category of people with income range from 25k to 50k.
Then I showed the relationship between the number of investors and borrower rate. The highest number of investors is for loans with borrower rate between 0.1 and 0.2.
I brought into relationship the amount of loan with income range by using box plot. It seems that the higher the income the bigger the loan amount. Also, I explored the relationship between the amount of loan with the number of investors. Apparently, the highest number of investors is for people who take the loan around 20k.

Then I moved on combining more than 2 variables. 
I performed FacetGrid for BorrowerRate, Investors, and LoanStatus but the graph was not eadily readable. 
Then I performed FacetGrid for BorrowerRate, Investors, LoanStatus, and IncomeRange. The highest number of investors is related to income range between 50k and 75k while the most frequently the borrower rate is 0.2. This part was supported with two addition PairGrid graphs. 
I performed three sountplot where the main findings were that people with the highest number of current loans fall into income range category between 50k and 75k, while completed loans are the highest for people between 25k and 50k income range. The current loans are the highest for people who are employed, while completed loans are the highest for people who are full-time employed. Out of people who are employed there most of them fall into income range category of 50k-70k, while people who are full-time employed have 35k-50k per year.
Finally, FacetGrid showed that the number of investors increases with the loan amount for people who are full-time employed, while for retirees or part-time workers both the number of investors and the amount of loan are lower.

## Key Insights for Presentation

For the presentation, I focused only on the results that show some differences or influence of different factors on loan status or borrower rate. 

Afterwards, I introduced each of the categorical and numerical variables one by one. Then I moved on showing the relationship between different variables (including relationship between 2, 3 oe 4 variables). Also, every graph that shows the relationship or differences is supported with a brief explanation. At the end, I wrote a conclusion based on all the results. 
