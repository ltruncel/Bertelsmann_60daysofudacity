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


## Christmas Day - 12.25.20 


:cherry_blossom: I decided to take a day off on Christmas Day which was OK according to the challenge rules [here](https://sites.google.com/udacity.com/bertelsmann-tech-scholarship/community/60-days-of-udacity). :christmas_tree: <br>


## Day 16 - 12.26.20

:cherry_blossom: Today I continued with the practice project. <br>

:cherry_blossom: Several new tools are worth noting:

- Score Tool: This is a tool that determines the quality of the prediction model. We can use it to create scores for a model, which estimates the accuracy of the value predicted by the model. See more info about the score tool [here](https://help.alteryx.com/2018.2/Score.htm). Below is a screenshot of me practice using the score tool, which shows how it is connected to the data icon and the linear regression icon: <br>

![D16_score_tool](/images/D16_score_tool.png) <br>

- Formula Tool: This tool is similar to the formulas you would use in a spreadsheet application. You can learn more about how this tool is used in Alteryx [here](https://help.alteryx.com/11.0/Reference/Functions.htm). <br>


## Day 17 - 12.27.20

:cherry_blossom: I learned about ways to fix errors in Alteryx.  One of the tools to use is the **Select Tool**, which allows you to inspect the data type and fix any potential errors. <br>

![D17_select_tool](/images/D17_select_tool.png) <br>

:cherry_blossom: Another common Alteryx error is the null value. To fix this, add a **Field Summary Tool** before the data enter another tool.  This way you'll be able to see the missing values. Another tool is the **Filter Tool**, which you can use to single out those null values and fix them. Alternatively, you can use the **Imputation Tool**, where you can replace the null values with average or other values. Lastly, the **Data Cleansing Tool** will replace the null values with blanks (for string fields) or 0 (for numeric fields). <br>

![D17_other_tools](/images/D17_other_tools.png) <br>


## Day 18 - 12.28.20

:cherry_blossom: Today I worked on the practice project.  The goal of the project is to use a large database of diamond prices to build a model and predict the price of a diamond based on its attributes, which will be the basis for making recommendations to a jewelry company to decide how much it should bid on the diamonds. <br>

:cherry_blossom: In the process of working on this project, I learned about the new [Alteryx Multi-threaded Processing (AMP)](https://help.alteryx.com/current/designer/alteryx-amp-engine).  AMP is a multi-threaded concept of processing your data in parallel packets.  It allows for faster processing of large volumes of data while maintaining efficient use of resources.

## Day 19 - 12.29.20

:cherry_blossom: I continued to work on the practice project in Lesson 4. In the process I read about the [select tool](https://help.alteryx.com/current/designer/dynamic-select-tool).  I try to resist the temptation of looking at the solution.  I also learned more about [configuration connection](https://help.alteryx.com/current/designer/connection-configuration). :smile:

:cherry_blossom: The features of machine learning in Alteryx caught my eye and I basically spent the rest of my time here: https://help.alteryx.com/current/designer/machine-learning


## Day 20 - 12.30.20

:cherry_blossom: I continued with the practice project.  In the process, I read about [The Scatterplot Tool](https://help.alteryx.com/current/designer/scatterplot-tool).

:cherry_blossom: I read an article about [linear regression for data science](https://towardsdatascience.com/an-introduction-to-linear-regression-for-data-science-9056bbcdf675).

:cherry_blossom: I also read a review about [AI in 2020](https://medium.com/towards-artificial-intelligence/2020-a-year-full-of-amazing-ai-papers-a-review-c42fa07aff4b) which is fitting for end of the yaer. :smiley:


## Day 21 - 12.31.20

:cherry_blossom: Still working on the practice project.  I created a scatterplot to see the initial relations between the carat and price.  As you can see, there are other factors in addition to weight that determine the price of a diamond. I then used the linear regression tool and added all the variables to predict the price.<br>

![D21_scatterplot](/images/D21_scatterplot.png) <br>

:cherry_blossom: Happy New Year! :fireworks:

## Day 22 - 1.1.21

:cherry_blossom: Late post. I did the challenge yesterday but didn't get to post due to a medical emergency.  I tested out different predictive variables and looked at the results.

![D22_scatterplot](/images/D22_test_sample.png) <br>

## Day 23 - 1.2.21

:cherry_blossom: I wrapped up with the practice project and went through the sample solution walkthrough.  The steps to solve this problem are as follows: 
- Bring in the diamond data with an input tool. (Use the select tool to check the relations between carat and price, if preferred.)
- Add the linear regression tool. Select price as the target variable and the remaining factors as predictive variables.
- Check the p-values of predictive variables.  Disregard those that are not statistically significant. We want those with p-values that are <0.05.
- Look at the adjusted R-squared. It's above 0.9 so it's good. (See my Day 5 and Day 8 posts for more info about R-squared.)
- Apply our model to the batch of 3,000 to make a prediction and recommendation.
- Use the score tool and bring in the new_diamonds data set.
- Bring in a summarize tool to add all the predicted prices together. This gives us an estimate of the total retail value of the batch of 3,000 diamonds.
- Come up with a bid price by multiplying 0.7 to the estimate of the total retail value of the batch of 3,000 diamonds. Thus we've completed the project.  


## Day 24 - 1.3.21

:cherry_blossom: I ran the practice project again, with a cleaner connection:

![D24_practice_final](/images/D24_practice_final.png)

Here is a scatterplot for carat vs score. As you can see, the relation is now tighter:

![D24_practice_final](/images/D24_carat_score.png)

:cherry_blossom: I began working on the optional project: predicting catalog demand. :blush: <br>


## Day 25 - 1.4.21

:cherry_blossom: I continued to work on the optional project.  Today I had a more comprehensive idea about how to tackle this problem.  To begin, the goal of the project is to predict how much money a company can expect to earn from sending out a catalog to new customers. To solve this problem, I would build a linear regression model and apply the results to this business problem. <br> 

:cherry_blossom: The steps to take in order to solve the problems are as follows:
- understand the business problem and the data available
- analysis, modeling and validation
- writeup

I've downloaded and reviewed the data. More to go tomorrow.

:cherry_blossom: I also read an article and learned more about [Tableau](https://medium.com/@priyankabhagat6392/getting-started-with-tableau-data-science-and-data-visualization-7c9e2af9e9ef).


## Day 26 - 1.5.21

:cherry_blossom: I loaded the data into Alteryx and further examined the data. I also reviewed the project [rubric](https://review.udacity.com/#!/rubrics/186/view) today. 

:cherry_blossom: I read a helpful article about [creating a portfolio for data science jobs](https://www.dataquest.io/blog/career-guide-data-science-projects-portfolio?utm_source=Iterable&utm_medium=email&utm_campaign=10-days-of-data-6).


## Day 27 - 1.6.21

:cherry_blossom: Today I continued to work on the optional problem.  Here are more details about the problem that I looked into further:
- The costs of printing and distributing is $6.50 per catalog.
- The average gross margin on all products sold through the catalog is 50%.
- In p1-mailinglist.xlsx, there are two additional variables:
  - Score_No: The probability that the customer WILL NOT respond to the catalog and not make a purchase.
  - Score_Yes: The probability that the customer WILL respond to the catalog and make a purchase.

:cherry_blossom: I used the select tool and the scatterplot tool to see the relations between several variables.

## Day 28 - 1.7.21

:cherry_blossom: I began today's session by reviewing the Score Tool(https://help.alteryx.com/current/designer/score-tool).  

:cherry_blossom: I learned more about data investigation using the association analysis tool with this [tutorial](https://www.youtube.com/watch?v=7AvidkIPcbY).

:cherry_blossom: All of these are steps I take in order to further understand the business problem and to further learn about the tools I can use to solve the problem. :smiley: 


## Day 29 - 1.8.21

:cherry_blossom: I took a detour today and checked out the course: [Data Scientist in Python](https://www.dataquest.io/path/data-scientist/).  It was fun to review some of the basics in Python.  I look forward to the later units where python intersects with data science.



## Day 30 - 1.9.21

:cherry_blossom: I continued to work on the catalog demand project.  I looked into relations between a few predictive variables that I believe might affect the target variable (average sales amount) by using the scatterplot tool.  Here are a few samples:

![D30_years_as_customer](/images/D30_years_as_customer.png) 

![D30_avg_no_products_purchased](/images/D30_avg_no_products_purchased.png) 


:cherry_blossom: I also attended an informative seminar about building a Flask App using Database. :smiley:


## Day 31 - 1.10.21

:cherry_blossom: Still working on the catalog demand prediction project.  Today I looked into store number and zip code as potential predictive variables.  Zip codes seem to play a role in predicting the average sales amount while store number doesn't appear to have a big influence on the sales amount.

![D31_zip](/images/D31_zip.png) 


![D31_store_no](/images/D31_store_no.png) 

:cherry_blossom: I also plugged in the linear regression tool to look into the reports. 

![D31_progress](/images/D31_progress.png) 


## Day 32 - 1.11.21

:cherry_blossom: Today I looked into the results of the linear regression model.  As I look into p-value to determine the relevance of various predictive variables, I read [this article](https://www.simplypsychology.org/p-value.html).

:cherry_blossom: As shown from the report, customer segment and average number of product purchased are statistically significant (p-value <0.05) while other factors (zip code, store number, and number of years as a customer) are not.  I'll revise my initial hypothesis and my model accordingly.

![D32_linear_regression_report](/images/D32_linear_regression_report.png)



## Day 33 - 1.12.21

:cherry_blossom: Today I went back to the [Data Scientist in Python course](https://www.dataquest.io/path/data-scientist/). 

:cherry_blossom: I also I read a long report by [Google AI](https://ai.googleblog.com/2021/01/google-research-looking-back-at-2020.html). It's long but I highly recommend it.  


## Day 34 - 1.13.21

:cherry_blossom: I attended a virtual webinar at the AWS re:invent and learned how Tableau and AWS address analytics infrastructure challenges, and had a behind-the-scenes look at Tableau Public architecture on AWS, including how Tableau and AWS support surges in traffic, and how to securely scale Tableau deployment in the cloud.

![D34_tableau](/images/D34_tableau.png)

:cherry_blossom: I continued to work on the catalog demand prediction project. 


## Day 35 - 1.14.21

:cherry_blossom: I continued with the model and changed predictive variables for the regression model.  The updated model has a much better p-value overall. 

![D35_updated_model](/images/D35_updated_model.png)

:cherry_blossom: I completed another webinar by AWS and learned how to prototype, build, and delivery analytics with Dataiku DSS on AWS.


![D35_aws_dataiku](/images/D35_aws_dataiku.png)


## Day 36 - 1.15.21

:cherry_blossom: Today I cleaned up the model and all predictive variables look to have good p-values. The adjusted R squared is good too (0.8366).

![D36_final_model](/images/D36_final_model.png)

:cherry_blossom: I also learned to create [visualization for function optimization in Python](https://machinelearningmastery.com/visualization-for-function-optimization-in-python/). The purpose of visualization is that by observing lower-dimensional functions and algorithm behavior it can help us to develop the intuitions that can carry over to more complex higher-dimensional function optimization problems down the road.  Along the way I also looked at the [mplot3d tutorial](https://matplotlib.org/mpl_toolkits/mplot3d/tutorial.html#mpl_toolkits.mplot3d.Axes3D.plot_surface). 3D plots are super cool!



## Day 37 - 1.16.21

:cherry_blossom: I completed the  of the remainder of the catalog demand prediction project.  The linear regression I arrived at is 

Y = 303.46 + (-149.36 * Loyalty_Club_Only) + (281.84 * Loyalty_Club_And_Credit_Card) + (-245.42 * Store_Mailing_List) + (66.98 * Avg_Num_Products_Purchased) + (0 * Credit_Card_Only) 

I then used the score tool to validate the model to make sure that this works with the other dataset that we were provided with.  (I read this post about the [score tool](https://community.alteryx.com/t5/Alteryx-Designer-Knowledge-Base/Tool-Mastery-Score/ta-p/179436) along the way which is helpful.)

:cherry_blossom: I also learned techniques to [write unbreakable python](https://jessewarden.com/2020/03/write-unbreakable-python.html?utm_medium=email&utm_source=topic+optin&utm_campaign=awareness&utm_content=20200328+prog+nl&utm_medium=email&utm_source=topic+optin&utm_campaign=awareness&utm_content=20210116+prog+nl&mkt_tok=eyJpIjoiWkRBNU9EZGhZamt3TkRsbSIsInQiOiJyNWdoMzVZWnNXZFpMclpGZ3lLcGV4WDR0N2V1S2pqa3I2YmNweWdiUUlISFRicGQ3b044Q0R5NmV1ZUswTjhZa3o1TFk2U1pqUitXZXRBTmJlRWFxWjl4eW56XC9sUE5wKzRndjV2TDlTemFPYzY3K0JBa2UrUXYrdkxGaG9DUjgifQ%3D%3D).  Here “never break” means the function will always work, will always return a value, won’t ever raise an Exception, nor will it ever exit the Python process. These techniques help with writing Python with no runtime exceptions and therefore does what it’s supposed to do. 


## Day 38 - 1.17.21

:cherry_blossom: I learned about the [formula tool](https://help.alteryx.com/current/designer/formula-tool) today.  I also learned about various [functions](https://help.alteryx.com/current/designer/functions) in Alteryx.

:cherry_blossom: I worked on the final portion of the catalog demand prediction project. :smiley:


## Day 39 - 1.18.21

:cherry_blossom: I learned the basics of using [Snowflake](https://www.snowflake.com/wp-content/uploads/2020/06/Test-Driving-Snowflake.pdf).  I'm looking forward to learning more about this cloud data platform tomorrow. 

:cherry_blossom: I began working on a project to optimize an ML pipeline. The first step is to use a python train script and create a dataset which will then be evaluated with logistic regression from scikit learn.


![D39_optimizing_ml_pipeline](/images/D39_optimizing_ml_pipeline.png)

*Image credit: Udacity Machine Learning Engineer with Microsoft Azure Nanodegree Program*



## Day 40 - 1.19.21

:cherry_blossom: I came across this wonderful site [Bookdown](https://bookdown.org/) which provides info regarding bookdown, an open-source R package that facilitates writing books and long-form articles/reports with R Markdown. 

:cherry_blossom: I then explored [text minding with R](https://github.com/dgrtwo/tidy-text-mining/blob/master/index.Rmd) and went through one of the case studies of [mining NASA emtadata](https://www.tidytextmining.com/nasa.html).


## Day 41 - 1.20.21

:cherry_blossom: I wrapped up the final steps of the catalog demand prediction project and thus concluded my foundations course. :celebrate: I'll plan to review it in the coming days.

:cherry_blossom: I learned about [master data](https://www.youtube.com/watch?v=KUX6DDlrtF8). 


## Day 42 - 1.21.21

:cherry_blossom: I looked at [the stack that Medium is using](https://stackshare.io/medium/the-stack-that-helped-medium-scale-to-2-6-millennia-of-reading-time).  It uses [DynamoDB](https://stackshare.io/amazon-dynamodb) for its primary datastore and [Redis](https://stackshare.io/redis) cache cluster sitting in front of Dynamo to avoid hotkey issues.  I then read more about the hotkey issues [here](https://medium.engineering/how-medium-detects-hotspots-in-dynamodb-using-elasticsearch-logstash-and-kibana-aaa3d6632cfd
).

:cherry_blossom: I continue to work on the machine learning pipeline optimization project. 



## Day 43 - 1.22.21

:cherry_blossom: I'm still working on the pipeline optimization project.  

:cherry_blossom: Along the way I reviewed helpful concepts such as [uniform distribution](http://cplusplus.com/reference/random/uniform_real_distribution/).  I also reviewed plotting for [Matplotlib](https://scipy-lectures.org/intro/matplotlib/index.html).


## Day 44 - 1.23.21

:cherry_blossom: It was a busy, but wonderful day of learning because of the Study Jam.  I participated in an informative seminar about SQL.

![D44_intro_to_sql](/images/D44_intro_to_sql.png)

:cherry_blossom: In the afternoon, I attended yet another helpful seminar about data literacy.  I also [wrote a post about this on Linkedin](https://www.linkedin.com/embed/feed/update/urn:li:share:6758906909673197568).

![D44_data_literacy_seminar](/images/D44_data_literacy_seminar.png)


## Day 45 - 1.24.21

:cherry_blossom: I reviewed materials from the Study Jam.  I also continued to work on the machine learning pipeline optimization project. 

:cherry_blossom: I read an interesting article about [choosing C Hyperparameter for SVM Classifiers with Scikit-Learn](https://queirozf.com/entries/choosing-c-hyperparameter-for-svm-classifiers-examples-with-scikit-learn)


## Day 46 - 1.25.21

:cherry_blossom: It was a long day but I managed to get a little work done on the machine learning pipeline project.  

:cherry_blossom: I began learning more about SQL through this [SQL tutorial](https://www.youtube.com/watch?v=HXV3zeQKqGY&feature=emb_logo).


## Day 47 - 1.26.21

:cherry_blossom: I continued with SQL through this [SQL tutorial](https://www.youtube.com/watch?v=HXV3zeQKqGY&feature=emb_logo).

:cherry_blossom: I also learned about [setting up SQL server in Azure](https://www.daveondata.com/blog/sql-for-excel-users-part-1/).



## Day 48 - 1.27.21

:cherry_blossom: I returned to the machine learning pipeline project again today.  

:cherry_blossom: I also began the [Azure Data Fundamentals course](https://docs.microsoft.com/en-us/learn/modules/explore-core-data-concepts/2-identify-need-data-solutions).  The course begins with core concepts such as relational data and JSON, and then discusses common data processes:

![D48_data_process](/images/D48_data_process.png) <br>

*image credit: Azure Data Fundamentals*


## Day 49 - 1.28.21

:cherry_blossom: I continued to work on the machine learning pipeline project. It was slower than I had hoped but I tried to keep my spirit up and kept going. 


## Day 50 - 1.29.21

:cherry_blossom: I continued to work on the machine learning pipeline project.

:cherry_blossom: I had a look at [Django](https://www.thecoderpedia.com/blog/what-is-django/) and then learned the differences between Django and [Flask](https://www.thecoderpedia.com/blog/django-vs-flask/).
