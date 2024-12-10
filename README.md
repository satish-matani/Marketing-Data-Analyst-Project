# Marketing Data Analyst Project

## Business Problem
The goal of this project was to address the challenges faced by a marketing team in improving customer engagement and optimizing product sales. The primary business problem involved analyzing customer reviews and sentiment to gain insights into customer satisfaction. These insights could then be used to enhance product offerings and marketing strategies. The project was developed using SQL, Python, and Power BI to clean, process, and visualize data that drives marketing decisions.

## Technical Approach

### SQL
* Data Extraction: Used SQL to fetch data from the customer_reviews table in a Microsoft SQL Server database, including key attributes such as ReviewID, CustomerID, ProductID, ReviewDate, Rating, and ReviewText.
* Window Functions: Leveraged SQL window functions like ROW_NUMBER(), RANK(), and PARTITION BY to calculate running totals and rankings across products based on customer ratings. This helped identify high-performing products and customer engagement trends.
* Aggregation & Joins: Aggregated review data and joined multiple tables to correlate customer sentiment with product attributes.

### Python
* Fetched data from SQL Server using SQLAlchemy.
* Cleaned and preprocessed data using Pandas.
* Performed sentiment analysis using VADER from NLTK.
* Categorized sentiment scores and engineered a `SentimentBucket` feature.
* Exported processed data to a CSV file.

### Power BI
* Imported cleaned data from the CSV file.
* Transformed data within Power Query.
* Built dynamic KPIs using DAX.
* Designed visualizations like bar charts, pie charts, and sentiment distribution histograms.
* Incorporated slicers and filters for interactive analysis.

## Conclusion
By combining SQL, Python, and Power BI, this project provided actionable insights into customer sentiments, enabling the marketing team to make informed decisions aimed at improving customer satisfaction and driving product sales.
