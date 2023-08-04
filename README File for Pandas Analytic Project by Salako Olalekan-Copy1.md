# Project Title: Pandas Analytics-Analysis of 3 Different Branches of Company XYZ across Nigeria.
# Project Steps:
# 1...Data Collection:
### ...Datasets for The 3 Branches of Company XYZ(Lagos, Abuja & Port Harcourt) from The Company Repository
# 2...Reading The Datasets
```python
df1 = pd.read_csv('Abuja_Branch.csv')
df2 = pd.read_csv('Lagos_Branch.csv')
df3 = pd.read_csv('Port_Harcourt_Branch.csv')
```
# 3...Combining The 3 Datasets
```python
dff = pd.concat([df1, df2, df3])
```
# 4...Creating New Variable for The Concatenated Datasets and Save it back to The Database in csv format
```python
Newdataset = ['df1', 'df2', 'df3']
dff.to_csv('Newdataset.csv', index = False)
```
# 5...Viewing The Dataset
```python
dff = pd.read_csv('Newdataset.csv')
```
# 6 Data Cleaning and Preparation
```python
1...Checking the number of rows and columns using an Attribute called .shape
2...Checking statistical summary of the dataframe using a pandas function called .discribe()
3...Checking the missing values using a pandas function called (.isnull().sum()
4...Checking non-missing values using another pandas function (.notna().sum())
5...Combining the date and time columns, and gave it a new variable name (New_date)
6...Converting the New_date column to datetime datatype using a pandas function called (pd.to_datetime())
7...Creating new columns for Day, Month, Year & Hour from New_date column
8...Checking Data Information using a pandas function called .info()
9...Dealing with Datetime features
```
# Insights:
```python
Pandas Analytics datasets of Company XYZ gave me an opportunity to understand the following:
  - The quantities of product lines sold.
  - The reason why some product lines had higher demand than others.
  - The payment channel for each product line, the branch with highest and lowest rating.
  - The highest payment channel for each branch.
  - The branch that had highest sales record, and the branch with highest gross income
```
# Future Work:
```python
  - The future work can be more robust and challenging to students if the datasets that have missing values are given.
  - In this case students will be given the task of checking for the missing values, 
    and looking for a way of replacing or dropping them.
  - Moreover, the datasets given were too clean. Please, in the future,
    always give the students the task of cleaning the data by themselves.
  - This will improve their skills in the aspect of Data Cleaning and Processing.
```
# Findings:
```python
  - Port Harcourt is The City with The Highest sum of Cost of Good Sold(cogs) of 37909270.8
  - Port Harcourt has The Highest mean of Cost of Good Sold(cogs) of 115577.045122
  - Port Harcourt has The Highest gross income of 1895463.54
  - City with The Highest Unit Price is Lagos
  - The City with Highest Quantity is Lagos
  - City with The Most Sales is Port Harcourt
  - The Branch with The Highest Sales Record is Lagos
  - The Most Used Payment Method is Epay
  - The Highest Sold Product line is Food and Beverages, closely followed by Sports and Travel.
    While The Lowest Sold Product line is Heath and Beauty
  - The payment channel used by most customers to pay for Electronic Accessories is cash
  - The payment channel used by most customers to pay for Food and Beverages is card
  - The payment channel used by most customers to pay for Fashion Accessories is Epay
  - The payment channel used by most customers to pay for Sports and Travel is cash
  - The payment channel used by most customers to pay for Home and Lifestyle is Epay
  - The payment channel used by most customers to pay for Health and Beauty is Epay
  - The highest payment channel for Abuja_Branch is Card.
  - The highest payment channel for Lagos_Branch is Epay.
  - The highest payment channel for Port_Harcourt_Branch is Cash
  - Lagos had the highest sales of Electronic Accessories
  - Port Harcourt had the highest sales of Fashion Accessories
  - Port Harcourt had the highest sales of Food and beverages
  - Abuja had the highest sales of Sports and travel
  - Lagos had the highest sales of Home and lifestyle
  - Abuja had the highest sales of Health and beauty
  - The Branch with Lowest Rating is Abuja
  - The Branch with Highest Rating is Lagos
  - The Most Purchased Product line based on Gender Type is Electronic Accessories
  - Based on the analysis here, electronic accessories were the most sold Product line with a bit higher price.
  - Fashion accessories were so expensive and very little quantities were purchased. Meanwhile, health and beauty
    accessories were the least sold Product line despite lower prices.
```
# Screenshots
<div>
  <img style="margin:15px" height=300px width=300px src="https://github.com/Lekxite/project-screenshots/blob/main/pandas-screenshots/Branch%20with%20Highest%20and%20Lowest%20Rating%20(1).png?raw=true" alt="Branch with Highest and Lowest Rating"/>
  <img style="margin:15px" height=300px width=300px src="https://github.com/Lekxite/project-screenshots/blob/main/pandas-screenshots/City%20with%20The%20Most%20Sales.png?raw=true" alt="City with The Most Sales"/>
</div>

# Summary
```python
Company XYZ had 3 branches(Lagos, Abuja and Port Harcourt). And according to the analysis, it made its highest Gross Income
from Port Harcourt branch. Hence, efforts should be made to allocate more products to this branch. Also, more promotions
should be carried out in this branch for more profits in the future.
Moreso, according to the analysis, Lagos branch, despite its highest sales record and ratings than the 2 other branches,
the Gross Income was lower than that of Port Harcourt. This might be attributed to higher prices of products in this branch.  
Hence, efforts should be made by the company to reduce the price of the products. Also more promotions should be carried out
to improve sales and profits in the future.  
Meanwhile, Abuja branch recorded lower Gross Income, sales and ratings than the two other branches. The company should make
efforts to promote sales at this branch to improve sales and profits in the future.  
According to the analysis, more Electronic Accessories and Home & Style products should be allocated to Lagos branch  
More Fashion Accessories and Food & Beverages should be allocated to Port Harcourt branch  
More Sports & Travel and Health & Beauty products should be allocated to Abuja branch
```
