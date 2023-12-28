# Project Title: Financial Statements of Major Companies(2009-2023)
# Introduction:
```python
- This is a compiled datasets comprising of data from various companies' 10-K annual reports and balance sheets.
- The data is a longitudinal or panel data, from year 2009-2022(/23) and also consists 
  of a few bankrupt companies to help for investigating factors.
- The names of the companies are given according to their Stocks.
- Companies divided into specific categories.
```
# Analysis Questions:
```python
- Analyze a compiled datasets comprising of data from various companies' 10-K annual reports and balance sheets. 
- Fetch the companies that grew since 2009 2023, and the ones that went bankrupt, from the given datasets.
- Investigate the factors that led to the growth and bankruptcy of these companies.
```
# Body:
### Data Overview:
```python
- Financial Statements.csv from kaggle, with 161 rows and 23 columns.
```
# Methods/Approaches:
### 1...Data Collection
```python
- Financial Statements.csv from kaggle
```
### 2...Reading The Datasets
```python
- data = pd.read_csv('FinancialStatements.csv')
```
### 3...Viewing The Datasets
```python
data = pd.read_csv('FinancialStatements.csv')
```
### 4...Data Cleaning and Preparation
```python
1...Checking the number of rows and columns using an Attribute called.shape()
2...Checking Data Information using a pandas function called .info().
3...Checking duplicated data using .duplicated().any()
```
# Analysis:
<div>
  <img style="margin:15px" height=400px width=500px src="https://github.com/Lekxite/project-screenshots/blob/main/Financial-Statements.md/MSFT.png?raw=true" alt="MSFT"/>
  <img style="margin:15px" height=400px width=500px src="https://github.com/Lekxite/project-screenshots/blob/main/Financial-Statements.md/NVDA.png?raw=true" alt="NVDA"/>
  <img style="margin:15px" height=400px width=500px src="https://github.com/Lekxite/project-screenshots/blob/main/Financial-Statements.md/AAPL.png?raw=true" alt="AAPL"/>
  <img style="margin:15px" height=400px width=500px src="https://github.com/Lekxite/project-screenshots/blob/main/Financial-Statements.md/GOOG.png?raw=true" alt="GOOG"/>
  <img style="margin:15px" height=400px width=500px src="https://github.com/Lekxite/project-screenshots/blob/main/Financial-Statements.md/AIG.png?raw=true" alt="AIG"/>
  <img style="margin:15px" height=400px width=500px src="https://github.com/Lekxite/project-screenshots/blob/main/Financial-Statements.md/PCG.png?raw=true" alt="PCG"/>
  <img style="margin:15px" height=400px width=500px src="https://github.com/Lekxite/project-screenshots/blob/main/Financial-Statements.md/MCD.png?raw=true" alt="MCD"/>
  <img style="margin:15px" height=400px width=500px src="https://github.com/Lekxite/project-screenshots/blob/main/Financial-Statements.md/BCS.png?raw=true" alt="BCS"/>
  <img style="margin:15px" height=400px width=500px src="https://github.com/Lekxite/project-screenshots/blob/main/Financial-Statements.md/INTC.png?raw=true" alt="INTC"/>
  <img style="margin:15px" height=400px width=500px src="https://github.com/Lekxite/project-screenshots/blob/main/Financial-Statements.md/AMZN.png?raw=true" alt="AMZN"/>
  <img style="margin:15px" height=400px width=500px src="https://github.com/Lekxite/project-screenshots/blob/main/Financial-Statements.md/SHLDQ.png?raw=true" alt="SHLDQ"/>
  <img style="margin:15px" height=400px width=500px src="https://github.com/Lekxite/project-screenshots/blob/main/Financial-Statements.md/PYPL.png?raw=true" alt="PYPL"/>
</div>

# Results:
```python
- MSFT has been growing from 2009-2023. The factors responsible for this were Revenue generated,
  increase in Number of Employees and Share Holder Equity.
- NVDA was the most successful of all the companies. It has been growing since 2009-2023.The factors responsible
  for this were Market Capitalization, Revenue generated, Number of Employees and Share Holder Equity.
- AAPL also has been growing since 2009-2022. The factors responsible for this were Revenue generated
  and increase in Number of Employees.
- GOOG has been growing since 2009-2022. The factors responsible for this were Revenue generated, 
  Share Holder Equity and increase in Number of Employees.
- AIG has been declining in growth since 2015-2022. The factors responsible for the bankruptcy
  were low Market Cap, Revenue generated, Net Income, Share Holder Equity and decrease in Number of Employees.
- Despite the drop in Net Income in 2018-2021, PCG still performed through factors like Market Cap,
  Revenue generated, Share Holder Equity and increase in Number of Employees.
- MCD also experienced a decrease in growth since 2013-2022. Among the factors responsible for this were
  low Market Cap, Revenue generated, Net Income, Share Holder Equity and decrease in Number of Employees.
- BCS was another company that got liquidated due to low Market Cap, Revenue generated,
  Net Income, Share Holder Equity and decrease in Number of Employees.
- INTC also performed very well since 2009-2022 through some factors like Revenue generated, 
  Share Holder Equity and increase in Number of Employees.
- AMZN performed very well from 2009-2021. But in 2022 there was a drop in growth due to low or negligible Net Income.
- SHLDQ has also been dropping in growth since 2011-2018. Some factors like low Market Cap,
  Revenue generated, Net Income, Share Holder Equity and a decrease in Number of Employees were responsible for this.
- PYPL has been performing well since 2014 to 2021.The growth dropped slightly in 2022 due to some
  factors like low Market Cap,Net Income, Share Holder Equity and a decrease in Number of Employees
```
# Conclusion:
```python
- Five economic factors were used to analyze the dataset got from Kaggle website.
- The dataset stated the financial statements of 12 different companies from 2009-2023.
- NVDA was the most succesful of all the companies analyzed. While companies like AIG.
  MCD, BCS and SHLDQ went bankrupt due to economic factors mentioned above.
- 

```   
