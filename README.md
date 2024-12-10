# Marketing Data Analyst Project

## Business Problem
The goal of this project was to address the challenges faced by a marketing team in improving customer engagement and optimizing product sales. The primary business problem involved analyzing customer reviews and sentiment to gain insights into customer satisfaction. These insights could then be used to enhance product offerings and marketing strategies. The project was developed using SQL, Python, and Power BI to clean, process, and visualize data that drives marketing decisions.

## Technical Approach

### SQL
* Data Extraction: Used SQL to fetch data from the `customer_reviews` table in a Microsoft SQL Server database, including key attributes such as ReviewID, CustomerID, ProductID, ReviewDate, Rating, and ReviewText.
* Window Functions: Leveraged SQL window functions like ROW_NUMBER(), RANK(), and PARTITION BY to calculate running totals and rankings across products based on customer ratings. This helped identify high-performing products and customer engagement trends.
* Aggregation & Joins: Aggregated review data and joined multiple tables to correlate customer sentiment with product attributes.

### Python
* Data Fetching & Preprocessing: Utilized SQLAlchemy to fetch data from the SQL Server database, and employed Pandas for data manipulation and cleaning.
* Sentiment Analysis: Implemented sentiment analysis using Python’s VADER sentiment analysis model from the nltk library. The sentiment scores were calculated for each customer review text and categorized into Positive, Mixed Positive, Negative, and Mixed Negative categories based on both sentiment score and the review rating.
* Feature Engineering: Introduced a SentimentBucket feature to categorize sentiment scores into defined ranges, helping identify the intensity of customer sentiment (e.g., strongly positive, mildly negative).
* Data Export: Exported the processed data with sentiment categories to a CSV file for further analysis and reporting.

### Power BI
* Data Import & Transformation: Imported cleaned data into Power BI using the CSV output from Python. Transformed data within Power Query for better performance and ease of use.
* Key Metrics & KPIs: Built dynamic KPIs using DAX to display metrics like average customer sentiment, top-rated products, and total reviews per product.
* Visualizations: Designed multiple visualizations such as bar charts, pie charts, and sentiment distribution histograms to represent customer sentiment and engagement across different products.
* Interactivity: Incorporated slicers and filters to allow marketing managers to drill down into product-specific reviews and sentiment data.

## Conclusion
In this project, I employed SQL for efficient data extraction and transformation, Python for deep sentiment analysis and feature engineering, and Power BI for building interactive dashboards. These combined techniques provided actionable insights into customer sentiments, enabling the marketing team to make informed decisions aimed at improving customer satisfaction and driving product sales.
