# NORTHWIND-TRADERS-ANALYSIS

# **Introduction**
Northwind traders dataset was analysed based on different category of products sold to different companys within Europe, North America and South America. The total quantity purchased by these countries, their order details, the shipping mode to different countries, freight rate and more factors will be considered and analysed to give a better meaning and view of the Northwind traders sales.


# **Activity**
- [ ]  Importation of the ‘Northwind Traders Dataset’ dataset into Power BI Desktop
- [ ]  To determine the total quantity ordered, average unit price by product, average quantity ordered, the total discount
- [ ]  To determine the maximum period required to deliver products.
- [ ]  To determine the average quantity sold by product name, average sales per year, total unit sold by product catergory, average freight by country, and the freight rate by shipping mode
- [ ]  A slicer will be used to visualize the trend by different years
- [ ]  A dashboard to monitor the traders market sales will also be developed dataset.
 

# **Skills Demonstrated**
- Data Importation and data cleaning
- Data Modelling
- Using Dax functions
- Creating a Dashboard


# **Data Importation and Cleaning**
The Northwind Traders datasets containing seven tables (Categories, Customers, Employees, Order_details, Orders, Products and Shippers) which were all imported into my Power BI software. These tables were cleaned by first captalizing the first letter of all title headers and choosing suitable 'data name' for each column title. The 'Data Type', Data format, 'summarization' and 'category' were formatted for all columns, to suit each column selected. The tables were to transformed into the power query editor to further cleaning, where some table headers were promoted, null values found in the employees table, 'Report To' column was replaced with 5, the column distribution and column profile were checked to determine values/text distribution, errors, valid rows and empty rows were checked, empty rows found in the shipped_date column, from the order table was replace with '10/01/2013'. The column profiling for all tables were changed from 'top 1000 rows' to the entire data. The data modelling of the tables and their connections was checked and and changed from 'single' to 'both' in the cross filter section. The changed made to the entire work was closed and applied.

To determine the total quantity ordered, the Card visual was used to represent the 'Total Sales' KPI, this was calculated using the _Sum_ aggregate funtion for the summation of the total quantity ordered by customers, where the value was observed to be seen as 51317, which varied across the three years of sales. The average unit price of product sold was evaluated to be 29, using the _Average_ aggregate function, the average unit price remained throughout the 2013, 2014 and 2015 hence there was no increase in the three years of sales. The average quantity ordered was also visualized to be 24 yearly. The total discount on all products was observed to be 121 which increased 2014, but decreased in 2015.


[Project.PBI...pdf](https://github.com/Jessie-Watt/NORTHWIND-TRADERS-ANALYSIS/files/12597881/Project.PBI.pdf)

The maximum period required for the delivery of good was evaluated using a calculated column
