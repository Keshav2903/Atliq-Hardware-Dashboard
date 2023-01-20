# Atliq-Hardware-Dashboard
Project description

The project shows the sales insights of the ATLIQ HARDWARE in INDIA which sells millions of products each year. To track down the live sales and revenue/cost, we generated a POWER BI based report along with the dashboard to check what sales have patterns throughout the years and months.

The report helps to see:

1- Revenue per year 2- Revenue per month 3- Revenue per customer 4- Revenue per region 5- Top 5 customers 6- Top 5 sales Quantities 7- Sales by customer 8- Sales by city 9- Sales by year 10- Sales by month 11- Overall sales/Revenue

Tools that we used:

1- Microsoft Power BI Desktop 2- MYSQL Workbench 3- Microsoft Power BI Web version

Skills needed to complete the job:

1- Data Cleansing 2- DAX language 3- Analytical Skills 4- SQL Query Language 5- Business Intelligence Knowledge

Here are some of the querys that helped me to verify my Report and Dashboard results

1- The query will tell you sum of total sales amount throughout all years. SELECT sum(transactions.sales_amount) from date inner join transactions on date.date = transactions.order_date where date.year = '2020' and transactions.currency = 'INR\r' or transactions.currency = 'USD\r'

2-This can be used for to check the total sales in a specific region like I checked in Chennai select sum(sales.transactions.sales_amount) from sales.markets inner join sales.transactions on sales.markets.markets_code = sales.transactions.market_code where sales.markets.markets_name = "Chennai"
