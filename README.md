# Bertelsmann 60 Days of Udacity Challenge 

### Greetigns from LauraT! This is a record of my 60-day learning challenge for the Bertelsmann Data Track Scholarship where I pledged to code and work through my Foundations course content for at least 30 minutes every day. I began on December 10, 2020. <br>

<i> Image Credits: Unless otherwise mentioned, images included in the challenges are from the Bertelsmann Tech Scholarship Challenge Course - Introduction to Problem Solving with Advanced Analytics Nanodegree Program by Udacity</i> <br>


![LT Scholarship Badge](/images/D0_Bertelsmann_Scholarship_LauraT.jpg)

## Day 1 - 12.10.20

:cherry_blossom: I made the pledge and reviewed lesson 1. Let's start! <br>

:cherry_blossom: The core of this lesson is the problem solving framework, which involves the understanding of business issues and data, data preparation, modeling, validation, and visualization. <br>

![The Problem Solving Framework](/images/D1_framework.png)<br>


## Day 2 - 12.11.20

:cherry_blossom: I completed the first half of Lesson 2. It began with the methodology map, which helps to determine the right methodology for a variety of business problems. <br>

:cherry_blossom: Non-Predictive Analysis has four categories: Geospatial, Segmentation, Aggregation, and Descriptive. <br>

:cherry_blossom: Predictive business problems can be data rich or data poor. <br>

:cherry_blossom: If there is not sufficient usable data to solve the problem, we'll need to set up an experiment to help us get the data we need, which is called the A/B Test. <br>

:cherry_blossom: There's more to it. Stay tuned for my updates tomorrow!

![Methodology Map](/images/D2_methodology_map.jpg)<br>

## Day 3 - 12.12.20

:cherry_blossom: Today I began with the data rich problems. There are two types of data-rich problems, numeric and non-numeric, depending on the desired outcomes.<br>  
  - Models predicting numeric outcomes are called regression models.
  - Models predicting non-numeric outcomes are classification models.<br>
  

:cherry_blossom: Numeric models can be continuous, time-based, or count: <br>

![Numeric Variables](/images/D3_numeric_variables.png)<br>

:cherry_blossom: Non-numeric models can be binary or non-binary.<br>

:cherry_blossom: I also completed the quizzes at the end of the lesson and thus concluded Lesson 2.


## Day 4 - 12.13.20 

:cherry_blossom: I began Lesson 3 by analyzing a business problem, where we need to determine whether we have enough capacity on the support team to handle the support tickets from the new customer, and if not, how many people we would need to add to reach the desired capacity.  The steps to analyze the problem are as follows: 

1. Is this a data rich, or data poor problem?
2. Should we use a numeric or classification model?
3. Is our target variable continuous or time-based? 

The answer to this problem is that we should use a continuous model.

:cherry_blossom: I also completed the unit about linear regression. 

![Linear Regression](/images/D4_linear_regression.png)



## Day 5 - 12.14.20 

:cherry_blossom: I continue to work on the unit about linear regression. We can use a simple Google sheet to calculate slope and interception to learn about the relation of x and y. To know whether the linear expression we calculated a good fit of our data, we use the correlation function CORREL(data_y, data_x) to calculate the correlation r between the target and predictor variable. The range of r is from -1 to +1. The closer r is to plus or minus 1, the higher the correlation between x and y. <br>

![Google Sheet](/images/D5_r_google_sheet.png)

:cherry_blossom: In addition to know how well the data fits our line. we would also want to know how good the formula is at approximating the data by calculating the coefficient of determination, or r-squared. R-squared is a coefficient between 0 and 1.
- closer to 1: nearly all variance in the target variable is explained by the model
- closer to 0: nearly none of the variance in the target variable is explained by the model.
- In general: above 0.7 are considered strong and below 0.3 are considered weak.

![R Squared](/images/D5_r_squared.png)

*more info on R-squared:*
(https://blog.minitab.com/blog/adventures-in-statistics-2/regression-analysis-how-do-i-interpret-r-squared-and-assess-the-goodness-of-fit)


## Day 6 - 12.15.20 

:cherry_blossom: More about linear regression today. R-squared can be easily calculated by the function RSQ(data_y, data_x) in Google Sheets:


![RSQ in Google Sheet](/images/D6_rsq_google_sheet.png)

:cherry_blossom: You can do the same in excel as well.  I completed a sample exercise using excel, as shown below:

![Excel Exercise](/images/D6_excel_exercise.png)

:cherry_blossom: The concept of multiple linear regression is the same, just with more independent variables. 
  
![Multiple Linear Regression](/images/D6_multiple_linear_regression.png)

:cherry_blossom: I also read about extracting data from a database using SQL: https://medium.com/swlh/searching-through-a-database-52eaaf64f89c


## Day 7 - 12.16.20 

:cherry_blossom: Today the focus is on steps for performing multiple linear regression in Excel. <br>

:cherry_blossom: The first step is to prepare and understand your data. Given any data set, we need to make sure that the data is clean and not biased. <br>

:cherry_blossom: Using the same example, we'll use the Number of Employees and Value of Contract to initially build our multiple linear regression model. <br>

:cherry_blossom: The steps to do this in Excel are as follows: <br>

- Install Analysis ToolPak Add-In. <br> 
- In Excel, select Data Analysis. Select Regression in the Pop-up window and select OK.
- The Y range is the target variable (Average Number of Tickets). The Input X Range should be the range of data of your predictor variables (the Number of Employees AND the Value of the Contract).  The reason we are selecting both is that they each show potential to have a linear relationship between the Average Number of Tickets.

:cherry_blossom: Click OK to run the model and see the results. We can quickly see our coefficients of the linear equation.


