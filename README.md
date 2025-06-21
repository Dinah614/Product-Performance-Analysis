# Product-Performance-Analysis

### Project Overview

Analyzing sales data to uncover trends, top-selling products, and areas for improvement, providing insights to inform business decisions. 
Analyze sales data to identify trends, top-selling products, and revenue metrics for business decision-making.

In this project, I dive into a large sales dataset to extract valuable insights. To explore sales trends over time, identify the best-selling products, calculate revenue metrics such as total sales and profit margins, and create visualizations and present my findings effectively.

This project showcases my ability to manipulate and derive insights from large datasets, enabling me to make data-driven recommendations for optimizing sales strategies.    
                                          
### ABOUT THE DATA

It shows the sales data record of a company that deals in the sales of Planes, Cars and Motorcycles from April 2003 to April 2005 i.e. for the period of thirteen (24) months, it comprises of 28 distinct columns and 2822 rows. The columns names are: Product_Id,Order Number, Order_Line_Number, Total Order, Product Line, Msrp, Product Code, Quantity Ordered, Price Each, Sales, Order Date, Order Day, Status, Qtr_Id, Month_Id, Year_Id, Customer Name, Phone, Address_Line1, Address_Line2, City, State, Postal Code, Country, Territory, Contact_Last_Name, Contact_First_Name, Deal Size.

![Screenshot (82)](https://github.com/user-attachments/assets/1351f0b7-4a1b-4ba9-9ade-17bc4cc3698c)

### DATA CLEANING
The cleaning process was one of the most important aspects of this project as it eliminated factors that could bring in bias or errors into our analysis.
I took the following steps to ensure the data was cleaned:
1.	I checked for duplicate rows by selecting the table, navigating to the data tab and clicking on “Remove Duplicates”. There was no duplicate in the dataset.

![Screenshot (88)](https://github.com/user-attachments/assets/ab70a079-9dde-4b7e-9884-7ae34343fe0f)

2.  I formatted the Order Date column to a more standard date format. I did this by selecting the date column and applying custom formatting. Also I change the date column to Month and Year only by creating a new column date and input the “TEXT(Order Date column, “MMMM-YYYY”) thereby having the Month and Year Only for the Order Date.

![WhatsApp Image 2025-06-18 at 10 49 56](https://github.com/user-attachments/assets/1dbbf150-1819-4249-88e2-00327d770d61)

New Date Column
3. I deleted the initial Order Date column because they weren’t important to our analysis.

![WhatsApp Image 2025-06-18 at 10 54 29](https://github.com/user-attachments/assets/a5b76246-1be6-4d18-8654-dc502448d02c)

4. I formatted the entire table with a bright table style to make the table presentable “CTRL +A”, then I went to the home tab and took  “Format as Table” and chose a table style.

![WhatsApp Image 2025-06-18 at 11 05 14](https://github.com/user-attachments/assets/3decaa10-f835-4569-aa2d-93328ca60dc4)
![WhatsApp Image 2025-06-18 at 11 05 14 (1)](https://github.com/user-attachments/assets/6949a193-327f-443f-bc0d-5bfcca2d1d02)

5. I also formatted the column headers to Proper Case by inserting a row below the column headers, inserted “=PROPER(Table2[[#Headers],[product_id]])”, copied the entire row and pasted it on the above row to replace the old column headers and deleting the newly created rows.

  ![WhatsApp Image 2025-06-18 at 11 18 25](https://github.com/user-attachments/assets/8cfedfa9-2bc9-4fa9-9bae-8482c05cdc56)
 ![WhatsApp Image 2025-06-18 at 11 18 26](https://github.com/user-attachments/assets/efee490b-9ae7-4a10-9baf-d2deda2e1b76)
![WhatsApp Image 2025-06-18 at 11 18 27](https://github.com/user-attachments/assets/a237f429-eddb-4980-a5ff-07d450408ef0)
![WhatsApp Image 2025-06-18 at 11 18 27 (1)](https://github.com/user-attachments/assets/c91ebac3-f080-4326-b142-776ee71888f1)
![WhatsApp Image 2025-06-18 at 11 18 27 (2)](https://github.com/user-attachments/assets/5b26968b-656d-469e-ad5a-68dd25c92bce)

6. Carefully looking at the data, not all orders were shipped. Some of the orders were cancelled, disputed and on hold. Revenue cannot be calculated on orders that were Cancelled, I will filter the data sheet and select only the data that orders were shipped and resolved.Create a new worksheet only with the shipped and resolved order data.

![WhatsApp Image 2025-06-18 at 11 42 11](https://github.com/user-attachments/assets/18ce22a8-9975-4e45-bc69-37138e2794bf)
![WhatsApp Image 2025-06-18 at 11 42 11 (1)](https://github.com/user-attachments/assets/955c1582-9761-4f64-8986-d15bdc39ae78)

### ANALYSIS
I loaded the Clean Data Set into MySQL for the further analysis in order to answer business questions and meet up with objectives.
## KPIs Requirements
I need to need to analyze key indicators for our Product Sales data to gain insights into the business performance. Specifically i want to calculate the following metrics using MySQL
1. Total Revenue: The sum of all products ordered.
2. Avereage Order Value: The average amount spent per Order. Calculated by dividing the Sum of Total Revenue by the Total Number of Orders.
3. Total Products Sold: The sum of the Quantity of products sold.
4. Average Product Per Order: The Average Numberof Products Sold Per Oder. Calculated by Dividing the Total Number of Products Sold by the Total Number of Orders.

   ## Problem Statement

   # Charts Requirement
   I would like to visualize various aspects of our Products Sales Data to gain insights and understand key trends. I've identified the following requirements for creating Charts.
   1. Daily Trend for Total Orders: I will create a Bar Chart that displays the daily trend of total orders over a specific period of time.This Chart will help us identify any patterns or fluctuations in order volume on a daily basis.
   2. Percentage of sales by product category: Create a Pie Chart that shows
   3. 
















































































