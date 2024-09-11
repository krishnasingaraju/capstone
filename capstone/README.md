
## LendingClub Data Set Information:

Complete loan data for all loans issued through the 2007-2015, including status


#### Business Understanding

Lending Club is a peer-to-peer Lending company based in the US. They match people looking to invest money with people looking to borrow money. When investors invest their money through Lending Club, this money is passed onto borrowers, and when borrowers pay their loans back, the capital plus the interest passes on back to the investors. It is a win for everybody as they can get typically lower loan rates and higher investor returns.

The Lending Club dataset contains complete loan data for all loans issued through the 2007-2015, including the current loan status (Current, Late, Fully Paid, etc.) and latest payment information. Features (aka variables) include credit scores, number of finance inquiries, address including zip codes and state, and collections among others. Collections indicates whether the customer has missed one or more payments and the team is trying to recover their money. The file is a matrix of about 890 thousand observations and 75 variables. Quick Look at the dataset shows that it is highly imbalanced and includes a lot of features thus making this problem more challenging

##### Objective

Traditionally when a customer misses a 1-2 payments, most lending institutions flag the loan as potential at risk. Many of these loans are sold to collection agencies for pennies over dollar and loans are written off. This is sometime considered a cost to do business.
Post Covid and Work style changes, a re-look of the loan hyper parameters will save many of these defaulters and reduce the cost of doing business. This analysis plans to understand the features and predict whether a person who has defaulted on loan will be back being current again and pay back the loan. 


#### Source: https://www.kaggle.com/datasets/adarshsng/lending-club-loan-data-csv?resource=download
     Glossary: Field definitions are available at data/LCDataDictionary.xlsx


## Data Understanding
There are way more samples of fully paid borrowers versus not fully paid borrowers. This could be an issue when we make our prediction.
Also Income Distribution is skewed to left. The negative skewness of the distribution indicates that an Lending Club may expect frequent small gains and a few large losses.

#### Attribute Information:

 #   Column             Dtype  
---  ------             -----  
 0   policy_code        int64  
 1   purpose            object 
 2   int_rate           float64
 3   installment        float64
 4   annual_inc         float64
 5   dti                float64
 6   int_rate           float64
 7   acc_now_delinq     float64
 8   revol_bal          int64  
 9   revol_util         float64
 10  grade              object 
 11  loan_status        object 
 12  inq_last_6mths     float64
 13  delinq_2yrs        float64
 14  pub_rec            float64
 15  hardship_type      object 
 16  settlement_status  object 
 17  settlement_amount  float64
 18  addr_state         object 


## Team collaboration - directory structure

#### Instructions

- Clone the GitHub repository
- Please run the notebooks in sequence


├── data
│    ├── loan.csv
│    ├── LCDataDictionary.xlsx
│ 
├── images
│    ├── Correlation_Matrix.jpg  
│    ├── etc..    
| 
├── models
|    ├── predictive_maint.hd5 
|    ├── predictive_maint.json
├── 1. LendingClubData_EDA.ipynb
│   2.
├── presentation
|   ├── Final presentation



## Data Preparation and Visulalization

Code Used: Python
Packages: Pandas, Numpy, Matplotlib

## Data Cleansing, processing, and modeling

Code Used: Python
Packages: Pandas, tensorflow, Keras (Sequential, Dense, Dropout, lambda, Flatten, LSTM, Activation)

## Process Summary
**By performing different ML models, we aimed to get better at predictively optimizing 
- operational efficiency
- Recovery of debts
