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

:cherry_blossom: I learned about Alteryx Designer: https://www.youtube.com/watch?v=8kUPNSBHCxo <br>


## Day 8 - 12.17.20 

:cherry_blossom: I learned more about special cases for multiple linear regression today: 
- For categorial variables, we can't really use a scatterplot or any other graph to see whether a linear relationship exists.  The best way to deal with this is to run the categorical variables through the regression model and see if the coefficients turn out to be significant with a high multiple-R-squared.  If there is a linear relationship, then the coefficients should be significant (0.7 or above). <br>
- As more variables are included, we should use the adjusted r-squared value. This is because the more variables that are included, the higher the r-squared value will be, even if there is no relationship between the additional variables and the target variable. Namely, this is an attempt to account for the phenomenon of the R2 automatically and spuriously increasing when extra explanatory variables are added to the model. See more info [here](https://en.wikipedia.org/wiki/Coefficient_of_determination#Adjusted_R2). <br>


## Day 9 - 12.18.20 

:cherry_blossom: I completed an exercie of multiple linear regression in Excel. :smile: <br>
![multiple_linear_regression_exercise](/images/D9_multiple_linear_regression_exercise.png) <br>

:cherry_blossom: For categorial variables, we DO NOT just assign ordinal numbers (like 1, 2, 3, 4) to each category because that would result in skewed results. A better way of using categorical variables in regression is to use **dummy variables** (0 or 1).  To represent n categories, we would need n-1 dummy variables. <br>

:cherry_blossom: I downloaded Alteryx but encountered challenges when trying to install it via Virtual Box onto my Mac. Will try again. <br>

:cherry_blossom: I read about free data science tools for Alteryx [here](https://community.alteryx.com/t5/Data-Science/Free-Data-Science-Tools-for-Designer-A-Gallery-Tour/ba-p/669590).


## Day 10 - 12.19.20 

:cherry_blossom: I spent a fair amount of time trying to figure out how to install Alteryx onto my Mac.  It turns out it's not enough to have a Virtual Box.  You would need to have Windows installed in the VirtualBox (or other VMs such as VMWare or Parallels).  I'm installing Windows 10 Development Environment from [here](https://developer.microsoft.com/en-us/windows/downloads/virtual-machines/). Hopefully this will work. <br>

:cherry_blossom: Alteryx is a data analytics tool with the ability to prep, blend, and analyze data using a repeatable workflow, then deploy and share analytics at scale. It allow analysts to:
- connect to and cleanse data from data warehouses, cloud applications, spreadsheets, and other sources;
- join data together;
- perform analytics (predictive, statistical and spatial). <br>

The interface looks like this:
![D10_alteryx_intro](/images/D10_alteryx_intro.gif) <br>

As you can see, several key panels include:
- The Tools (such as input data, output data...etc. You can drag them onto the canvas)
- The configuration panel (where you select the configurations you want for each tool)
- The Canvas (where you place and connect the tools.) <br>

:cherry_blossom: Inspired by fellow scholars, I began this [SQL tutorial](https://www.w3schools.com/sql/default.asp).


## Day 11 - 12.20.20 

:cherry_blossom: The installation challenge continues as I'm trying to install it on an external hard drive (my Mac HD is too small). It took me about 2 hours to download all requirements and install them. <br>

![D11_Windows_VM](/images/D11_Windows_VM.png)

:cherry_blossom: As it turns out, working in a Windows Environment via VirtualBox on an external drive is simply too slow. I started over again, using VMware and following [this instruction](https://www.youtube.com/watch?v=mtxtqw95484&feature=emb_logo). Thanks to fellow scholar Serkan for the tip! <br>

:cherry_blossom: While I'm waiting, I read a guide for [CRISP-DM: Cross-Industry Standard Process for Data Mining](https://medium.com/analytics-vidhya/a-beginners-guide-to-industry-standard-process-of-data-mining-crisp-dm-c1d7d50e57c3). (Thanks to fellow scholar Susy and Ebinbin for the recommendation!) The upshot is that we need to understand the business problem and the data before preparing and modeling it. After the models are generated, they need to be assessed and determine their effectiveness in solving the business problems. During deployment, the results are used to provide insights for informed business decisions. 

:cherry_blossom: At the end of this post I'm still waiting to download the Windows 10 disk image (an iso file) in order to finish the installaiton. There's more work later tonight. Wish me luck! 

## Day 12 - 12.21.20 

:cherry_blossom: I was finally able to install Alteryx onto my Mac (actually in a Windows environment via VMWare); I was overjoyed! <br>

:cherry_blossom: It was smooth sailing once I had Alteryx installed. I completed a tutorial, and the completed a sample workflow.

![D12_tutorial](/images/D12_tutorial.png) <br>

![D12_sample_workflow](/images/D12_sample_workflow.png) <br>

*source: Alteryx Tutorial* <br>

:cherry_blossom: Today is #MotivationMonday in our Slack community and we were encouraged to share what motivates us.  This is what I shared: <br>
*For me it’s a sense of purpose. My desire to help others and to make this world a better place is what keeps me going.* :fire: <br>

![D12_sample_workflow](/images/D12_maya_angelou.jpg) <br>
*source: Maya Angelou* <br>

## Day 13 - 12.22.20 

:cherry_blossom: Today I built my first model (a linear regression model) in Alteryx. :smile: <br>

![D13_1st_model](/images/D13_1st_model.png) <br>

:cherry_blossom: Today is TreatYourselfTuesday. I treated myself with a hot cup of lemon myrtle green tea.:relaxed::tea: <br>

![D13_treat_yourself_tuesday](/images/LT-treatyourselftuesday.jpeg) <br>

## Day 14 - 12.23.20 

:cherry_blossom: I completed an exercise on the regression model I worked on yesterday and also completed the remainder of the Lesson. :smiley: <br>

:cherry_blossom: To be able to successfully interpret a regression model, it's worth a refresher of statistics:

- P-value: A p-value is the probability that observed results (the coefficient estimate) occurred by chance.  The lower the p-value the higher the probability that a relationship exists between the predictor and target variable. When a predictor variable has a p-value < 0.05, the relationship between it and the target variable is considered to be statistically significant.<br> 

- R-Squared: It represents the amount of variation in the target variable explained by the variation in the predictor variables.  The higher the r-squared, the higher the explanatory power of the model. 


## Day 15 - 12.24.20 

:cherry_blossom: It's tough to get work done on Christmas Eve but I managed to review a playbook for [linear regression](https://d17h27t6h515a5.cloudfront.net/topher/2017/May/5915face_linear-regression-playbook/linear-regression-playbook.pdf). <br>

:cherry_blossom: I also began the practice project to predict diamond prices. <br>


12.25.20 Christmas Day

I took a day off which is allowed according to the challenge rules [here](https://sites.google.com/udacity.com/bertelsmann-tech-scholarship/community/60-days-of-udacity). <br>


## Day 16 - 12.26.20

:cherry_blossom: Today I continued with the practice project. <br>

:cherry_blossom: Several new tools are worth noting:

- Score Tool: This is a tool that determines the quality of the prediction model. We can use it to create scores for a model, which estimates the accuracy of the value predicted by the model. See more info about the score tool [here](https://help.alteryx.com/2018.2/Score.htm). Below is a screenshot of me practice using the score tool, which shows how it is conencted to the data icon and the linear regression icon: <br>

![D16_score_tool](/images/D16_score_tool.png) <br>

- Formula Tool: This tool is similar to the formulas you would use in a spreadsheet application. You can learn more about how this tool is used in Alteryx [here](https://help.alteryx.com/11.0/Reference/Functions.htm). <br>






