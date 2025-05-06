# 🦠 COVID-19 Global Data Trends using PySpark

This project analyzes global COVID-19 data using PySpark. It covers various analytical insights like case trends, vaccination progress, mortality rates, testing rates, and more using a distributed data processing approach.

## 📁 Dataset

- **Source:** [Our World in Data (OWID)](https://ourworldindata.org/coronavirus)
- **File Used:** [covid-data.csv](./covid-data.csv)
- **Description:** Contains country-wise daily COVID-19 statistics including new cases, deaths, vaccinations, and testing information.
  

## 🚀 Technologies Used

- Python
- PySpark
- Google Colab
- PySpark SQL functions

## 📊 Key Analyses Performed

### 1. 📥 Data Loading
- Loaded the COVID-19 dataset using SparkSession.
- Used schema inference and header recognition.

### 2. 🧹 Data Cleaning
- Dropped rows with missing critical fields like `location`, `date`, and `total_cases`.
- Converted the `date` column to proper date format.

### 3. 🌍 Total Cases and Deaths by Country
- Aggregated total cases and deaths per country using `groupBy` and `max`.

### 4. 🇮🇳 Daily New Cases Trend in India
- Filtered data for India and visualized the trend of daily new cases.

### 5. 💉 Vaccination Progress by Country
- Summarized the number of people vaccinated and total vaccinations for each country.

### 6. ⚰️ Mortality Rate by Country
- Computed mortality rate using:  
  \[
  \text{mortality\_rate} = \left(\frac{\text{deaths}}{\text{cases}}\right) \times 100
  \]

### 7. 🕒 Late Vaccine Rollout Countries
- Identified countries with the latest start dates for vaccination.

### 8. 🌊 Comparing India's First and Second Wave
- Segregated new cases into two time periods and compared total cases:
  - First Wave: Before Jan 1, 2021
  - Second Wave: Jan 1, 2021 to May 31, 2021

### 9. 🧪 Top Countries by Testing Rate
- Listed countries by `total_tests_per_thousand`.

### 10. 📈 Countries with Most Fluctuating Cases
- Used standard deviation of daily new cases to measure volatility.


### 🧠 Learnings

- Gained hands-on experience in big data processing using PySpark.
- Learned how to handle and analyze real-world public health datasets.
- Practiced writing optimized PySpark SQL code for transformation and aggregation.

