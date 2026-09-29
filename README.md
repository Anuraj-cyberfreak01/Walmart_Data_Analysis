

# Walmart Data Analysis: End-to-End SQL + Python Project

## Project Overview

![Project Pipeline](https://github.com/Anuraj-cyberfreak01/Walmart_Data_Analysis/blob/main/walmart_project_pipeline.png)

This project is an end-to-end data analysis solution designed to extract critical business insights from Walmart sales data. We utilize Python for data processing and analysis, SQL for advanced querying, and structured problem-solving techniques to solve key business questions. The project is ideal for data analysts looking to develop skills in data manipulation, SQL querying, and data analysis.

---

## Project Steps

### 1. Set Up the Project Environment

* **Tools Used**: Jupyter Notebook, Python, SQL (MySQL)
* **Goal**: Create a structured project folder and organize the dataset and Jupyter Notebook for smooth development and analysis.
* Create a folder named `Walmart Project`.
* Download the Walmart sales dataset from Kaggle and place the CSV file inside the project folder.
* Open Jupyter Notebook from the `Walmart Project` folder.

### 2. Download Walmart Sales Data

* **Data Source**: Kaggle
* **Dataset Link**: [Walmart Sales Dataset](https://www.kaggle.com/najir0123/walmart-10k-sales-datasets)
* Download the dataset manually from Kaggle.
* Place the downloaded CSV file inside the `Walmart Project` folder.
* The dataset is then loaded into the Jupyter Notebook for further analysis.

### 3. Install Required Libraries and Load Data

* **Libraries**: Install the necessary Python libraries using:

  ```bash
  pip install pandas numpy sqlalchemy mysql-connector-python
  ```
* **Loading Data**: Import the required libraries and read the Walmart sales CSV file into a Pandas DataFrame for initial analysis and transformations.

### 4. Explore the Data

* **Goal**: Conduct an initial data exploration to understand the data distribution, column names, data types, and identify potential issues.
* **Analysis**: Use functions like `.info()`, `.describe()`, and `.head()` to get a quick overview of the data structure and statistics.

### 5. Data Cleaning

* **Remove Duplicates**: Identify and remove duplicate entries to avoid skewed results.
* **Handle Missing Values**: Drop rows or columns with missing values if they are insignificant; fill values where essential.
* **Fix Data Types**: Ensure all columns have consistent data types (e.g., dates as `datetime`, prices as `float`).
* **Currency Formatting**: Use `.replace()` to handle and format currency values for analysis.
* **Validation**: Check for any remaining inconsistencies and verify the cleaned data.

### 6. Feature Engineering

* **Create New Columns**: Calculate the `Total Amount` for each transaction by multiplying `unit_price` by `quantity` and adding this as a new column.
* **Enhance Dataset**: Adding this calculated field will streamline further SQL analysis and aggregation tasks.

### 7. Load Data into MySQL and PostgreSQL

* **Set Up Connections**: Connect to MySQL and PostgreSQL using `sqlalchemy` and load the cleaned data into each database.
* **Table Creation**: Set up tables in both MySQL and PostgreSQL using Python SQLAlchemy to automate table creation and data insertion.
* **Verification**: Run initial SQL queries to confirm that the data has been loaded accurately.

### 8. SQL Analysis: Complex Queries and Business Problem Solving

* **Business Problem-Solving**: Write and execute complex SQL queries to answer critical business questions, such as:

  * Revenue trends across branches and categories.
  * Identifying best-selling product categories.
  * Sales performance by time, city, and payment method.
  * Analyzing peak sales periods and customer buying patterns.
  * Profit margin analysis by branch and category.
* **Documentation**: Keep clear notes of each query's objective, approach, and results.

### 9. Project Publishing and Documentation

* **Documentation**: Maintain well-structured documentation of the entire process in Markdown or a Jupyter Notebook.
* **Project Publishing**: Publish the completed project on GitHub or any other version control platform, including:

  * The `README.md` file (this document).
  * Jupyter Notebooks (if applicable).
  * SQL query scripts.
  * Data files (if possible) or instructions for accessing the dataset.

---

## Requirements

* **Python 3.8+**
* **SQL Databases**: MySQL, PostgreSQL
* **Python Libraries**:

  * `pandas`
  * `numpy`
  * `sqlalchemy`
  * `mysql-connector-python`
  * `psycopg2`

---

## Getting Started

1. Create a project folder named `Walmart Project`.

2. Download the Walmart Sales Dataset manually from Kaggle:
   [Walmart Sales Dataset](https://www.kaggle.com/najir0123/walmart-10k-sales-datasets)

3. Place the downloaded CSV file inside the `Walmart Project` folder.

4. Open Jupyter Notebook from the `Walmart Project` folder.

5. Install the required Python libraries:

   ```bash
   pip install -r requirements.txt
   ```

6. Import the required libraries and load the CSV dataset into Pandas.

7. Follow the data exploration, cleaning, feature engineering, database loading, and SQL analysis steps described above.

---

## Project Structure

```plaintext
|-- Walmart Project/
    |-- walmart.csv             # Walmart sales dataset
    |-- walmart_analysis.ipynb  # Jupyter Notebook
    |-- sql_queries/             # SQL scripts for analysis and queries
    |-- README.md                # Project documentation
    |-- requirements.txt         # List of required Python libraries
```

---

## Results and Insights

This section will include the analysis findings:

* **Sales Insights**: Key categories, branches with highest sales, and preferred payment methods.
* **Profitability**: Insights into the most profitable product categories and locations.
* **Customer Behavior**: Trends in ratings, payment preferences, and peak shopping hours.

---

## Future Enhancements

Possible extensions to this project:

* Integration with a dashboard tool (e.g., Power BI or Tableau) for interactive visualization.
* Additional data sources to enhance analysis depth.
* Automation of the data pipeline for real-time data ingestion and analysis.

---

## License

This project is licensed under the MIT License.

---

## Acknowledgments

* **Data Source**: Kaggle's Walmart Sales Dataset
* **Inspiration**: Walmart's business case studies on sales and supply chain optimization.

---
