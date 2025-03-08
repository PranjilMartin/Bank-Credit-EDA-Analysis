# Bank-Credit-EDA-Analysis

Should you get the loan? Will you pay the loan on time?

## 🗒️ **Business Understanding**


The loan providing companies find it hard to give loans to the people due to their insufficient or non-existent credit history. Because of that, some consumers use it to their advantage by becoming a defaulter. Suppose you work for a consumer finance company which specialises in lending various types of loans to urban customers. You have to use EDA to analyse the patterns present in the data. This will ensure that the applicants capable of repaying the loan are not rejected.

When the company receives a loan application, the company has to decide for loan approval based on the applicant’s profile. Two types of risks are associated with the bank’s decision:

If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company

If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the company.

The data given below contains the information about the loan application at the time of applying for the loan. It contains two types of scenarios:

The client with payment difficulties: he/she had late payment more than X days on at least one of the first Y instalments of the loan in our sample,

**All other cases:** All other cases when the payment is paid on time.

When a client applies for a loan, there are four types of decisions that could be taken by the client/company):

 - **Approved:** The Company has approved loan Application

 - **Cancelled:** The client cancelled the application sometime during approval. Either the client changed her/his mind about the loan or in some cases due to a higher risk of the client, he received worse pricing which he did not want.

 - **Refused:** The company had rejected the loan (because the client does not meet their requirements etc.).

 - **Unused offer:** Loan has been cancelled by the client but at different stages of the process.

In this case study, you will use EDA to understand how consumer attributes and loan attributes influence the tendency to default.

## 🎯 **Business Objectives**


This case study aims to identify patterns which indicate if a client has difficulty paying their instalments which may be used for taking actions such as denying the loan, reducing the amount of loan, lending (to risky applicants) at a higher interest rate, etc. This will ensure that the consumers capable of repaying the loan are not rejected. Identification of such applicants using EDA is the aim of this case study.

In other words, the company wants to understand the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default. The company can utilise this knowledge for its portfolio and risk assessment.

To develop your understanding of the domain, you are advised to independently research a little about risk analytics - understanding the types of variables and their significance should be enough.



## ⏳ **DataSet** 

This dataset has 3 files as explained below: 


1. 'application_data.csv'  contains all the information of the client at the time of application.
    The data is about whether **a client has payment difficulties**.

2. 'previous_application.csv' contains information about the client’s previous loan data. It contains the data on whether the previous application had been **Approved, Cancelled, Refused or Unused offer**

3. 'columns_description.csv' is data dictionary which describes the meaning of the variables.

## 💻 **Technologies Used**

 - Python - version 3.12.4
 - Matplotlib - version 3.10.0
 - Numpy - version 1.26.4
 - Pandas - version 2.2.3
 - Seaborn - version 0.13.2

## 📃**Approach**

 - Step 1: Import Necessary Libraries
 - Step 2: Load the Data and Understanding the Data
 - Step 3: Data Cleaning and Missing Value Check
 - Step 4: Segmentation of Columns
 - Step 5: Exploratory Data Analysis (EDA) -- Univariate Analysis (One Variable at a Time) -- Bivariate Analysis (Two Variables at a Time) -- Multivariate Analysis (More Than Two Variables at a Time)
 - Step 6: Conclusion

## 💡 **Conclusion**

**Analysing the whole dataset we can consider the follwing thing that would help bank to provide the loan who can repay the or not**

**Successful applicant will be Repayer:**


AGE : - Loan applicants above the age of 60 has a lower tendency to default.
NAME_INCOME_TYPE :- Student and Businessmen have no defaults.
AMT_INCOME_TOTAL :- Applicants with incomes exceeding 10 Millions experience a lower likelihood of default.
NAME_HOUSING_TYPE :- Applicant leaving in there own house, or parents , or rental apartment are lower likelihood of default
CNT_CHILDREN:- People with zero to two children tend to repay the loans.


**Applicant will be Defaulter:**


NAME_EDUCATION_TYPE: People with Lower Secondary & Secondary education has higher defaulter
CNT_CHILDREN: Client who have children equal to or more than 9 default 100% and hence their applications are to be rejected.
CODE_GENDER: Men are at relatively higher default rate
NAME_FAMILY_STATUS : People who have civil marriage or who are single default a lot.
OCCUPATION_TYPE: Avoid Low-skill Laborers, Drivers and Waiters staff, Security staff, Laborers and Cooking staff has the higher default rate .
DAYS_BIRTH: Avoid young people who are in age group of 20-30 as they have higher probability of defaulting
AMT_GOODS_PRICE: When the credit amount goes beyond 3M, there is an increase in defaulters.


