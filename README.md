# EduTechTainMent_Udacity_Data_Analyst_ND_Project_Prosper_Loan_Data_Exploration
## Udacity Project 3 exploring Prosper Loan Dataset


# Prosper Loan Dataset Exploration

## by Abdulwasiu Bamidele Popoola

## Prosper Loan Dataset

> This data set contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others.

> This data [dictionary](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit) explains the variables in the data set.

The dataset can be downloaded from this [LINK](https://www.google.com/url?q=https://www.google.com/url?q%3Dhttps://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv%26amp;sa%3DD%26amp;ust%3D1581581520570000&sa=D&source=editors&ust=1657791099475595&usg=AOvVaw0-TOnL_-tvEMcT7qa-sRiO).

This exploration is in no way exhaustive or completed. This is a work in progress. However for the purpose of this submission, I shall be focusing on some of the features in the dataset.

Since we wouldn't be using or analyzing all the variables, we created a subset of the main dataset we shall be working on, using the loc method. This subset is named `loans`. Going forward, we shall run our analysis on the `loans` DataFrame. To achieve this, first I identified and created a list of all the columns (called column_list) i used in this exploration.

My main feature of interest is the `BorrowerStatus`. Other features that would help me in my exploration include: `Term`, `BorrowerAPR`, `BorrowerRate`, `rosperRating (Alpha)`, `ProsperScore`, `ListingCategory (numeric)`, `Occupation`, `EmploymentStatus`, `EmploymentStatusDuration`, `IsBorrowerHomeowner`, `CreditScoreRangeLower`, `CreditScoreRangeUpper`, `CurrentCreditLines`, `OpenCreditLines`, `IncomeVerifiable`, `TotalProsperLoans`, `Recommendations`, etc.

## Summary of Findings

Some observations I made from this exploration, which is far from being complete include the following:

However, some conclusions I could make from this exploration include the following.

A borrowers `LoanStatus` is affected by the `BorrowerAPR`, `BorrowerRate`, `EmploymentStatusDuration` etc.

There is a positve correlation between the `BorrowerAPR` and `BorrowerRate`.

The borrowers with `Current` loan status had longer `EmploymentStatusDuration`. Those who defaulted or past due dates had relatively smaller `EmploymentStatusDuration`.

Borrowers with `Current` or `Completed` loan status have relatively lower `BorrowerRate` while those who defaulted or were past due dates had higher `BorrowerRate`.

The `BorrowerRate` was highest amongst those who have `Defaulted` `LoanStatus`.

Most loans were for a `Term` of 36 months.

## Key Insights for Presentation

I will showcase how some select features affect the `LoanStatus` of the borrowers. I had to set the order of charting for the nominal categorical variables but not for the ordinal variables. For some featurs, I also had to set the bin sizes (in some cases by using numpy arange function) in order to get a better view of the distribution of the variables. I also had to select some features from the entire dataset to narrow down my exploration on them. I chose to visualize the distribution usin different chart types that are apprppriate for the either univariate, bivariate or multivariate features.

The datatypes of some features was also changed to the appropriate datatype to enable proper exploration and visualization with the appropriate charts.

For some features with too many values, I focused on visualizing the top and bottom part ( a sample) of the observations. User defined functions were used to plot repeated visualizations.


For a detailed view of all the exploratory process, please refer to the files below:

1. [Part_II_slide_decks.slides HTML](https://github.com/Waga43/EduTechTainMent_Udacity_Data_Analyst_ND_Project_Prosper_Loan_Data_Exploration/blob/main/Part_II_slide_decks.slides.html)

2. [Part_II_slide_decks Jupyter Notebook](https://github.com/Waga43/EduTechTainMent_Udacity_Data_Analyst_ND_Project_Prosper_Loan_Data_Exploration/blob/main/Part_II_slide_decks.ipynb)

3. [Part_I_exploration HTML](https://github.com/Waga43/EduTechTainMent_Udacity_Data_Analyst_ND_Project_Prosper_Loan_Data_Exploration/blob/main/Part_I_exploration.html)

4. [Part_I_exploration Jupyter Notebook](https://github.com/Waga43/EduTechTainMent_Udacity_Data_Analyst_ND_Project_Prosper_Loan_Data_Exploration/blob/main/Part_I_exploration.ipynb)
