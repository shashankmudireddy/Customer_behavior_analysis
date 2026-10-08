# Retail Customer Shopping Behavior Analysis

## Overview

This project is an end-to-end **Data Analytics project** focused on understanding customer shopping behavior and identifying useful business insights from retail transaction data.

The project covers the complete analytics workflow, starting from **loading and exploring the dataset using Python**, followed by **data cleaning and preparation**, **SQL-based analysis**, and the creation of an interactive **Power BI dashboard**. A detailed project report and presentation were also created to communicate the findings clearly.

The main objective is to transform raw customer data into meaningful insights that can support better business decisions.

---

## Dataset

The dataset contains customer shopping and transaction information, including:

* Customer ID
* Age
* Gender
* Item Purchased
* Category
* Purchase Amount
* Location
* Size
* Color
* Season
* Review Rating
* Subscription Status
* Shipping Type
* Discount Applied
* Previous Purchases
* Payment Method
* Frequency of Purchases

The dataset was inspected and cleaned before performing further analysis.

---

## Tools & Technologies

* **Python** – Data loading, cleaning, and analysis
* **Pandas** – Data manipulation and preprocessing
* **Jupyter Notebook** – Data analysis and EDA
* **MySQL / PostgreSQL / SQL Server** – SQL-based business analysis
* **SQL** – Data querying and extracting insights
* **Power BI** – Interactive dashboard and data visualization
* **Gamma** – Project presentation/PPT creation
* **GitHub** – Project documentation and version control

---

## Project Workflow

```text
Raw Dataset
     ↓
Load Data using Python
     ↓
Data Exploration
     ↓
Data Cleaning & Transformation
     ↓
Exploratory Data Analysis (EDA)
     ↓
Load Data into SQL Database
     ↓
SQL Business Analysis
     ↓
Power BI Dashboard
     ↓
Business Insights
     ↓
Project Report & Presentation
```

---

## Steps Performed

### 1. Data Loading

The dataset was loaded into a Jupyter Notebook using Python and Pandas.

```python
import pandas as pd

df = pd.read_csv("customer_shopping_behavior.csv")

print(df.head())
print(df.shape)
```

The initial dataset was examined to understand its structure, columns, data types, and number of records.

---

### 2. Exploratory Data Analysis

EDA was performed to understand the data and identify important patterns.

The analysis included:

* Checking dataset shape
* Understanding column names
* Checking data types
* Identifying missing values
* Checking duplicate records
* Examining unique values
* Analyzing numerical columns
* Studying categorical variables
* Understanding customer purchasing patterns

Example:

```python
df.info()
df.describe()
df.isnull().sum()
df.duplicated().sum()
```

---

### 3. Data Cleaning

The dataset was cleaned before performing business analysis.

The cleaning process included:

* Handling missing values
* Removing unnecessary columns
* Checking duplicate records
* Correcting data types where required
* Standardizing column names
* Preparing the data for SQL analysis and visualization

The cleaned dataset was then used for further analysis.

---

### 4. SQL Analysis

The cleaned data was loaded into a relational database such as **MySQL, PostgreSQL, or SQL Server**.

SQL queries were used to answer business-related questions and identify useful patterns.

Analysis included:

* Total sales and purchase amount
* Customer purchasing behavior
* Sales by category
* Sales by location
* Sales by season
* Customer subscription analysis
* Discount analysis
* Payment method analysis
* Purchase frequency
* Customer ratings
* Previous purchase behavior

Example SQL query:

```sql
SELECT
    Category,
    SUM(Purchase_Amount_USD) AS Total_Sales
FROM customer_shopping
GROUP BY Category
ORDER BY Total_Sales DESC;
```

SQL helped convert the cleaned dataset into meaningful business insights.

---

## Power BI Dashboard

An interactive **Power BI dashboard** was created to present the key findings visually.

The dashboard includes visualizations for areas such as:

* Total Sales
* Customer Count
* Sales by Category
* Sales by Season
* Sales by Location
* Customer Purchasing Behavior
* Discount Analysis
* Subscription Status
* Payment Methods
* Purchase Frequency

Interactive filters and visuals allow users to explore the data from different perspectives.

---

## Results & Insights

The analysis helped identify important patterns in customer shopping behavior.

Key areas analyzed include:

* Which product categories generate higher sales
* How customer purchasing behavior changes across seasons
* The relationship between discounts and purchases
* Customer preferences across different locations
* Popular payment methods
* Subscription and non-subscription customer behavior
* Customer purchase frequency
* Customer ratings and purchasing patterns

These insights can help businesses better understand their customers and make data-driven decisions related to sales, marketing, discounts, and customer engagement.

---

## Project Report

A detailed project report was prepared covering:

* Business Problem
* Dataset Description
* Data Cleaning
* Exploratory Data Analysis
* SQL Analysis
* Power BI Dashboard
* Key Findings
* Business Insights
* Conclusion

---

## Presentation

A professional project presentation was created using **Gamma** to summarize the project.

The presentation covers:

* Project Objective
* Dataset
* Tools Used
* Data Preparation
* EDA
* SQL Analysis
* Power BI Dashboard
* Key Insights
* Conclusion

---

## How to Run

### Step 1: Clone the Repository

```bash
git clone <your-github-repository-url>
```

### Step 2: Install Required Python Libraries

```bash
pip install pandas numpy matplotlib seaborn
```

### Step 3: Open the Jupyter Notebook

Open the project notebook:

```text
customer_shopping_behavior.ipynb
```

### Step 4: Add the Dataset

Place the dataset in the appropriate project folder:

```text
data/
└── customer_shopping_behavior.csv
```

### Step 5: Run the Python Analysis

Run the notebook cells in order to:

* Load the dataset
* Explore the data
* Clean the data
* Perform EDA
* Prepare the final dataset

### Step 6: Set Up the SQL Database

Create the database and table in your selected database system.

Then load the cleaned dataset into the database.

### Step 7: Run SQL Queries

Execute the SQL scripts provided in the project to perform business analysis.

### Step 8: Open the Power BI Dashboard

Open the `.pbix` file in **Power BI Desktop**.

Update the data source connection if required and refresh the dashboard.

---

## Project Structure

```text
Retail-Customer-Shopping-Analysis/
│
├── data/
│   └── customer_shopping_behavior.csv
│
├── notebooks/
│   └── customer_shopping_behavior.ipynb
│
├── sql/
│   └── customer_analysis.sql
│
├── powerbi/
│   └── customer_shopping_dashboard.pbix
│
├── report/
│   └── project_report.pdf
│
├── presentation/
│   └── project_presentation.pdf
│
└── README.md
```

---

## Skills Demonstrated

* Python
* Pandas
* Data Cleaning
* Exploratory Data Analysis
* SQL
* MySQL / PostgreSQL / SQL Server
* Data Visualization
* Power BI
* Business Analysis
* Data Interpretation
* Report Preparation
* Presentation Development

---

## Conclusion

This project demonstrates a complete **data analytics workflow**, from raw data preparation to business insights and visualization.

By combining **Python, SQL, and Power BI**, the project shows how raw customer data can be transformed into meaningful information that supports business decision-making.

It demonstrates practical skills in **data cleaning, exploratory analysis, SQL querying, visualization, and communicating analytical findings**.
