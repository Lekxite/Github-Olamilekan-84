# Project Title: Nigeria COVID-19 Data Analysis Using Python
# Introduction:
```python
- Coronavirus disease (COVID-19) is an infectious disease caused by a newly discovered coronavirus, and it has affected major 
  parts of the world. Nigeria, a West-African country, has also been affected by the COVID-19 pandemic after recording its first
  case on 27th February 2020.
- Nigeria is a country with 37 states - Federal Capital Territory included- and a fast-growing economic environment with about 
  200 million citizens. COVID-19 has affected several country activities as the country steadily progressed from its first case 
  to shutting down major airports, state-wide lockdown, curfews, and reviving its economy.
- The major aim of writing this report is to evaluate the negative impact of covid-19 on Nigeria's economy and how the country
  managed to survive it.
```
# Analysis Questions:
```python
- Generate a plot that shows the Top 10 states in terms of Confirmed Covid cases by Laboratory test.
- Generate a plot that shows the Top 10 states in terms of Discharged Covid cases. Hint - Sort the values.
- Plot the top 10 Death cases.
- Generate a line plot for the total daily confirmed, recovered and death cases in Nigeria.
- Determine the daily infection rate, you can use the Pandas diff method to find the derivate of the total cases.
- Generate a line plot for the above.
- Calculate maximum infection rate for a day (Number of new cases).
- Find the date.
- Determine the relationship between the external dataset(overall community vulnerability index) and the NCDC COVID-19 dataset.
- Determine the relationship between the external dataset and the NCDC COVID-19 dataset(Confirmed Cases and Population Density).
- Provide a summary of your observation.
- Determine the effect of the Pandemic on the economy. To do this, you will compare the Real GDP value Pre-COVID-19 
  with Real GDP in 2020 (COVID-19 Period, especially Q2 2020.
```
# Body:
### Data Overview:
```python
# 1...covidnig.csv from NCDC Website, with 37 Rows and 5 Columns.
# 2...(a) Global Daily Confirmed Cases from John Hopkins Repository, with 289 Rows and 1147 Columns.
#   ...(b) Global Daily Recovered Cases from John Hopkins Repository, with 274 Rows and 1147 Columns.
#   ...(c) Global Daily Death Cases from John Hopkins Repository, with 289 Rows and 1147 Columns.
# 3...External Data from Ustacky Github Repository such as:
#   ...(a) covid_external.csv. It has 32 Rows and 12 Columns.
#   ...(b) Budget data.csv, with 37 Rows and 3 Columns.
#   ...(c) RealGDP.csv, with 7 Rows and 5 Columns.
```
# Methods/Approaches:
### 1...Data Collection
```python
#1...covidnig.csv from NCDC Website
#2...(a) Global Daily Confirmed Cases from John Hopkins Repository
#...(b) Global Daily Recovered Cases from John Hopkins Repository
#...(c) Global Daily Death Cases from John Hopkins Repository
#3...External Data such as:
#...(a) covid_external.csv
#...(b) Budget data.csv
#...(c) RealGDP.csv
```
### 2...Reading The Datasets
```python
# data = pd.read_csv('covidnig.csv')
# confirmed = pd.read_csv('https://raw.githubusercontent.com/CSSEGISandData/COVID-19/master/csse_covid_19_data/csse_covid_19_time_series/time_series_covid19_confirmed_global.csv')
# recovered = pd.read_csv('https://raw.githubusercontent.com/CSSEGISandData/COVID-19/master/csse_covid_19_data/csse_covid_19_time_series/time_series_covid19_recovered_global.csv')
# deaths = pd.read_csv('https://raw.githubusercontent.com/CSSEGISandData/COVID-19/master/csse_covid_19_data/csse_covid_19_time_series/time_series_covid19_deaths_global.csv')
# covid_external = pd.read_csv('https://raw.githubusercontent.com/Ustacky-dev/Nigeria-COVID-19-Data-Analysis-Using-Python/main/covid_external.csv')
# BG = pd.read_csv('https://raw.githubusercontent.com/Ustacky-dev/Nigeria-COVID-19-Data-Analysis-Using-Python/main/Budget%20data.csv')
# RG = pd.read_csv('https://raw.githubusercontent.com/Ustacky-dev/Nigeria-COVID-19-Data-Analysis-Using-Python/main/RealGDP.csv')
```
### 3...Viewing The Datasets
```python
# data = pd.read_csv('covidnig.csv')
# confirmed = pd.read_csv('https://raw.githubusercontent.com/CSSEGISandData/COVID-19/master/csse_covid_19_data/csse_covid_19_time_series/time_series_covid19_confirmed_global.csv')
# recovered = pd.read_csv('https://raw.githubusercontent.com/CSSEGISandData/COVID-19/master/csse_covid_19_data/csse_covid_19_time_series/time_series_covid19_recovered_global.csv')
# deaths = pd.read_csv('https://raw.githubusercontent.com/CSSEGISandData/COVID-19/master/csse_covid_19_data/csse_covid_19_time_series/time_series_covid19_deaths_global.csv')
# covid_external = pd.read_csv('https://raw.githubusercontent.com/Ustacky-dev/Nigeria-COVID-19-Data-Analysis-Using-Python/main/covid_external.csv')
# BG = pd.read_csv('https://raw.githubusercontent.com/Ustacky-dev/Nigeria-COVID-19-Data-Analysis-Using-Python/main/Budget%20data.csv')
# RG = pd.read_csv('https://raw.githubusercontent.com/Ustacky-dev/Nigeria-COVID-19-Data-Analysis-Using-Python/main/RealGDP.csv')
```
### 4...Data Cleaning and Preparation
```python
# 1...Checking the number of rows and columns using an Attribute called .shape
# 2...Checking statistical summary of the dataframe using a pandas function called .discribe()
# 3...Checking the missing values using a pandas function called (.isnull().sum()
# 4...Changing Columns Names where necessary.
# 5...Checking Data Information using a pandas function called .info().
# 6...Dropping Columns that were not needed using .drop().
# 7...Renaming Columns
# 8...Dealing with Datetime features
```
<div>
  <img style="margin:15px" height=250px width=250px src="https://github.com/Lekxite/project-screenshots/blob/main/New-Capstone-Screenshots.md/Top%2010%20States%20with%20Lab%20Confirmed%20Cases.png?raw=true" alt="Top 10 States with Lab Confirmed Cases"/>
  <img style="margin:15px" height=250px width=250px src="https://github.com/Lekxite/project-screenshots/blob/main/New-Capstone-Screenshots.md/Top%2010%20States%20with%20Smallest%20Lab%20Confirmed%20Cases.png?raw=true" alt="Top 10 States with Smallest Lab Confirmed Cases"/>
 <img style="margin:15px" height=250px width=250px src="https://github.com/Lekxite/project-screenshots/blob/main/New-Capstone-Screenshots.md/Top%2010%20States%20with%20No%20of%20Discharged%20Cases.png?raw=true" alt="Top 10 States with No of Discharged Cases"/>
  <img style="margin:15px" height=250px width=250px src="https://github.com/Lekxite/project-screenshots/blob/main/New-Capstone-Screenshots.md/Top%2010%20States%20with%20Smallest%20No%20of%20Discharged%20Cases.png?raw=true" alt="Top 10 States with Smallest No of Discharged Cases"/>
  <img style="margin:15px" height=250px width=250px src="https://github.com/Lekxite/project-screenshots/blob/main/New-Capstone-Screenshots.md/Top%2010%20States%20with%20No%20of%20Death%20Cases.png?raw=true" alt="Top 10 States with No of Deaths Cases"/>
  <img style="margin:15px" height=250px width=250px src="https://github.com/Lekxite/project-screenshots/blob/main/New-Capstone-Screenshots.md/Top%2010%20States%20with%20Smallest%20No%20of%20Death%20Cases.png?raw=true" alt="Top 10 States with Smallest No of Deaths Cases"/>
  <img style="margin:15px" height=250px width=250px src="https://github.com/Lekxite/project-screenshots/blob/main/New-Capstone-Screenshots.md/Daily%20Confirmed%20Cases.png?raw=true" alt="Daily Confirmed Cases"/>
  <img style="margin:15px" height=250px width=250px src="https://github.com/Lekxite/project-screenshots/blob/main/New-Capstone-Screenshots.md/Daily%20Recovered%20Cases.png?raw=true" alt="Daily Recovered Cases"/>
  <img style="margin:15px" height=250px width=250px src="https://github.com/Lekxite/project-screenshots/blob/main/New-Capstone-Screenshots.md/Daily%20Death%20Cases.png?raw=true" alt="Daily Death Cases"/>
  <img style="margin:15px" height=250px width=250px src="https://github.com/Lekxite/project-screenshots/blob/main/New-Capstone-Screenshots.md/Daily%20Infection%20Rate.png?raw=true" alt="Daily Infection Rate"/>
  <img style="margin:15px" height=250px width=250px src="https://github.com/Lekxite/project-screenshots/blob/main/New-Capstone-Screenshots.md/Relationship%20Between%20Overall%20CCVI%20Index%20&%20Lab%20Confirmed%20Cases.png?raw=true" alt="Relationship Between Overall CCVI Index & Lab Confirmed Cases"/>
   <img style="margin:15px" height=250px width=250px src="https://github.com/Lekxite/project-screenshots/blob/main/New-Capstone-Screenshots.md/Budget%20Adjustment%20in%2010%20Leading%20States.png?raw=true" alt="Budget Adjustment in 10 Leading States"/>
  <img style="margin:15px" height=250px width=250px src="https://github.com/Lekxite/project-screenshots/blob/main/New-Capstone-Screenshots.md/Linear%20Relationship%20Between%20Population%20Density%20&%20Lab%20Confirmed%20Cases.png?raw=true" alt="Linear Relationship Between Population Density & Lab Confirmed Cases"/>
  <img style="margin:15px" height=250px width=250px src="https://github.com/Lekxite/project-screenshots/blob/main/New-Capstone-Screenshots.md/RealGDP%20Values%20Before%20and%20During%20Covid-19.png?raw=true" alt="RealGDP Values Before and During Covid-19"/>
</div>

# Results:
```python
- Lagos State had the highest Laboratory Confirmed cases of covid-19
- While Kogi State recorded lowest Laboratory confirmed cases of covid-19
- Lagos State had the highest Number of Discharged people from covid-19 Isolation Centers
- Kogi State had the lowest No of Discharged people from covid-19
- Lagos State recorded the highest No of Deaths of people with covid-19
- Kogi State recorded the lowest No of Deaths of people with covid-19
- The rate of daily Confirmed Cases of covid-19 was much higher in March, 2023
- The rate of daily recovered cases of covid-19 started rising from July 2021 to August 2021.
- The daily death cases from November 2022 to March 2023 remains the unchanged. There is no increase.
- The Maximum Daily Infection Rate was over 6000 cases. And this occured on December 22nd, 2021.
- Negative Relationship exists between the Overall Community Vulnerability Index(CCVI) and the Laboratory Confirmed Cases,
  as the Overall CCVI Index decreases, Laboratory Confirmed Cases surge.
- The initial budgets of States were revised and reduced due to the effects of covid-19. And this had adverse effects on the
  economy
- There was a positive relationship between Population and Laboratory Confirmed Cases. As Population
  increases(denser population), more people were infected with covid-19 virus
- The RealGDP value in the quarter 1 (Q1 2020) were much higher. But when it got to Q2, Q3 & Q4 2020, the RealGDP value reduces.
  In fact, according to this analysis, there was no RealGDP value in Q4 2020. This could be attributed to the spread of the
  virus in some parts of the country. This had greater negative effects on Nigerian economy.
```
# Conclusion:
```python
- The emergence of Coronavirus disease lead to shutting down of major airports,seaports, state-wide lockdown, curfews, 
  in Nigeria. This really affected the economy negatively as reflected in the analysis. 
- A country whose Gross Domestic Value(GDP)
  reduces due to one problem or another really ecounters economic meltdown. 
``` 
