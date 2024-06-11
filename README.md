# Coffee Sales Dashboard

## About
This project aim to explore the Coffee Sales Data to understand top performing sales and types of coffee in 3 countries included United States, United Kingdom and Ireland.

## Historical Background
The United States, United Kingdom and Ireland have different coffee flavors. The data are known to affect sales and orders, but it is challenging to understanding which have the most coffee consumption habits.

## Purpose of The Project
The major aim of this project is to gain insight into the sales data of Coffee Sales to understand the different factors that affect sales of the different countries.

## Approach
Make the dashboard to pivot data and summary the information needed by using Excel.
1. **Data Wrangling:** This is the first step where inspection of data is done to make sure **NULL** values and missing values are detected and data replacement methods are used to replace, missing or **NULL** values.
> Using formulas such as **XLOOKUP** to retrieve the country for each orders. Combining the **INDEX MATCH** syntax to retrieve the `roast_type`, `size`, `name`, and `loyalty_card`.
> Calculating the sales by take the column `quantity` to multiply by column `unit_price`.
> Using combination of **IF** functions to get data in the *coffee_type_name, roast_type_name*.

2. **Data Pivot:** This is the second step which make the pivot table in order to summary data as needed. Make separately in three different sheets includes `total_sales`, `country_bar_chart`, and `top_5_customers`.
> Retrieving data by using pivot table for making the summary table.

3. **Exploratory Data Analysis (EDA):** Exploratory data analysis in order to accurately pull data and the aims of this project.

4. **Data Visualization:**  This step is used interchangeably with information graphics, information visualization and statistical graphics to make it easier to identify patterns, trends and outliers in large data sets.

## Dataset
The dataset contains orders, customers products which respectively located in United States, United Kingdom and Ireland:
`orders`
| Column                  | Description                             |
| :---------------------- | :-------------------------------------- |
| Order ID                | the ID of orders                        |
| Order Date              | the Date which get the orders           |
| Customer ID             | the ID of customers                     |
| Product ID              | the ID of products                      |
| Quantity                | the number of orders                    |
| Customer Name           | the customer name                       |
| Email                   | the ID of products                      |
| Country                 | the ID of products                      |
| Coffee Type             | the ID of products                      |
| Roast Type              | the ID of products                      |
| Size                    | the ID of products                      |
| Unit Price              | the ID of products                      |
| Sales                   | the ID of products                      |

`customers`
| Column                  | Description                             |
| :---------------------- | :-------------------------------------- |
| Customer ID             | the ID of customer                      |
| Customer Name           | the customer name                       |
| Email                   | the email customer                      |
| Phone Number            | the phone number of customer            |
| Address Line 1          | the address of customer                 |
| City                    | the city name of each country           |
| Country                 | the country name                        |
| Postal Code             | the post code depends on the country    |
| Loyalty Card            | customers will receive when they often use coffee at all times   |

`products`
| Column                  | Description                             |
| :---------------------- | :-------------------------------------- |
| Product ID              | the ID of products                      |
| Coffee Type             | the type of coffee                      |
| Roast Type              | the name of roast (medium, light, dark) |
| Size                    | the size of a bag of roast type         |
| Unit Price              | the unit price                          |
| Price per 100g          | the unit price of 100g coffee           |
| Profit                  | the profit of each products             |

## Generic Question
1. Top names of customers who use coffee the most
2. Rank countries by coffee consumption from highest to lowest
3. Calculate the sum of total sales in yearly (from 2019 to 2022)

## Unit
- Currency unit: United States dollar ($)
- Unit of mass: kilogram (kg)

## Calculation
- `total_sales` = `quantity` * `unit_price`
  

