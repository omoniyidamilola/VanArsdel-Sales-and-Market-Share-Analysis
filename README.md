
## SALES AND MARKET SHARE ANALYSIS
### INTRODUCTION

As a Business Developer for VanArsdel. My goal is to analyze the sales and market share of our company and its competitor. VanArsdel is a fictitious manufacturing company that manufactures expensive electronic products that could be used for fun as well as works and it sells them directly to consumers nationwide as well as several other countries.

# ABOUT THE DATASETS
1.	International Sales Folder: Contains the sales data of six different countries which include: Australia, Canada, Germany, Japan, Mexico and Nigeria.

2.	US Sales Folder: Contains US sales dataset and also contains data for other dimensions table like products, manufacturer and geographical location.

3.	Color Theme Folder: Contains the color theme you can use to design the charts and dashboards.

4.	VanArsdel Logo: This is the VanArsdel company logo for the dashboard design.

## PROBLEM STATEMENT 

To identify:

•	What is the Market Share of our company (VanArsdel)?

•	What is the Revenue Trend across all Manufacturers?

•	What is the Sales distribution in the US?

•	Revenue Trend and Year-On-Year Growth?

## SKILLS DEMONSTRATED
The following Microsoft Excel Skills were incorporated into this project:

•	Data transformation using Power Query.

•	Data modelling using Power Pivot.

•	The use of Data Analysis eXpression (DAX) in Power Pivot.

•	Building Pivot Tables and Pivot Charts.

•	The use of Slicers.

#### DATA TRANSFORMATION
I imported my dataset after which I transformed it into Power Query and renamed the tables. After renaming, I started with the data cleaning. I cleaned the products table first. Split the product column using the split column by delimiter and renamed the splitted columns into Product and Segment.

![Product by delimiter](https://github.com/omoniyidamilola/VanArsdel-Sales-and-Market-Share-Analysis/blob/main/Product%20by%20Delimiter.png)

I separated the Price column into two column and renamed it currency and price. From the Geography table, I removed the top 3 rows because they are irrelevant and use the first row as Headers. The country column contains a Null value which was filtered out.

![Null values](https://github.com/omoniyidamilola/VanArsdel-Sales-and-Market-Share-Analysis/blob/main/Geo%20Null%20values.png)

I joined zip and country column together. From the manufacturer table, I removed the bottom 3 rows. I transpose the table and use first row as header. The US sales table doesn’t really need much cleaning, I just changed the type. From the International Sales table I removed the Source name from the table because I don’t need it for my analysis and is irrelevant.
To combine US sales with international sales I used Append Table but for Append to work properly I need to have the same exact column in both table so I created a new column called country to US sale by using the custom column.

![Custom Column](https://github.com/omoniyidamilola/VanArsdel-Sales-and-Market-Share-Analysis/blob/main/Geo%20Custom%20column.png)

 After creating a new column named country, I append international sales and US sales together. I renamed the Append1 as All sales. After cleaning I loaded my datasets into the Power Pivot because the data set is large about 7 million rows which is too large to load to excel.

![Append table](https://github.com/omoniyidamilola/VanArsdel-Sales-and-Market-Share-Analysis/blob/main/Append%20Table%20for%20All%20sales.png)

## DATA MODELLING

![Data Model](https://github.com/omoniyidamilola/VanArsdel-Sales-and-Market-Share-Analysis/blob/main/Data%20Modelling.png)

I created relationships between the tables from the diagram view using many to one and one to many relationships. I created the date table, I calculated Total Revenue: =SUM (All Sales [Revenue]. I Calculated the Last Year Revenue. I also calculated for YOY Change.
Below are the tables showing the calculated measures from the Power Pivot.

![Date Time table](https://github.com/omoniyidamilola/VanArsdel-Sales-and-Market-Share-Analysis/blob/main/Date%20time%20for%20Power%20Pivot.png)

![last year revenue table](https://github.com/omoniyidamilola/VanArsdel-Sales-and-Market-Share-Analysis/blob/main/Last%20year%20Revenue%20table.png)


![Total revenue table](https://github.com/omoniyidamilola/VanArsdel-Sales-and-Market-Share-Analysis/blob/main/Total%20Revenue%20Table.png)

![YOY Growth](https://github.com/omoniyidamilola/VanArsdel-Sales-and-Market-Share-Analysis/blob/main/YOY%20Growth.png)

I analyze and visualized my reports by using the Pivot Table and Pivot charts.

I created dashboard for the report. Below is the dashboard

![Sales and market share dashboard](https://github.com/omoniyidamilola/VanArsdel-Sales-and-Market-Share-Analysis/blob/main/Sales%20and%20Market%20Share%20Analysis%20Dashboard.jpg)

## CONCLUSION

VanArsdel has the largest Market Share in 3 countries (Germany by 60.67%, Australia by 51.49% and Japan by 48.23%) out of the 7 countries and VanArsdel is the top manufacturer over the years from 2014-2021.
VanArsdel is also trending upward by revenue.
There was increase in sales from the revenue generated BUT the Year of Year % Growth dropped from 27.1% in 2015- 6.68% in 2019 and and begins to rise again in 2020 to 7.06%.
In the United States Sales, California, Texas and Florida are topping by Sales.


### RECOMMENDATIONS

Allocate resources to Germany, Australia and Japan to ensure continued growth and competitive advantage.

Develop targeted marketing and sales strategies to sustain and further accelerate revenue growth.

Evaluate the impact of external factors such as market conditions and internal factors like product innovation and customer satisfaction.

Implement strategies to drive consistent and sustainable year-on-year growth.  

Analyze customer preferences and buying behavior. 

Identify competitors’ strengths, weaknesses, and strategies. 

Leverage this knowledge to refine VanArsdel's market positioning, differentiate its products, and identify potential opportunities for expansion. 

Stay at the forefront of innovation by investing in research and development. 

Continuously improve existing products and develop new ones to meet evolving customer needs and stay ahead of competitors. 

Focus on maintaining high levels of customer satisfaction and retention. 

Implement customer feedback systems and analyze customer data to identify areas for improvement. 

Develop customer loyalty programs, provide excellent after-sales support, and deliver exceptional service to strengthen customer relationships.

Develop market entry strategies tailored to each country where VanArsdel’s Share is low, considering cultural, regulatory, and competitive factors.


