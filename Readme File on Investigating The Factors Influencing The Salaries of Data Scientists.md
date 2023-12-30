# Project Title: Investigating The Factors Influencing The Salaries of Data Scientists.
# Introduction:
```python
- The aim of this study is to investigate the factors influencing the salaries of Data Scientists.
- To achieve this, a dataset containing various relevant variables was utilized. This report describes the exploratory
  analysis conducted to understand the relationship between these factors and Data Scientists' salaries.
```
# Analysis Questions:
```python
Investigate The Factors Influencing The Salaries of Data Scientists.
```
# Body:
### Data Overview:
```python
- ds_salaries.csv from kaggle
```
# Methods/Approaches:
### 1...Data Collection
```python
- ds_salaries.csv from kaggle
```
### 2...Reading The Datasets
```python
data = pd.read_csv('ds_salaries.csv')
```
### 3...Viewing The Datasets
```python
data = pd.read_csv('ds_salaries.csv')
```
### 4...Data Cleaning and Preparation
```python
1...Checking the number of rows and columns using an Attribute called.shape()
2...Checking Data Information using a pandas function called .info().
3...Checking duplicated data using .duplicated().any()
```
# Analysis:
<div>
<img style="margin:15px" height=400px width=500px src="https://github.com/Lekxite/project-screenshots/blob/main/Salaries%20of%20Data%20Scientists.md/Job%20Titles%20and%20Salaries%20in%20USD.png?raw=true" alt="Job Titles and Salaries in USD"/> 
<img style="margin:15px" height=400px width=500px src="https://github.com/Lekxite/project-screenshots/blob/main/Salaries%20of%20Data%20Scientists.md/Experience%20Levels%20and%20Salaries%20in%20USD.png?raw=true" alt="Experience Level and Salaries in USD"/>
<img style="margin:15px" height=400px width=500px src="https://github.com/Lekxite/project-screenshots/blob/main/Salaries%20of%20Data%20Scientists.md/Employment%20Type%20and%20Salaries%20in%20USD.png?raw=true" alt="Employment Type and Salaries in USD"/>
<img style="margin:15px" height=400px width=500px src="https://github.com/Lekxite/project-screenshots/blob/main/Salaries%20of%20Data%20Scientists.md/Salary%20Currency%20and%20Salaries%20in%20USD.png?raw=true" alt="Salary Currency and Salaries in USD"/>
<img style="margin:15px" height=400px width=500px src="https://github.com/Lekxite/project-screenshots/blob/main/Salaries%20of%20Data%20Scientists.md/Employee%20Residence%20and%20Salaries%20in%20USD.png?raw=true" alt="Employee Residence and Salaries in USD"/> 
<img style="margin:15px" height=400px width=500px src="https://github.com/Lekxite/project-screenshots/blob/main/Salaries%20of%20Data%20Scientists.md/Remote%20Ratio%20and%20Salaries%20in%20USD.png?raw=true" alt="Remote Ratio and Salaries in USD"/>
<img style="margin:15px" height=400px width=500px src="https://github.com/Lekxite/project-screenshots/blob/main/Salaries%20of%20Data%20Scientists.md/Company%20Location%20and%20Salaries%20in%20USD.png?raw=true" alt="Company Location and Salaries in USD"/>
<img style="margin:15px" height=400px width=500px src="https://github.com/Lekxite/project-screenshots/blob/main/Salaries%20of%20Data%20Scientists.md/Company%20Size%20%20and%20Salaries%20in%20USD.png?raw=true" alt="Company Size and Salaries in USD"/>
<div/>
  
# Results:
```python
- Data Engineer is the highest paid based on Salaries_in_USD. While Data Scientist and Data Analyst follow respectively.
- Senior level or Expert in Data Science earns more money than other experience levels.
- Full-Time(FT) Data Scientist earns more money than other Employment Type.
- Data Scientists that get paid in USD earn more money than those that earn in other currencies.
- Data Scientists that live in the US earn more money than others that live in other countries.
- Data Scientists that work On-Site get paid more than those that work remotely.
- Companies located in the US pay more salaries to Data Scientists than other companies located elsewhere.
- Medium-sized companies pay more salaries to Data Scientists than both Large and Small-sized companies.
```

# Conclusion:
```python
- According to this analysis, Senior-Level/expert, Full-Time, Data Scientists that earn salary in USD, live and
  work in the United State of America get paid more than others. 
```



