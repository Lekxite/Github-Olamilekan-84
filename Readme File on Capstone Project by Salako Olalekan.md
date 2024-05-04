# Project Title: Pandas Analytics-Analysis of 3 Different Branches of Company XYZ across Nigeria.
# Introduction:
```python
- Company XYZ owns a supermarket chain across the country. Each major branch located in 3 cities across the country recorded
  sales information for 3 months, to help the company understand sales trends and determine its growth, as the rise of supermarkets
  competition is seen to increase.
- The data folder contains datasets from three different branches; Lagos, Abuja and Port Harcourt.
```
# Analysis Questions:
```python
- Data Statistical Information.
- Which city has the highest sum of Cost of Goods Sold(COGS)?
- Which city has the highest mean of Cost of Googs Sold(COGS)?
- Which city has the highest Gross Income?
- Which city has the highest Unit Price?
- Which city has the highest quantity of goods?
- Which branch has the highest sales record?
- Which one is the most used payment method?
- Which one is the highest sold prpduct line?
- State the payment method/chanel used by most customers for each product line
- State the highest payment channel/method for each branch
- Which is the most available product line in terms of Qty?
- List the highest sold product line in each city
- Name the branch with highest and lowest ratings
- Mention the most purchased product line
- Briefly explain the interacion of Unit Price and Quantity of goods purchased
```
# Body:
### Data Overview:
```python
...Datasets for The 3 Branches of Company XYZ(Lagos, Abuja & Port Harcourt) from The Company Repository
...with 1000 rows and 17 columns
```
# Methods/Approaches:
### 1...Data Collection
```python
1...'Abuja_Branch.csv' from Company's Repository
2...'Lagos_Branch.csv' from Company's Repository
3...'Port_Harcourt_Branch.csv' from Company's Repository
```
### 2...Reading The Datasets
```python
1...df1 = pd.read_csv('Abuja_Branch.csv')
2...df2 = pd.read_csv('Lagos_Branch.csv')
3...df3 = pd.read_csv('Port_Harcourt_Branch.csv')
```
### 3...Viewing The Datasets
```python
1...df1 = pd.read_csv('Abuja_Branch.csv')
2...df2 = pd.read_csv('Lagos_Branch.csv')
3...df3 = pd.read_csv('Port_Harcourt_Branch.csv')
```
### 4...Data Cleaning and Preparation
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
# Insights
```python
- More products should be given to Port-Harcourt branch. And advertisement on all the products should not stop.
- There is a lot more to do on Abuja branch. New marketing strategies should be carried out to boost sales.
```
# Future Work:
```python
- The future work can be more challenging to students if the datasets that have missing values are given.
  In this case students will be given the task of checking for the missing values, and looking for a way of
  replacing or dropping them.
- Moreover, the datasets given were too clean. Please, in the future, always give the students the task of
  cleaning the data as this will improve their skills in the aspect of Data Cleaning and Processing.
```
# Analysis:
<div>
  <img style="margin:15px" height=250px width=250px src="https://github.com/Lekxite/project-screenshots/blob/main//pandas-screenshots/Sum%20of%20Cost%20of%20Good%20Sold%20for%20Each%20City%20(1).png?raw=true" alt="Sum of Cost of Goods Sold(COGS) for Each City"/>
  <img style="margin:15px" height=250px width=250px src="https://github.com/Lekxite/project-screenshots/blob/main/pandas-screenshots/Mean%20of%20Cost%20of%20Good%20Sold%20for%20Each%20City%20(1).png?raw=true" alt="Mean of Cost of Goods Sold for Each City"/>
  <img style="margin:15px" height=250px width=250px src="https://github.com/Lekxite/project-screenshots/blob/main/pandas-screenshots/Sum%20of%20Gross%20Income%20for%20Each%20City%20(1).png?raw=true" alt="Sum of Gross Income for Each City"/>
  <img style="margin:15px" height=250px width=250px src="https://github.com/Lekxite/project-screenshots/blob/main/pandas-screenshots/Unit%20Price%20for%20Each%20City%20(1).png?raw=true" alt="Unit Price for Each City"/>
  <img style="margin:15px" height=250px width=250px src="https://github.com/Lekxite/project-screenshots/blob/main/pandas-screenshots/Quantity%20for%20Each%20City%20(1).png?raw=true" alt="Quantity for Each City"/>
  <img style="margin:15px" height=250px width=250px src="https://github.com/Lekxite/project-screenshots/blob/main/pandas-screenshots/The%20Branch%20with%20Highest%20Sales%20Record.png?raw=true" alt="The Branch with Highest Sales Record"/> 
  <img style="margin:15px" height=250px width=250px src="https://github.com/Lekxite/project-screenshots/blob/main/pandas-screenshots/The%20Most%20used%20Payment%20Method.png?raw=true" alt="The Most Used Payment Method"/>
  <img style="margin:15px" height=250px width=250px src="https://github.com/Lekxite/project-screenshots/blob/main/pandas-screenshots/The%20Highest%20Sold%20Product%20Line%20for%20Each%20City.png?raw=true" alt="The Highest Sold Product Line for Each City"/>
 <img style="margin:15px" height=250px width=250px src="https://github.com/Lekxite/project-screenshots/blob/main/pandas-screenshots/The%20Payment%20Channel%20used%20by%20Most%20Customers.png?raw=true" alt="The Payment Channel Used by Most Customers"/>
 <img style="margin:15px" height=250px width=250px src="https://github.com/Lekxite/project-screenshots/blob/main/pandas-screenshots/The%20Highest%20Payment%20Channel%20for%20Each%20Branch.png?raw=true" alt="The Highest Payment Channel for Each Branch"/>
  <img style="margin:15px" height=250px width=250px src="https://github.com/Lekxite/project-screenshots/blob/main/pandas-screenshots/Most%20Available%20Product%20Line%20in%20Terms%20of%20Qty%201.png?raw=true" alt="The Most Available Product Line in Terms of Qty"/>
  <img style="margin:15px" height=250px width=250px src="https://github.com/Lekxite/project-screenshots/blob/main/pandas-screenshots/Most%20Sold%20Product%20line.png?raw=true" alt="The Highest Sold Product Line"/> 
  <img style="margin:15px" height=250px width=250px src="https://github.com/Lekxite/project-screenshots/blob/main/pandas-screenshots/Branch%20with%20Highest%20and%20Lowest%20Rating%20(1).png?raw=true" alt="Branch With Highest and Lowest Rating"/>
  <img style="margin:15px" height=250px width=250px src="https://github.com/Lekxite/project-screenshots/blob/main/pandas-screenshots/Interaction%20of%20Unit%20Price%20&%20The%20Quantity%20of%20Goods%20Purchased.png?raw=true" alt="Interaction of Unit Price & 
  The Qty of Goods Purchased"/>  
</div>

# Findings:
```python
- Port Harcourt is The City with The Highest sum of Cost of Good Sold(cogs) of 37909270.8
- Port Harcourt has The Highest mean of Cost of Good Sold(cogs) of 115577.045122
- Port Harcourt has The Highest gross income of 1895463.54
- The City with Highest Unit Price is Lagos
- The City with Highest Quantity is Lagos
- City with The Most Sales is Port Harcourt
- The Branch with The Highest Sales Record is Lagos
- The Most Used Payment Method is Epay
- The Highest Sold Product line is Food and Beverages, closely followed by Sports and Travel.
  While The Least Sold Product line is Heath and Beauty
a.. The payment channel used by most customers to pay for Electronic Accessories is cash
b.. The payment channel used by most customers to pay for Food and Beverages is card
c.. The payment channel used by most customers to pay for Fashion Accessories is Epay
d.. The payment channel used by most customers to pay for Sports and Travel is cash
e.. The payment channel used by most customers to pay for Home and Lifestyle is Epay
f.. The payment channel used by most customers to pay for Health and Beauty is Epay
a.. The highest payment channel for Abuja_Branch is Card.
b.. The highest payment channel for Lagos_Branch is Epay.
c.. The highest payment channel for Port_Harcourt_Branch is Cash
a...Lagos had the highest sales of Electronic Accessories
b...Port Harcourt had the highest sales of Fashion Accessories
c...Port Harcourt had the highest sales of Food and beverages
d...Abuja had the highest sales of Sports and travel
e...Lagos had the highest sales of Home and lifestyle
f...Abuja had the highest sales of Health and beauty
a...The Branch with Lowest Rating is Abuja
b...The Branch with Highest Rating is Lagos
- The Most Purchased Product line in Terms of Qty is Electronic Accessories
- Based on the analysis, electronic accessories were the most sold Product line with a bit higher prices.
- Fashion accessories were so expensive and very little quantities were purchased.
- Health and Beauty were the least sold Product line despite lower prices. 
```
# Summary
```python
- More products should be given to Port-Harcourt branch. And advertisement on all the products should not stop.
- There is a lot more to do on Abuja branch. New marketing strategies should be carried out to boost sales.
- Health and Beauty product line should be given much more priority in terms of good marketing srategies and
  promotions on regular basis.
``` 

