# Challenge_7

**Background**

In recent years, finance has had an explosion in passive investing. Passive investing means that I invest in a basket of assets that’s called an exchange-traded fund (ETF). This way, you don’t spend time researching individual stocks or companies or take the risk of investing in a single stock. ETFs offer more diversification.

In this Challenge assignment, I built a financial database and web application by using SQL, Python, and the Voilà library to analyze the performance of a hypothetical fintech ETF.

**What I am Creating**
For this Challenge assignment, you need to create and submit the following deliverables:

A Jupyter notebook that contains the following:

1. Your analysis of the ETF data that a SQL database stores

2. Professionally styled and formatted interactive visualizations


**Instructions**
I used the etf_analyzer.ipynb notebook to complete your analysis of a fintech ETF that consists of four stocks: GOST, GS, PYPL, and SQ. Each stock has its own table in the etf.db database, which the Starter_Code folder contains.

I analyzed the daily returns of the ETF stocks both individually and as a whole. Then deploy the visualizations to a web application by using the Voilà library.

The detailed instructions are divided into the following parts:

1. I analyzed a single asset in the ETF

2. I optimized the data access with advanced SQL queries

3. I analyzed the ETF portfolio

4 I Deploy the notebook as a web application

**Analyze a Single Asset in the ETF**


For this part of the assignment, you’ll use SQL queries with Python, Pandas, and hvPlot to analyze the performance of a single asset from the ETF.

Complete the following steps:

1. I Wrote a SQL SELECT statement by using an f-string that reads all the PYPL data from the database. Using the SQL SELECT statement, execute a query that reads the PYPL data from the database into a Pandas DataFrame.

2. I used the head and tail functions to review the first five and the last five rows of the DataFrame. Make a note of the beginning and end dates that are available from this dataset. You’ll use this information to complete your analysis.

3. I used hvPlot, create an interactive visualization for the PYPL daily returns. Reflect the “time” column of the DataFrame on the x-axis. Make sure that you 
     professionally style and format your visualization to enhance its readability.

4. I then used hvPlot, create an interactive visualization for the PYPL cumulative returns. Reflect the “time” column of the DataFrame on the x-axis. Make sure that you 
     professionally style and format your visualization to enhance its readability.

**Optimize Data Access with Advanced SQL Queries**

For this part of the assignment, I continued to analyze a single asset (PYPL) from the ETF. I used advanced SQL queries to optimize the efficiency of accessing data from the database.

I completed the following steps:

1. Accessed the closing prices for PYPL that are greater than 200 by completing the following steps:

2. wrote a SQL SELECT statement to select the dates where the PYPL closing price was higher than 200.0.

3. Used the SQL statement, read the data from the database into a Pandas DataFrame, and then review the resulting DataFrame.

4. Selected the “time” and “close” columns for those dates where the closing price was higher than 200.0.

5. Found the top 10 daily returns for PYPL by completing the following steps:

6. Wrote a SQL statement to find the top 10 PYPL daily returns. Make sure to do the following:

7. Used SELECT to select only the “time” and “daily_returns” columns.

8. Used ORDER to sort the results in descending order by the “daily_returns” column.

9. Used LIMIT to limit the results to the top 10 daily return values.

10. Used the SQL statement, read the data from the database into a Pandas DataFrame, and then review the resulting DataFrame.

**Analyze the ETF Portfolio**

For this part of the assignment, I built the entire ETF portfolio and then evaluate its performance. To do so, you’ll build the ETF portfolio by using SQL joins to combine all the data for each asset.

I Completed the following steps:
1. Write a SQL query to join each table in the portfolio into a single DataFrame. To do so, complete the following steps:
2. used a SQL inner join to join each table on the “time” column. Access the “time” column in the GDOT table via the GDOT.time syntax. Access the “time” columns from 
    the other tables via similar syntax.
3. used the SQL query, read the data from the database into a Pandas DataFrame. Review the resulting DataFrame.
4. I created a DataFrame that averages the “daily_returns” columns for all four assets. Review the resulting DataFrame.
5. I Used hvPlot, create an interactive line plot that visualizes the cumulative return values of the ETF portfolio. Reflect the “time” column of the DataFrame on the x-axis. 



