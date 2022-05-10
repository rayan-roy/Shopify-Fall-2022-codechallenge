# Shopify Fall 2022 coding challenge

This repo contains my solution for the Fall 2022 Data Science Challenge from Shopify

Refer to the [link](https://github.com/rayan-roy/Shopify-Fall-2022-codechallenge/blob/main/Shopify_data_challenge_Fall_2022_solution.ipynb) to see the code and analysis in ipynb file.

A summary of the problem along with the solution is first provided followed by a detailed explanation of the average order value (AOV) investigation. The SQL solution is at the bottom of the python file with detailed analysis.

A brief solution is as follows:

**Think about what could be going wrong with our calculation. Think about a better way to evaluate this data.**

The orignal Average Order Value (AOV) was calculated by averaging the order_amount which led to a huge number of $3145.13. This is because the average (mean) is sensitive to outliers (extreme values). This was further confirmed by the high variance which indicates large variability between order amounts. 

**What metric would you report for this dataset?**

A better way is using median or average after removing outliers.

**What is its value?**

If we use the median as an estimate, then the AOV is $284.0. If we remove the outliers and calculate AOV, we get $300.15.

### SQL Solutions
**How many orders were shipped by Speedy Express in total?**

There were **54** orders that were shipped by Speedy Express

**What is the last name of the employee with the most orders?**

The last name of the employees with most orders is **Peacock** with 40 orders

**What product was ordered the most by customers in Germany?**

The product that most ordered by customers in Germany is **'Boston Crab Meat'**
