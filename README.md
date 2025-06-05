# Walmart Data Analysis: End-to-End (Python + MySQL + PowerBI)

## Project Overview

This project is an end-to-end data analysis solution designed to extract critical business insights from Walmart sales data. We utilize Python for data processing and analysis, SQL for advanced querying, and structured problem-solving techniques to solve key business questions. Power BI is used for creating rich, interactive dashboards. The project is ideal for data analysts looking to develop skills in data manipulation, SQL querying, data visualization, and pipeline creation.

---

## Project Steps

### 1. Set Up the Environment
   - **Tools Used**: Visual Studio Code (VS Code), Python, MySQL , PowerBI
   - **Goal**: Create a structured workspace within VS Code and organize project folders for smooth development and data handling.

### 3. Download Walmart Sales Data
   - **Data Source**: Use the Kaggle Website to download the Walmart sales datasets.
   - **Dataset Link**: https://github.com/kushal-0412/walmart-data-analytics-py-mysql-powerbi/blob/main/data/Walmart.csv

### 4. Install Required Libraries and Load Data
   - **Libraries**: Install necessary Python libraries using:
     ```bash
     pip install pandas numpy sqlalchemy mysql-connector-python 
     ```
   - **Loading Data**: Read the data into a Pandas DataFrame for initial analysis and transformations.

### 5. Explore the Data
   - **Goal**: Conduct an initial data exploration to understand data distribution, check column names, types, and identify potential issues.
   - **Analysis**: Use functions like `.info()`, `.describe()`, and `.head()` to get a quick overview of the data structure and statistics.

### 6. Data Cleaning
   - **Remove Duplicates**: Identify and remove duplicate entries to avoid skewed results.
   - **Handle Missing Values**: Drop rows or columns with missing values if they are insignificant; fill values where essential.
   - **Fix Data Types**: Ensure all columns have consistent data types (e.g., dates as `datetime`, prices as `float`).
   - **Currency Formatting**: Use `.replace()` to handle and format currency values for analysis.
   - **Validation**: Check for any remaining inconsistencies and verify the cleaned data.

### 7. Feature Engineering
   - **Create New Columns**: Calculate the `Total Amount` for each transaction by multiplying `unit_price` by `quantity` and adding this as a new column.
   - **Enhance Dataset**: Adding this calculated field will streamline further MYSQL analysis and aggregation tasks.

### 8. Load Data into MySQL
   - **Set Up Connections**: Connect to MySQL using `sqlalchemy` and load the cleaned data into each database.
   - **Table Creation**: Set up tables in MySQL using Python SQLAlchemy to automate table creation and data insertion.
   - **Verification**: Run initial MYSQL queries to confirm that the data has been loaded accurately.

### 9. MYSQL Analysis: Complex Queries and Business Problem Solving
   - **Business Problem-Solving**: Write and execute complex SQL queries to answer critical business questions, such as:
     - Revenue trends across branches and categories.
     - Identifying best-selling product categories.
     - Sales performance by time, city, and payment method.
     - Analyzing peak sales periods and customer buying patterns.
     - Profit margin analysis by branch and category.
   - **Documentation**: Keep clear notes of each query's objective, approach, and results.

---

## Requirements

- **Python 3.8+**
- **SQL Databases**: MySQL
- **Python Libraries**:
  - `pandas`, `numpy`, `sqlalchemy`, `mysql-connector-python`
- **PowerBI Desktop**

## Project Structure

```plaintext
|-- data/                     # Raw data and transformed data
|-- mysql_queries/            # SQL scripts for analysis and queries
|-- notebooks/                # Jupyter notebooks for Python analysis
|-- powerbi_dashboard/        # Power BI dashboard (.pbix files, visuals, screenshots)  
|-- README.md                 # Project documentation
```
---

## Results and Insights

This section will include your analysis findings:
- **Sales Insights**: Key categories, branches with highest sales, and preferred payment methods.
- **Profitability**: Insights into the most profitable product categories and locations.
- **Customer Behavior**: Trends in ratings, payment preferences, and peak shopping hours.

--- 

 ## 📊 Power BI Dashboard Integration

After performing data cleaning, transformation, and analysis using Python and SQL, the insights were visualized using **Power BI** to make them accessible and interactive for business stakeholders.

### 🔍 Key Visualizations:

| **Visualization**                       | **Description**                                                                                   |
|----------------------------------------|---------------------------------------------------------------------------------------------------|
| **Top 5 Branch by Profit**             | Horizontal bar chart showing the five Walmart branches with the highest profits.                 |
| **Sales by Product Category**          | Vertical bar chart displaying the total sales across different product categories.               |
| **Top Performing Cities by Profit**    | Horizontal bar chart comparing total sales and profit for top-performing cities.                 |
| **Sales by Payment Type**              | Donut chart visualizing the proportion of sales by payment methods (Credit Card, Ewallet, Cash). |
| **Key Metrics Summary**                | KPI cards showing overall Total Sales, Total Profit, and average Customer Rating.                |
| **Total Sales by Year**                | Column chart representing yearly sales totals to observe long-term trends.                       |
| **Monthly Sales and Profit % Trend**   | Combo chart with bars for total monthly sales and a line showing profit percentage trends.       |


### 🧭 Dashboard Preview:

![Power BI Walmart Dashboard](https://github.com/kushal-0412/walmart-data-analytics-py-mysql-powerbi/blob/main/powerbi/Dashboard_Image.png)


### 🗂️ Access the Dashboard:

- 📁 Power BI file: [`Walmart_Sales_Dashboard.pbix`](https://github.com/kushal-0412/walmart-data-analytics-py-mysql-powerbi/blob/main/powerbi/Dashboard_Walmart.pbix)

To view:

1. Download the `.pbix` file.
2. Open in [Power BI Desktop](https://powerbi.microsoft.com/desktop/).
3. Explore, filter, and interact with the visuals.


## Future Enhancements

Possible extensions to this project:
- Integration with a dashboard tool (e.g., Power BI or Tableau) for interactive visualization.
- Additional data sources to enhance analysis depth.
- Automation of the data pipeline for real-time data ingestion and analysis.

---

## License

This project is licensed under the MIT License. 

---

## Acknowledgments

- **Data Source**: Kaggle’s Walmart Sales Dataset
- **Inspiration**: Walmart’s business case studies on sales and supply chain optimization.

---
