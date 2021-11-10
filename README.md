# Project Name
> Lenading club loan data analysis


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- Loan data was analyzed using EDA with python
- The company gives out loans to applicants and has collected data on past and current loans
- The goal was to identify factors that lead to loan default - so that it can avoid bad customers without losing business on good customers
- Dataset and its description was provided by the compny

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- EDA was performed
- Univariate, bivariate and multi-level interactions were studied
- Factors affecting defaults were identified​
- Factor combinations that lead to higher defaults were identified
- No machine learning methods were used ​
- further analysis with a method such as gradient boosting may be useful

<br>

### Important factors affecting default rate  
|Factor|Description|Dangerous level|
|-------------|------------|-------------|
|annual_inc_class​|Annual income categorical– derived from annual_inc​|Under 25th percentile​|
|amnt_to_income​|Loan amount as % of annual income​|Above median​|
|loan_amnt​|Amount of loan taken​|Above Median​|
|int_rate​|Interest rate​|Above Median​|
|pub_rec_bin​|Public derogatory records - 0 or 1 – derived from pub_rec​|Above 0​|
|purpose​|Why the loan was taken​|Small_business, Other​|
|addr_state​|State​|'NE', 'NV', 'SD', 'AK', 'FL', 'MO', 'OR'​|
|delinq_2yrs_bin​|delinquencies in last 2 years – derived from delinq_2yrs​|Above 1​|
|inq_last_6mths_bin​|inquiries in last 2 years – derived from inq_last_6mths​|Above 0​|
|term​|Loan term​|60 months​|

<br>

### Combinations for high default rate
|Combination for default rate higher than 14.4%​||||Default rate​|
|------------|------------|------------|------------|------------|
|annual_inc_class < 25th percentile|​int_rate > median|small_business loan​||41.66%​|
|annual_inc_class < 25th percentile​|int_rate > median| ​ small_business loan| ​ term = 60 months​|54.43%​|
|annual_inc_class < 25th percentile ​| amnt_to_income > median | small_business loan|​  term = 60 months​|48.78%​|
|annual_inc_class < 25th percentile​ | revol_bal > median |​ small_business loan​||43.75%​|

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Python - version 3.8.3

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- Kaggle eda discussed in live session - [house price eda](https://www.kaggle.com/ekami66/detailed-exploratory-data-analysis-with-python)
- US regions - [link](https://www.kaggle.com/omer2040/usa-states-to-region/version/1)



## Contact
Created by [@nvkhedkar] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->