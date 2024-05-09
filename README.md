# Life-Expectancy-Linear-Regression



## Executive Summary
* **Problem**: What are the key factors that influence life expectancy across different countries?
* **Data Source**: Life Expectancy World of Health Organization from Kaggle
* **Methods Used**: Multi-linear Regression Model, Collinearity, Residual Plots
* **Measures Used**: Variables, P-values of Variables, Multicollinearity/Correlation
* **Conclusion**: The most significant variables are **Adult Morality** & **Alcohol Consumption**. However, it's concluded that addition data from different countries would be necessary to develop more accurate results.

## Problem Statement: What Am I Trying to Solve?
* **What am I trying to solve?**: What are the key factors that influence life expectancy across different countries?
* **Big Analytical Question**: What factors are significant in determining life expectancy? 
* **More Questions**:
  * What factor has the greatest impact on life expectancy?
  * What factor has the least impact on life expectancy?

## Problem Statement: How Am I Going To Solve It?
* **Dependent Variable**:
  * Life Expectancy: The number of years a person is expected to live.
* **Independent Variables**:
  * Adult Morality
  * Alcohol Consumption
  * BMI (Body Mass Index)
  * Total Expenditure
  * Polio
  * Hepatitis B
  * Measles
* **Strategy**:
  * Create a multivariable regression model to estimate what key factors affect Life Expectancy across different countries.
 
## Data

**Cleaned Data**: 2938 Rows, 10 Columns, 7 independent variables, 1 dependent variable

* **Multivariable Regression**
* Dependent Variable - Life Expectancy
* Independent Variables- Adult Mortality, Alcohol Consumption, BMI (Body Mass Index), Total Expenditure, Polio, Hepatitis B, and Measles.
* I chose **eight** variables that I thought would be most significant in determining Life Expectancy.

## Definition of Variables
<img width="840" alt="image" src="https://github.com/aashnadorwal/Life-Expectancy-Linear-Regression/assets/122498175/ead21df4-6b2d-4a81-ad65-c06d6cc17fb0">

## Methodology: Data Preparation
* Exported the data from Kaggle to an Excel file
  * Moved ‘Year’ to inside column for easier analysis
* Removed unnecessary data and chose 8 variables I thought were most significant.
  * Removed: Status, Infant Death, HIV/AIDS, Diphtheria, Income and Schooling
 
<img width="623" alt="image" src="https://github.com/aashnadorwal/Life-Expectancy-Linear-Regression/assets/122498175/4bcb674f-b3d6-4fe9-9dcd-3db80edc2acb">


## Methodology: Multicollinearity

<img width="884" alt="image" src="https://github.com/aashnadorwal/Life-Expectancy-Linear-Regression/assets/122498175/d5f3f279-9cad-4447-902d-92a55110a3ec">

## Methodology: Removing High P-Values
* I removed the following variables because their P-Values were greater than alpha of 0.05:
  * Measles
  * Total Expenditure
  * Polio
  * Hepatitis B
  * BMI

<img width="504" alt="image" src="https://github.com/aashnadorwal/Life-Expectancy-Linear-Regression/assets/122498175/8412f83b-1e51-40d1-a241-2b2b04926e55">
<img width="504" alt="image" src="https://github.com/aashnadorwal/Life-Expectancy-Linear-Regression/assets/122498175/5ad1f868-0eb7-4e61-b61b-8e3d43dacd7b">


## Final Parsimonious Model

<img width="612" alt="image" src="https://github.com/aashnadorwal/Life-Expectancy-Linear-Regression/assets/122498175/a777df2c-9b4e-4466-bb47-082757dddcc3">

## Final Regression Equation

<img width="550" alt="image" src="https://github.com/aashnadorwal/Life-Expectancy-Linear-Regression/assets/122498175/9e331f57-da64-4a4f-a706-ec80b979e171">

## Residual Plots

<img width="391" alt="image" src="https://github.com/aashnadorwal/Life-Expectancy-Linear-Regression/assets/122498175/5f265207-4c47-41ac-b31b-c5a1e0525e86">

## Conclusion and Application

The most significant variables would be **Adult morality** and **Alcohol** because of their low P-values.  With a coefficient of  -.048, it suggests that life expectancy tends to increase when adult morality decreases.  On the contrary, the data suggest that with an increase in alcohol consumption, life expectancy increases. We know this to not be the case due to our knowledge of alcohol on human health.  I have concluded that additional data would be necessary to develop a more accurate data.

## Dataset Source
https://www.kaggle.com/datasets/vikramamin/life-expectancy-who















