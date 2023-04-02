
# Project Description

## Introduction

An online national clothing chain needs your help creating a targeted marketing campaign. Sales have been flat and they want to lure lost customers back. They want to advertise specific products to specific customers in specific locations, but they don’t know who to target. They have three products in mind:

- Shirt: $25
- Sweater: $100
- Leather Bag: $1,000
 
They need you to conduct an analysis to determine the best product to advertise to each customer.

## Project Environment and Data Sources

All work for the project will be completed using the Microsoft Power BI desktop application.

For viewing the raw spreadsheet data outside of that platform, students will need to use Google Sheets or Microsoft Excel.

The project will use a variety of data sources, including

#### US Census Bureau
- Average income
- location
- population
- industry
#### Business Data
- Product inventory
- Product prices
- Customer rating
- Product return rate
#### Customer Data
- Customer ID
- Names
- Location
- Date of birth
- Purchase history
#### Additional Data
- Weather
- Economics
- Demographics
- Competition

## Project Instructions

In this project, you will use population statistics from the US Census Bureau to determine where the greatest income exists around the country and whether there is a correlation between sales and income. We don’t know the incomes of our customers, but we should be able to predict it by looking at their purchase history and locations and comparing that against the census data. Additionally, we want to analyze our inventory, specifically customer ratings and return rate and see if there’s a correlation between the two.

## Draw conclusions

Draw conclusions from your analysis and use visuals to answer the following questions:

Analysis Questions:

1. What is the correlation (R2 value) between sales and income?
2. What is the correlation (R2 value) between customer ratings and product return rate?
3. What are the linear regression formulas to predict customer income from customer sales?
4. Which customer do you predict has the highest income?
5. Which product will be advertised the most?

## Present your analysis

You’ll need to present your analysis as a 1 page written summary and visual report in Power BI. Use the following visuals to present your data:

- Income Distribution: Histogram
- Household Income by Location: Map
- Correlations: Scatter Plot with Trendline and Card with R^2 value

Use other visuals as-needed to further present the results of your analysis.

## Detailed Instructions 

1. Import the census data, customer list, purchase list, and state list into Power BI. You’ll use the “Get Data” button to start the import process. Make sure you select each of the available tables within each Excel file. There should be 7 total tables:
- Avg Income by State
- Customer List
- Incomes by State
- Industries
- Product Inventory
- Purchase List
- State List
2. Set up the data in Power Query so that all the columns are correctly formatted and structured. Some of the tables will require steps in Power Query to be correctly set up.
3. Set up your table relationships. All tables you import should be tied into the table relationships (if possible). Avoid many-to-many relationships as they’re not needed and will cause issues with cross-filtering.
4. Review the table relationships and confirm if they are properly set up. Most of the tables should follow a star schema and the overall set up should look similar to the sample image:
5. Create a map to visualize the distribution of average household income across the country.

6. Create a new ‘Regression Table’ from the ‘Customer List’ to summarize the average customer sales by state and set up the following calculated columns for your regression formula:

- y = average sales by state (read the note below)
- y2 = Y^2
- x = average income by state (read the note below)
- x2 = X^2
- xy = X*Y
NOTE: You'll need to use this data to calculate predicted customer incomes, and this can be set up in 1 of 2 ways. Either (1) set up income as x and use x = b-y/-m to predict customer income, or (2) set up sales as x and use y = mx +b to predict customer income. The results will be very similar.

7. Create a scatterplot with a trendline to analyze the relationship between average incomes and average sales.

8. Create the remainder of the regression formula variables as calculated measures: b (y-intercept), m (slope), n, Sum of X, Sum of Y, Sum of XY, Sum of X2, Sum of Y2

9. Create a calculated column in your customer table for your predicted customer incomes.

10. Use DAX formulas to categorize the predicted incomes into ranges and to determine the best product fit for each customer. Present this data with a histogram and other visuals.

11. Perform additional analysis using 1-2 other variables of your choosing. These variables can be part of the provided data set or data that you find from additional sources. Think about variables that may help you better understand the customer demographics and market conditions and that will allow creating a more rigorous analysis.

12. Write a brief 1 page summary of your findings, citing the visuals and tables you created as evidence. The summary should address the 5 analysis questions described. 

# My Project

## Market Analysis Report for National Clothing Company

### Understanding the Data

To begin analyzing the data, I had to format, clean, and merge multiple excel datasets such as census data, customer list, purchase list, and state list using Power Query. This allowed me to create tables and establish relationships between them.

Next, I utilized linear regression to determine the relationship between the independent variable x and the dependent variable y. Specifically, I wanted to examine the correlation between customer income and sales, as well as the correlation between ratings and return rate. To gauge the strength of these relationships, I calculated the coefficient of determination (R^2), which ranges from 0 to 1. 

### Summary Report

We have been responsible for developing a targeted marketing campaign to attract customers back to the online national clothing chain companies, which have experienced stagnant sales. Our strategy involves advertising particular products to specific customers in specific locations. The products we have been assigned to promote and sell include a Shirt priced at $25, a Sweater priced at $100, and a leather bag priced at $1000. To achieve our objective, we must answer a set of questions and draw appropriate conclusions.

1. What is the correlation (R2 value) between sales and income?

![Correlation between Income and Sales](https://github.com/ziwalon/Udacity-Data-Analysis-Visualization-with-Microsoft-Power-BI/blob/main/Project-3-Market-Analysis-for-National-Clothing-Company/Screenshots/1-Correlation-Income-and-Sales.png)

- The scatterplot illustrates a strong positive correlation between income and sales. As customers' income increases, the sales of products also increase. Therefore, income significantly influences the sales of products. With a coefficient of determination of 0.78, we can confidently conclude that there is a robust relationship between these two variables.

2. What is the correlation (R2 value) between customer ratings and product return rate?

![Correlation between Rating and Return Rate](https://github.com/ziwalon/Udacity-Data-Analysis-Visualization-with-Microsoft-Power-BI/blob/main/Project-3-Market-Analysis-for-National-Clothing-Company/Screenshots/2-Correlation-Rating-and-ReturnRate.png)

- The scatterplot depicts a noticeable negative correlation between the customer rating and return rate. A higher customer rating is linked with a lower return rate, suggesting that satisfied customers with higher ratings are less likely to return the product. The coefficient of determination, which is 0.69, confirms that there is a moderate association between the two variables.

3.	What are the linear regression formulas to predict customer income from customer sales? 

- By utilizing the inverse of the regression formula **`(X = b - Y / -m)`** we can estimate our customers' income based on their purchase history for the last six months.

4.	Which Customer do you predict has the highest income?

![Highest Predicted Income](https://github.com/ziwalon/Udacity-Data-Analysis-Visualization-with-Microsoft-Power-BI/blob/main/Project-3-Market-Analysis-for-National-Clothing-Company/Screenshots/4-Highest-Predicted-Income.png)

- According to the data, Jon Little from Illinois is the customer with the highest income, with a predicted income of $558,143.93. In addition, over the past six months, Jon Little also had the highest purchase amount of $5,250.

5.	Which product will be advertised the most? 

![Product Recommendations](https://github.com/ziwalon/Udacity-Data-Analysis-Visualization-with-Microsoft-Power-BI/blob/main/Project-3-Market-Analysis-for-National-Clothing-Company/Screenshots/5.1-Product-Recommendations.png)

![Product Recommendations](https://github.com/ziwalon/Udacity-Data-Analysis-Visualization-with-Microsoft-Power-BI/blob/main/Project-3-Market-Analysis-for-National-Clothing-Company/Screenshots/5.2-Product-Recommendations.png)

- After analyzing the purchase history and predicted income of the currently available list of customers, I suggest the following product recommendations: a sweater for approximately 50.7% of existing customers, which translates to 507 customers, a shirt for about 31.9% of customers, which is 319 customers, and a leather bag for approximately 17.4% of customers, which is 174 customers.

### Visual Report

![Sales and Income Report](https://github.com/ziwalon/Udacity-Data-Analysis-Visualization-with-Microsoft-Power-BI/blob/main/Project-3-Market-Analysis-for-National-Clothing-Company/Screenshots/Sales&Income-Report.png)

![Product Insights](https://github.com/ziwalon/Udacity-Data-Analysis-Visualization-with-Microsoft-Power-BI/blob/main/Project-3-Market-Analysis-for-National-Clothing-Company/Screenshots/ProductInsights-Report.png)

![Product Recommendations](https://github.com/ziwalon/Udacity-Data-Analysis-Visualization-with-Microsoft-Power-BI/blob/main/Project-3-Market-Analysis-for-National-Clothing-Company/Screenshots/Product-Recommendations.png)
