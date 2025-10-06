# Sales-Product-Analysis
## _Table of Contents_ ##
<ul>

[1. About the project](#about-the-project)

[2. Business Problem](#business-problem)

[3. Data Preprocessing](#data-preprocessing)

[4. Data Analysis](#data-analysis)

[5. Conclusions](#conclusions)

<ul>

[4.1. Average Ticket by Month](#1-average-ticket-by-month)

[4.2. Sales Throughout the Year](#2-sales-throughout-the-year)

[4.3. Location Analysis](#3-location-analysis)

[4.4. Most Sold Products](#4-most-sold-products)

[4.5. Products Sold Together](#5-products-sold-together)

[4.6. Best Time for Advertisement](#6-best-time-for-advertisement)

</ul> 

</ul>

 <hr>

## __About the Project__ ##
This project is a self-study project aimed at practicing real-world data analysis in Python.

It focuses on Tech Store, a U.S.-based e-commerce business, analyzing its 2019 sales data to gain insights into sales trends, customer behavior, and product performance.

The detailed notebook of the project is [here](Tech%20Store%20Sales%20Analysis.ipynb)
.

<hr>

## __Business Problem__ ##

Tech Store opened in 2019, and by the end of the year, the director requested a year-end sales report.

The data analyst was asked to answer the following questions:

1. What is the average ticket by month?

2. How were sales distributed throughout the year?

3. Which locations had the highest sales?

4. Which products were sold most often?

5. Which products are most often sold together?

6. At what time should advertisements be displayed to maximize purchases?

<img src="visuals/ecommerce.jpg" alt="analyst"/> <hr>


## __Data Preprocessing__ ##

* Before analysis, the dataset was cleaned and prepared:

* Merged all 12 months of sales CSV files into a single DataFrame.

* Removed NaN and incorrect rows.

* Converted columns to proper data types: 'Order Date', 'Quantity Ordered', and 'Price Each'.

* Split 'Order Date' and 'Purchase Address' into separate columns.

* Created a 'Sales' column (Price Each * Quantity Ordered).

* Filtered out 2020 data to focus exclusively on 2019.

<hr>

# Data Analysis

### 1. <u>Average Ticket by Month </u> ###

Results: The average ticket for 2019 was around $185, with peaks in May and June at approximately $190.

<img src="visuals/AvgTicketByMonth.png" alt="Average Ticket by Month" width="600"/>


### 2. <u>Sales Throughout the Year.</u> ###

<b>Results:</b> 

Sales fluctuated throughout 2019: 

January–April: +23.2% increase.

May & September: followed by declines (-18.2% in June, -15.2% in August).

October: +78.1% growth (from $2.1M to $3.7M).

November: -14.4% decline.

December: highest turnover at $4.6M.

Recommendation: Investigate causes of the mid-year declines. With only one year of data, it is unclear if this trend repeats annually.

<img src="visuals/GrowthPercentageByMonth.png" alt="Monthly Sales Trend" width="600"/>

### 3. <u>Location Analysis</u> ###

<b>Results:</b>

| Location         | % of Total Sales |
|------------------|------------------|
| California       | 40.0%            |
| San Francisco    | 24.0%            |
| Los Angeles      | 16.0%            |
| New York         | 13.5%            |
| Boston           | 10.6%            |
| Portland, Maine  | 1.3%             |

Recommendation: Increase marketing efforts in New York to leverage its population and purchasing potential.

<img src="visuals/TotalSalesByCity.png" alt="Sales by City" width="500"/>

### 4. <u>Most Sold Products</u> ###

<b>Results:</b>

| Product        | % of Sales Value |
|----------------|------------------|
| MacBook Pro    | 23.3%            |
| iPhone         | 13.9%            |
| ThinkPad       | 12.3%            |

By units sold, top items: cables, wired headphones, and batteries (~25,000 units each).

<img src="visuals/TotalSalesbyProducts.png" alt="Most Sold Products" width="500"/>

### 5. <u>Products Sold Together</u> ###

<b>Results:</b>
Top product pairings:

Cell phones with chargers or headphones represent ~40% of sales.

Recommendation: Bundle these products and implement cross-selling campaigns on the website.

<img src="visuals/Products Sold Together.png" alt="Sales by Hour" width="500"/>

### 6. <u>Best Time for Advertisement</u> ###

Results:

Peak sales: 11 a.m. – 8 p.m., with the highest at 7 p.m. (7% of total sales).

Recommendation: Schedule advertisements during the early evening for maximum impact.

<img src="visuals/SalesByTheHour.png" alt="Sales by Hour" width="500"/>

# Conclusions

California drives the majority of sales (40%) despite a smaller population than New York, due to higher purchasing power. Marketing should focus on this region.

Top-selling product combinations are cell phones and accessories; bundle campaigns are recommended.

Sales fluctuate throughout the year, with a strong finish in December; investigate mid-year dips for strategic planning.

## References

Dataset: <a href="https://www.kaggle.com/datasets/knightbearr/sales-product-data">Kaggle</a>

Per Capita Personal Income of US cities: <a href="https://www.census.gov/quickfacts/fact/table/portlandcitymaine,bostoncitymassachusetts/HSG010221">Census</a> and <a href="https://en.wikipedia.org/wiki/List_of_U.S._cities_by_adjusted_per_capita_personal_income">Wikipedia</a>

List of US cities by population: <a href="https://en.wikipedia.org/wiki/List_of_United_States_cities_by_population">Wikipedia</a>

Image by <a href="https://www.freepik.com/free-photo/person-analyzing-checking-finance-graphs-office_41791161.htm#fromView=keyword&page=1&position=29&uuid=c0ba11c9-1b4b-4721-a6fb-791fdf4be116&query=Data+analyst">Image From Freepik</a>