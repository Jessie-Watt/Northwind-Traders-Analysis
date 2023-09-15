# NORTHWIND-TRADERS-ANALYSIS

# **Introduction**
Northwind traders dataset was analysed based on different category of products sold to different companys within Europe, North America and South America. The total quantity purchased by these countries, their order details, the shipping mode to different countries, freight rate and more factors will be considered and analysed to give a better meaning and view of the Northwind traders sales.


# **Activity**
- [ ]  Importation of the ‘Northwind Traders Dataset’ dataset into Power BI Desktop
- [ ]  To determine the total quantity ordered, average unit price by product, average quantity ordered, the total discount
- [ ]  To determine the maximum period required to deliver products.
- [ ]  To determine the average quantity sold by product name, average freight by country, average sales per year, total unit price by catergory, and freight rate by shipping mode
- [ ]  A slicer will be used to visualize the trend by different years
- [ ]  A dashboard to monitor the traders market sales will also be developed dataset.
 

# **Skills Demonstrated**
- Data Importation and data cleaning
- Data Modelling
- Using Dax functions
- Creating a Dashboard


# **Data Importation and Cleaning**
The Northwind Traders datasets contained seven tables (Categories, Customers, Employees, Order_details, Orders, Products and Shippers), which were all imported into my Power BI software. These tables were cleaned by first captalizing the first letter of all title headers and choosing suitable 'data name' for each column title. The 'Data Type', Data format, 'summarization' and 'category' were formatted for all columns, to suit each column selected. The tables were to transformed into the power query editor for further cleaning, where some table headers were promoted, null values found in the employees table, 'Report To' column was replaced with 5, the column distribution and column profile were checked to determine values/text distribution, errors, valid rows and empty rows, the empty rows found in the shipped_date column, from the Order table was replace with '10/01/2013'. The column profiling for all tables were changed from 'top 1000 rows' to the entire data. The data modelling of the tables and their connections was checked and changed from 'single' to 'both' in the cross filter section. The changes made to entire dataset was then applied and closed from the power query editor. The data modelling can be view [here].

To determine the total quantity ordered, the Card visual was used to represent the 'Total Sales' KPI, this was calculated using the _Sum_ aggregate funtion for the summation of the total quantity ordered by the customers, where the result was observed to be seen as 51317, this value varied across the three years of sales. The average unit price of products sold was evaluated to be 29, which was eveluated using the _Average_ aggregate function. The average unit price remained constant throughout 2013, 2014 and 2015 hence there was no increase in the three years of sales. The average quantity ordered was also visualized to be 24 yearly. The total discount on all products was observed to be 121, which increased 2014, but decreased in 2015.

![Dashboard](https://github.com/Jessie-Watt/Northwind-Traders-Analysis/assets/140435577/efe9ac62-9fa0-4929-b12a-85a102865fc8)



To obtain the maximum period required for the delivery of goods, a calculated column was used to evaluate the syntax:_DATEDIFF(start_date, end_date, unit)_. The new column was titled 'Shipping Days Interval' with the function written as: _Shipping Days interval = DATEDIFF(orders[Order Date], orders[Shipped Date], DAY)_, the column was sorted in descending order, this visualized thirty-seven days as the maximum number of days required to deliver goods to a customer, hence over a month will get a desired product to a customers door-step. Please visualize the column [here]. 

The average quantity sold per product was visualized using a table build visual. The average quanity was evaluated by the product name using the _Average_ aggregate _syntax: AVERAGE(column or expression)_. The visual values were formatted in descending order, showing the background colour of the highest average value to be dark green, then the following lower values to be lighter shades of green, Hence this represented top product as 'Schoggi Schokolade'.

The average freight by country was calculated by the _average_ aggregate function syntax: _AVERAGE(column or expression)_, using the Bar Column chart to represent the visual. This visual reported Austria to have the highest freight rate cost for shipping goods to customers, followed by Ireland and USA.

The average sales per year was represented in the line chart visual to show the total sales trend across the years, hence the _sum_ aggreagte function was utilized to evaluate this _syntax:SUM(column or expression)_. The Line chart reported the average sales, to increase across the years. The average sales by month was also considered but it gave a haphazard trend across the line chart reporting.

The total unit price by catergory was visualized using a Bar chart, this pictured the category name that produces the highest unit price sold as beverages, followed by Confections, meat and poultry, then diary products. This was evaluated using the _sum_ aggregate and syntax: _SUM(column or expression)_.

The freight rate by shipping mode was visualize using a donut chart, this evaluated the sum of freight rate for different shipping companies. Three companies were involved in the delivery of products to customers but on evaluation 'United Package' Shipping Company incurred more freight rate compared to other shipping companies, from delivering products from one place to another. The _sum_ function was used to evaluate the Sum of frieght rate by each shipping company.

# Conclusion
From the total unit price by catergory, the sales of beverages will yield more revenue for the Traders. It was observed that the employee ID 7 and 8, were in charge of the products that took the highest number of days to deliver the items to their customers. Hence they should develop better means, that would not incur more cost but would be very efficient to transport goods to customers quickly and effieciently.
It was also observed that transporting more goods to Austria will increase the freight rate on the Northwind traders. 




