This repository contains a data-driven analysis project aimed at identifying the most efficient sales strategy for a new office stationery product line. The business tested three approaches: Email, Call, and a combination of both (Email + Call), and this project analyzes the performance of each method in terms of revenue generated and effort required. The dataset has 15000 rows and 8 columns.

## *The Jupyter Notebook 'Written Report' contains all the information and descriptions of what was done and discovered in each step.*

# Project Overview:


**Objective**: To determine which sales method yields the highest revenue and optimize resource allocation for future campaigns.
    
**Data Source**: Customer sales data over a 6-week campaign period, with variables including sales method, revenue, customer engagement, and more. Provided by Datacamp.


## Technologies Used:


    Language: Python
    Python Libraries:
    Pandas: Used for data cleaning, manipulation and analysis
    Matplotlib & Seaborn: Used for visualizations.
    Jupyter Notebook: Used or interactive data exploration.

## Project Structure:


**product_sales**: Contains the dataset used for analysis.
    
**Written Report**: Jupyter notebook with step-by-step data cleaning, analysis, and visualizations.
    
**Presentation**: A presentation and overview of the project.

## Key Features:

**Data Cleaning and Validation**: Handling missing values and correcting inconsistencies.
    
**Exploratory Data Analysis (EDA)**: Visualizations that reveal revenue trends across different methods.
    
**Business Metric Definition**: Calculation of key performance indicators like revenue per customer and strategy efficiency.
    
**Actionable Recommendations**: Insights into which sales approach the business should continue using to maximize revenue with minimal effort.

## Key Insights:

**Total Customers For Each Sales Method:**

The Email sales method was the method to reach the most customers, with 7465 customers in total, approximately 50% of all 14998 customers. The Call method comes in second place with 4961 customers, 33% of all customers. And in third is the Email + Call method which had 2572 customer, 17% of the total. Taking in consideration that the email method is the easiest and most time effective method to perform, it's easy to comprehend its performance in reaching considerably more customers than the other methods.

![Image](https://github.com/user-attachments/assets/72e60729-116e-4fb6-87b6-805460be8035)

**Distribution of Revenue:**

The distribution of revenue is not a normal distribution, being skewed to the right due to having an average of 95.56, lots of values above the 75th percentile and a high max value.

![Image](https://github.com/user-attachments/assets/91f8684d-2fc8-4e06-9ca3-8968b44bb025)

![Image](https://github.com/user-attachments/assets/a088d2eb-d7e3-4a48-9a0f-9dc1fdaced69)

**Overall Units Sold Spread**

In the data of number of units sold, we have a minimum of 7, an average of 10, and a maximum of 16 units sold. The majority of values are found inside the IQR, having only few outliers being above the 75% percentile.

![Image](https://github.com/user-attachments/assets/2cdc69b6-fd85-407d-abc7-077030b206a2)

**Revenue Spread for Each Sales Method**

What we can see by looking at the average revenues of each method is that the one with the least sales, Email + Call, had the best average revenue overall with an average of 183.7 (almost twice as much as the second place), beating the other methods, Email with an average of 97, and Call with an average of 47.6. However, we can see that the total revenue of the Email method is highr than the sum of the other 2 methods combined! The numbers are: Email with a total of 724216.13, Email + Call with 472730.95, and at last, Call with a total of 236391.07 revenue. For the Email method, we have a minimum revenue of 78.83, and average of 97, and a maximum of 148.97. For the Email + Call we have a minimum revenue of 122.11, an average of 183.8, and a maximum of 238.32. And for the Call method, we have a minimum of 32.54, an average of 47.6, and a maximum of 71.36 revenue.

![Image](https://github.com/user-attachments/assets/7a0a45b2-7597-4b79-b83b-6b9eca5e9268)

**Trend Difference in Revenue Over Time for Each Sales Method**

As we look through the data of revenue over time for each sales method, we can see that the Email + Call and Call methods have had consistently increased growth in revenue throughout the weeks, Email + Call with an average increase of +49.3%, Call with +6.8%, different than the Email method, which has seen an average decrease of – 31.8%. In the last week, all methods had a decrease in growth of revenue acquired, with the Email method having the biggest decrease of 68.5%, followed by Call with a decrease of 47%, and Email + Call, with the least decrease in growth of 12.6%. Overall, the Email + Call method has grown the most, but still, with lower total revenue numbers than the Email method, except in the last 2 weeks when the Email + Call method got higher revenue numbers than the Email method.

![Image](https://github.com/user-attachments/assets/af1055c3-d22c-4ebd-9bd0-2a918a69ebf4)

**Trend of Customer Amount and Percentage Change Over Time by Sales Method**

When we look at the change in number of customers over time, we can see that the Email + Call method had the best growth in number of customers between the 3 methods, with an average growth of +37.1%, followed by the Call method with a decrease in growth of -4.7%, and then the Email method with an average decrease in growth of -36.1%. The decrease in revenue growth in the last week that was seen in the other graph can be explained by the decrease in customer growth for each method.

![Image](https://github.com/user-attachments/assets/e4ebfd24-e05d-4a4c-a8f3-d3221e8da4ed)

**Creation of a business metric (revenue per hour of sales effort) to evaluate sales efficiency**

The business goal should be to maximize sales and revenue by maintaining the effort as low as possible so it increases its efficiency. Hence based on the sales strategies tested for the new line of office stationery, the business should focus on monitoring a key metric that reflects both revenue generation and the effort required by the sales team.

With that in mind, the proposed metric is revenue per hour of sales effort.

This metric accounts for the time spent on each sales approach (Email, Eall, Email + Call) and relates it to the revenue generated. By tracking this metric, the business can evaluate the efficiency of each method and optimize resource allocation based on the return generated from time spent by the team.

We can estimate the time spent on each sales strategy as follows:

•Email: Minimal time spent, let's assume 1 minute per customer.

•Call: 30 minutes per customer on average.

•Email + Call: 1 minute for the email + 10 minutes for the follow-up call.

Then we can calculate the revenue per hour of sales effort:

•Sum the total revenue for each method.

•Sum the total hours spent on each method.

Then the revenue per hour can be computed by dividing the total revenue by the total time spent in hours.

![Image](https://github.com/user-attachments/assets/a2c81ff9-9cb6-45d9-ae18-751dc86f0ea8)

With that, we can see that the Email method is the most efficient in generating revenue per sales effort, followed by Email + Call and, at last place, the call method which is the least effective method by far.

**Summary and Recommendations for prioritizing the most efficient strategies**

This analysis addresses the problem of creating the most revenue with as much efficiency as possible, by prioritizing the most efficient methods By comparing the performance of different sales methods (Email, Call, Email + Call), the business could benefit a lot in the long-term.

Based on the revenue per hour of sales effort metric and on the exploratory analysis, the most appropriate recomendation would be to keep the focus on the Email method which is the most time efficient and has generated the most revenue so far, while keeping track of increases in efficiency of the Email + Call method and diverting the efforts from the Call method to Email + Call, as the Call method compares very poorly to the other methods, demanding way too much time with not as much revenue in result.

Other recommendations to better improve and understand the data:

• Inconsistent values of the sales_method column should be corrected when collecting the data.

• Implement a strategy to identify the reasons as to why there are missing values corresponding to the revenue, and to fill those values if possible.

• More detailed information of the time spent reaching the customer could be gathered and included into a new column on the dataset.

• Create standardized templates of emails to be sent and include the types into a column on the dataset, so we could take a look at what template of email is the most efficient by A/B testing and other methods.

• Explore new methods of reaching out to new customers

• Gather more information about the period of time the client was approached and when the sale was made.

• Gather more information about the client, such as demographics and preferences.

The business could see a lot of improvements by implementing these strategies, as these strategies can increase the amount and quality of insights we can get from the data gathered.

**Estimation if the recommendations are applied**

By diverting the hours spent with the Call method equally between the other methods, the total change in revenue could reach an estimated increase of 707%.

## How This Project Helps:

This project helps the business optimize sales efforts, reduce unnecessary resource use, and improve decision-making by focusing on strategies that bring the highest returns based on real data.
