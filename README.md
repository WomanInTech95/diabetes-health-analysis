# Diabetes Health Indicators Analysis

Exploratory analysis of diabetes risk factors using CDC Behavioral Risk Factor Surveillance System (BRFSS) 2015 data with Python, pandas, NumPy, and Matplotlib.

## Project Overview

This project explores health, lifestyle, demographic, and socioeconomic factors associated with diabetes using data derived from the 2015 Behavioral Risk Factor Surveillance System (BRFSS).

The dataset contains **253,680 survey responses** and **21 predictor variables**, including BMI, high blood pressure, physical activity, general health, age, education, and income.

The goal of this project was to assess data quality, explore patterns within the dataset, and identify factors associated with diabetes and prediabetes using Python.

## Dataset

The analysis uses the **Diabetes Health Indicators Dataset**, a cleaned and consolidated version of the CDC BRFSS 2015 survey data available through Kaggle.

The target variable contains three categories:

* **0:** No diabetes or diabetes only during pregnancy
* **1:** Prediabetes
* **2:** Diabetes

The dataset is imbalanced, with approximately **84.2%** of respondents classified as having no diabetes, **1.8%** as having prediabetes, and **13.9%** as having diabetes.

## Data Quality Assessment

Before conducting exploratory analysis, the dataset was evaluated for:

* Missing values
* Duplicate response patterns
* Variable types and categorical codes
* Numerical ranges
* Potential outliers
* Target-class distribution

No standard null values or obvious invalid category codes were identified.

A total of **23,899 exact duplicate response patterns** were identified. These observations were retained because the dataset does not contain a unique respondent identifier, making it impossible to determine whether identical responses represent true duplicate records or different respondents with the same characteristics.

Extreme BMI values were also retained because they remained physiologically possible and there was insufficient evidence to classify them as data errors.

## Exploratory Data Analysis

The analysis examined relationships between diabetes status and several health and socioeconomic indicators, including:

* BMI
* High blood pressure
* Age
* Physical activity
* Self-reported general health
* Household income

## Key Findings

* **BMI:** Average BMI increased from approximately **27.7** among respondents without diabetes to **30.7** among respondents with prediabetes and **31.9** among respondents with diabetes.
* **High blood pressure:** Approximately **75.3%** of respondents with diabetes reported high blood pressure, compared with **37.1%** of respondents without diabetes.
* **Age:** Diabetes prevalence generally increased with age and reached approximately **21.8%** among respondents ages 70–74.
* **Physical activity:** Approximately **63.1%** of respondents with diabetes reported physical activity compared with **77.9%** of respondents without diabetes.
* **General health:** Approximately **40.6%** of respondents with diabetes rated their general health as Fair or Poor compared with **13.1%** of respondents without diabetes.
* **Income:** Diabetes prevalence generally decreased as household income increased, from approximately **24.3%** in the lowest income category to **8.0%** in the highest income category.

## Tools & Skills

* Python
* pandas
* NumPy
* Matplotlib
* Data quality assessment
* Data validation
* Exploratory data analysis (EDA)
* Data aggregation
* Data visualization
* Public health data interpretation

## Important Considerations

This analysis is descriptive and does not establish causal relationships. BRFSS data are observational and largely self-reported, and the diabetes-status groups are substantially imbalanced.

These limitations should be considered when interpreting the findings or using the dataset for future predictive modeling.

## View the Analysis

The complete analysis, Python code, outputs, and visualizations are available in the `diabetes-health-analysis.ipynb` notebook in this repository.
