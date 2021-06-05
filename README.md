# SQL-0
SQL projects and practice repository

Below are the log-in instructions to Google BigQuery, description of the datasets, and the 7 questions to answer. You have 90 minutes to email back the answers and SQL code that runs in BigQuery (StandardSQL). Feel free to use google. Good Luck.

Log-in instructions:

Head to link: https://cloud.google.com/bigquery/docs/sandbox
Click "Go To BigQuery"
Sign into personal Gmail account.
Agree to Terms and Conditions
Create default project (name doesn’t matter, but must be unique)
Click “+ Add Data” on the left side, then click “Pin a Project” and then select "Enter project name".
Type in “bigquery-public-data” in the field and click pin.
You should now be able to view and query all public tables
Dataset: `bigquery-public-data.usa_names.usa_1910_current`

Description: The table contains the number of applicants for a Social Security card by year of birth and sex. The number of such applicants is restricted to U.S. births where the year of birth, sex, State of birth (50 States and District of Columbia) are known, and where the given name is at least 2 characters long.

Fields:

state

STRING

2-digit state code

 

gender

STRING

Sex (M=male or F=female)

 

year

INTEGER

4-digit year of birth

 

name

STRING

Given name of a person at birth

 

number

INTEGER

Number of occurrences of the name

 

Dataset: `bigquery-public-data.geo_us_boundaries.states`

Description: The table contains geo data about all 50 states plus US territories. The columns you will need include a 2 digit state code, the FIPS code, and the area of water in the state.

Fields:

state

STRING

2-digit state code

state_fips_code

STRING

2-digit numeric state code

area_water_meters

INTEGER

Meters of land in state

 

Provide answer and Standard SQL code used to get answer for the following questions. All calculations should be done in SQL.

How many unique Male names were listed in 1984?
What were the 3 most popular Female names in 1945 and what was the number of Females that had each of those 3 names that year?
What year did the female name "Charlotte" reach its highest popularity rank vs. other names within that year and what rank was that?
In the year 2011, what was the most popular name and how many occurrences did that name have, for the state whose state_fips_code is 44.
What is the total number of occurrences of the Male name “Jamie” in the year 1988 for the states that have an area_water_meters between 1307243751 and 1550236199?
What is the most popular last letter of names in the 1990s (1990-99), and what % of names ended with that letter?
What is the annual growth rate in the number of people (Male or Female) that have a name that starts with “Sam” for each of the last 10 years (2007-2016) in the dataset?
