# Movie Theater Membership Analysis

## Background
This open-ended project uses a large dataset from a real-world client in the movie industry. The final project consists of two sections:  
1. **Business Intelligence**  
2. **Machine Learning**  

- **Section 1: Business Intelligence**  
  In this section, the task is to analyze movie theater membership data using various business intelligence techniques, such as data visualization with Pandas and pivot tables.

- **Section 2: Machine Learning**  
  In this section, the task is to analyze movie theater membership data using machine learning models.

## Problem Statement
The client has asked to develop insights from the provided data. Some of the business questions include (but are not limited to):
- Who are the customers likely to convert to Premier?
- Who are the customers that utilize Premier?
- Who are the customers that utilize Insider?

## Business Context & Significance of the Problem
- Provide the client with market insights into their rewards program to understand who is likely to convert to Premier.
- Identify frequent movie attendees and determine if they are utilizing their membership.
- Suggest ways the client could adjust their rewards program based on these insights.

## Data Dictionary
The client offers a theater dataset of loyalty members:

### Membership Types:
- **Insider members** (free program) who have not upgraded.
- **Premier members** (paid program) who were once Insider members and upgraded to the paid program.  
*Note*: The dataset only includes Premier members who upgraded from Insider, not those who directly bought into the Premier program without first being Insider members. The program has been live since June, so many metrics (e.g., spend) may still be low.

- **Each paid membership costs $20/year.**

### Variables:
- **ISPREMIER**:  
  - `0` if Insider  
  - `1` if Premier (i.e., the member has upgraded from Insider). This is the target binary variable to predict.

- **AGE21PLUSINDICATOR**:  
  - `0` is false  
  - `1` is true  

- **AGE18TO21INDICATOR**:  
  - `0` is false  
  - `1` is true  

- **AGE13TO18INDICATOR**:  
  - `0` is false  
  - `1` is true  

- **GENDERCODE**:  
  - `0` is female  
  - `1` is male  
  - `3` is unknown  

- **BIRTHDATE**: Date of birth.

- **LOYALTYEMAILOFFEROPTININDICATOR**:  
  - `0` is false  
  - `1` is true (Opted in to receive AMC Loyalty program email offers).

- **REWARDSEMAILOPTININDICATOR**:  
  - `0` is false  
  - `1` is true (Opted in to receive reward emails).

- **REWARDSMOBILEOPTININDICATOR**:  
  - `0` is false  
  - `1` is true (Opted in to receive mobile notifications for rewards).

- **REWARDSSMSOPTININDICATOR**:  
  - `0` is false  
  - `1` is true (Opted in to receive SMS messages for rewards).

- **THEATREMOBILEOFFEROPTININDICATOR**:  
  - `0` is false  
  - `1` is true (Opted in to receive mobile theater-level offers).

- **THEATRESMSOFFEROPTININDICATOR**:  
  - `0` is false  
  - `1` is true (Opted in to receive SMS theater-level offers).

- **LIFETIMEAWARDSEARNEDAMOUNT**: Amount of rewards earned in dollars by the member.

- **LIFETIMESPENDAMOUNT**: Total amount spent by the member.

- **ONLINEFEESWAIVEDAMOUNT**: Total dollars in online ticketing fees waived for the member.

- **ESTIMATEDINCOMERANGE**:  
  - `0`: Unknown  
  - `1`: Less than $15,000  
  - `2`: $15,000 - $19,999  
  - `3`: $20,000 - $29,999  
  - `4`: $30,000 - $39,999  
  - `5`: $40,000 - $49,999  
  - `6`: $50,000 - $74,999  
  - `7`: $75,000 - $99,999  
  - `8`: $100,000 - $124,999  
  - `9`: Greater than $124,999

- **ESTIMATEDHOMEMARKETVALUERANGE**:  
  - `0`: Unknown  
  - `1`: $1,000 - $24,999  
  - `2`: $25,000 - $49,999  
  - `3`: $50,000 - $74,999  
  - `4`: $75,000 - $99,999  
  - `5`: $100,000 - $124,999  
  - `6`: $125,000 - $149,999  
  - `7`: $150,000 - $174,999  
  - `8`: $175,000 - $199,999  
  - `9`: $200,000 - $224,999  
  - `10`: $225,000 - $249,999  
  - `11`: $250,000 - $274,999  
  - `12`: $275,000 - $299,999  
  - `13`: $300,000 - $349,999  
  - `14`: $349,000 - $399,999  
  - `15`: $400,000 - $449,999  
  - `16`: $450,000 - $499,999  
  - `17`: $500,000 - $749,999  
  - `18`: $750,000 - $999,999  
  - `19`: $1,000,000 plus  

- **CHILDRENPRESENCE**:  
  - `0`: False  
  - `1`: True  
  - `3`: Unknown (Has children present in household).

- **HASFREQUENTVISITTHEATRENUMBER**:  
  - `0`: False  
  - `1`: True (Has a most frequently visited theater selected).

- **TICKETQTYSUM**: Total number of tickets sold to this member.

- **TICKETBALANCEDUESUM**: Total amount in USD of tickets sold to this member.

- **CONCQTYSUM**: Total number of concession items purchased by this member.

- **CONCLOYDISCOUNTAMTSUM**: Total amount of loyalty discount received by this member (minus value in USD).

- **CONCBALANCEDUESUM**: Total amount in USD of concessions sold to this member.

## Data Quality
This is a real-world dataset, and it may contain data quality issues, such as inconsistencies, inaccuracies, and missing values. Various techniques will need to be applied to address these issues.

## License
[Insert license information here if applicable]
