PROJECT NO 1
 Sales Data Analysis Using NumPy Array Operations

 1. Introduction

In today’s world, businesses use data to understand how well they are performing. Sales data helps companies know how much they are earning, what customers are buying, and which products are selling more.

In this project, we analyzed a Supermarket Sales dataset using Python and the NumPy library. NumPy helps us perform fast numerical calculations using arrays. By using NumPy operations like indexing, slicing, statistical functions, broadcasting, and vectorized computation, we can easily study and understand sales data.


2. Problem Statement

The aim of this project is to analyze a real supermarket sales dataset using NumPy.

We use NumPy functions to calculate total sales, average sales, profit, and other statistical values. The goal is to understand sales performance and business trends using numerical analysis.



3. Dataset Description

The dataset includes the following details:
* Product Category
* Quantity Sold
* Unit Price
* Sales Amount
* Unit Cost
* Profit / Gross Income
* Product ID
* Sale Date
* Sales Representative
* Region
* Customer Type
* Discount
* Payment Method
* Sales Channel

These details help us understand revenue, profit, and sales performance.


4. Project Objectives

The main objectives of this project are:

* To load the sales dataset and convert important columns into NumPy arrays.
* To calculate total and average sales.
* To use indexing and slicing to view specific data.
* To calculate statistical values like mean, median, variance, and standard deviation.
* To calculate revenue using broadcasting.
* To calculate profit using vectorized operations.
* To understand sales trends using the results.


5. Data Loading and Preparation

The dataset was loaded using Pandas, and important columns were converted into NumPy arrays.

Example:

product_category = data["Product_Category"].values  
quantity = data["Quantity_Sold"].values  
unit_price = data["Unit_Price"].values  
sales_amount = data["Sales_Amount"].values  
unit_cost = data["Unit_Cost"].values  


Using NumPy arrays makes calculations faster and easier.


6. Revenue Analysis

Total revenue and average sales were calculated using:

total_revenue = np.sum(sales_amount)  
average_sales = np.mean(sales_amount)  

Results:

* Total Revenue ≈ 5,019,265.23
* Average Sales ≈ 5,019.27

This means the business earned about 5 million in total, and the average sale value is around 5,019.


 7. Indexing and Slicing

Indexing and slicing were used to view specific data:

sales_amount[:10]  
quantity[-5:]  


This helps us check the first few and last few records in the dataset.


8. Statistical Analysis

We calculated:

mean_sales = np.mean(sales_amount)  
median_sales = np.median(sales_amount)  
variance_sales = np.var(sales_amount)  
std_sales = np.std(sales_amount)  

Results:

* Mean: 5019.27
* Median: 5019.30
* Variance: 8,096,109.81
* Standard Deviation: 2845.37

The mean and median are almost equal, which shows balanced sales. The standard deviation shows that sales values vary moderately.


9. Revenue Verification Using Broadcasting

Revenue was recalculated using:

calculated_revenue = quantity * unit_price  

Broadcasting allows multiplication of arrays without using loops, making the calculation faster.

10. Profit Analysis

Profit was calculated using:

profit = (unit_price - unit_cost) * quantity  
profit_percentage = (profit / sales_amount) * 100  

This helps us understand how much profit the business makes from each sale.


 11. Category-Wise Sales

Total sales for each category:

* Clothing – 1,313,474.36
* Electronics – 1,243,499.64
* Food – 1,201,773.54
* Furniture – 1,260,517.69

Clothing has slightly higher sales, but all categories perform almost equally.


12. Sales Range

Highest and lowest sales were found using:

np.max(sales_amount)  
np.min(sales_amount)  

Results:

* Highest Sale: 9,989.04
* Lowest Sale: 100.12

This shows that some transactions are small while some are large.

 Conclusion

This project shows how NumPy can be used to analyze real sales data easily and efficiently.

We calculated total revenue, average sales, profit, and statistical values using NumPy functions. The results show that the business has strong revenue, balanced category performance, and stable sales trends.

Overall, NumPy is a powerful and useful tool for performing fast and accurate data analysis.

