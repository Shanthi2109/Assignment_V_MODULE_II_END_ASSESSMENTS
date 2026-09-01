# 🛍️ Online Retail Data Analysis & Business Insights

## 📌 Project Overview

This project focuses on analyzing an **Online Retail dataset** to understand customer purchasing behavior, sales trends, product performance, and business patterns.

As an aspiring **Data Scientist**, I developed a complete data analysis workflow that includes **data loading, data cleaning, feature engineering, exploratory data analysis (EDA), statistical analysis, data visualization, and business insight generation**.

The project uses Python libraries such as **Pandas, NumPy, Matplotlib, and Seaborn** to transform raw retail transaction data into meaningful insights that can support business decision-making.

The project is based on the **Online Retail Dataset from the UCI Repository**.

## 🎯 Project Objectives

The main objectives of this project are:

- Clean and preprocess real-world retail transaction data
- Handle missing values, duplicate records, and invalid values
- Perform exploratory data analysis (EDA)
- Create meaningful features from existing data
- Analyze customer and product behavior
- Perform statistical analysis
- Visualize important sales patterns and trends
- Identify high-value customers and top-selling products
- Generate actionable business insights
- Practice Git and GitHub project organization

These objectives align with the assignment requirements for data cleaning, feature engineering, data analysis, visualization, interpretation, and version control.

## 📊 Dataset

**Dataset:** Online Retail Dataset  
**Source:** UCI Machine Learning Repository

The dataset contains online retail transaction information, including:

- Invoice Number
- Product Description
- Quantity
- Invoice Date
- Unit Price
- Customer ID
- Country

The data represents customer transactions and provides information useful for studying sales trends, customer behavior, and product performance.

## 🛠️ Technologies & Tools Used

### Programming Language
- Python

### Libraries
- **Pandas** – Data manipulation and analysis
- **NumPy** – Numerical computations
- **Matplotlib** – Data visualization
- **Seaborn** – Statistical data visualization

### Development & Version Control
- Google Colab / Jupyter Notebook
- VS Code
- Git
- GitHub

# 🔍 Project Workflow

## 1. Data Import & Setup

The Online Retail dataset was loaded using Pandas.

The initial dataset was explored using:

- `head()`
- `tail()`
- `shape`
- `columns`
- `dtypes`

The `InvoiceDate` column was converted into datetime format for time-based analysis.
## 2. Data Cleaning

The following data-cleaning steps were performed:

### Missing Values
Rows with missing `CustomerID` values were removed.

### Duplicate Records
Duplicate transactions were identified and removed.

### Invalid Values
Transactions containing:

- Negative or zero quantities
- Invalid or zero unit prices

were removed from the analysis.

The cleaned dataset was then re-indexed.

These cleaning steps follow the assignment requirement to handle missing values, remove duplicates, and fix invalid quantity and price values.
## 3. Feature Engineering

New features were created to support deeper analysis.

### Total Price

A new `TotalPrice` column was created:

```text
TotalPrice = Quantity × UnitPrice
```

### Time-Based Features

The following features were extracted from `InvoiceDate`:

- Year
- Month
- Day
- Hour

### Customer Segmentation

Customers were categorized based on their total spending:

| Segment | Spending |
|---|---:|
| Low Value | < 500 |
| Medium Value | 500 – 1,999 |
| High Value | ≥ 2,000 |

### Order Size

Transactions were categorized according to quantity:

| Order Size | Quantity |
|---|---:|
| Small | ≤ 5 |
| Medium | 6 – 20 |
| Large | > 20 |

### Day Type

Transactions were classified as:

- Weekday
- Weekend

These derived features support customer, order, and time-based analysis.
# 📈 Exploratory Data Analysis

The dataset was explored using descriptive statistics and categorical analysis.

The analysis included:

- Dataset overview
- Descriptive statistics
- Country frequency analysis
- Customer segment analysis
- Order-size analysis
- Weekday vs. weekend transactions
- Sales by country
- Sales by month
- Top products by sales

Functions such as `describe()`, `value_counts()`, `unique()`, and `groupby()` were used throughout the analysis.


# 🔄 Data Wrangling

Data aggregation and restructuring were performed using Pandas.

The project includes:

- Customer-level sales aggregation
- Country-level sales aggregation
- Total spending calculation
- Total quantity calculation
- Number of orders calculation
- Top customer identification
- Top country identification
- Monthly sales by country using a pivot table

This helped transform transaction-level data into business-level summaries.


# 📊 Statistical Analysis

Statistical analysis was performed on:

- Quantity
- Unit Price
- Total Price

The following statistical measures were calculated:

- Mean
- Median
- Mode
- Standard deviation
- Variance
- 25th percentile
- 50th percentile
- 75th percentile
- 90th percentile
- 95th percentile

This helped understand the distribution and variability of retail transactions.

# 📉 Data Visualization

A total of **8 visualizations** were created using Matplotlib and Seaborn, meeting the assignment requirement of a minimum of eight plots.

## Matplotlib Visualizations

### 1. Line Chart – Monthly Sales

Shows the sales trend across different months.

### 2. Bar Chart – Top 10 Countries

Compares total sales across the top-performing countries.

### 3. Histogram – Quantity Distribution

Shows the distribution and frequency of quantities purchased.

### 4. Box Plot – Unit Price

Visualizes the distribution and spread of unit prices and helps identify potential outliers.

## Seaborn Visualizations

### 5. Count Plot – Transactions by Day Type

Compares transaction counts between weekdays and weekends.

### 6. Violin Plot – Total Price by Customer Segment

Shows the distribution of transaction values across customer segments.

### 7. Correlation Heatmap

Displays correlations between numerical variables such as:

- Quantity
- Unit Price
- Total Price
- Year
- Month
- Day
- Hour

### 8. Pair Plot – Numerical Variables

Visualizes pairwise relationships between:

- Quantity
- Unit Price
- Total Price


# 💡 Business Insights

Based on the analysis performed in the notebook, the following insights were identified:

### 🇬🇧 1. Top Country

**United Kingdom** is the top-performing country and generates the highest total sales.

### 📅 2. Best Sales Month

**November** is the best-performing sales month, indicating strong customer purchasing activity during this period.

### 🕛 3. Peak Sales Time

The analysis identifies approximately **12 PM** as the peak sales period.

### 👥 4. Customer Behavior

Customer spending varies considerably. A relatively smaller group of customers contributes a significant portion of revenue, while many customers make smaller purchases.

### 💎 5. High-Value Customers

Customers with high total spending and frequent orders represent valuable customers for the business.

These customers could be targeted through:

- Loyalty programs
- Personalized offers
- Exclusive promotions
- Customer retention strategies

### 🛒 6. Top Products

A relatively small number of products generate a large amount of sales.

Maintaining sufficient inventory for these products can help reduce the risk of stock shortages.

### 📢 7. Business Recommendation

The business should focus on:

- Retaining high-value customers
- Maintaining sufficient stock of top-selling products
- Running promotions during high-sales months
- Optimizing marketing activities around peak purchasing hours


# 📦 Requirements

The main Python libraries required for this project are:

```text
pandas
numpy
matplotlib
seaborn
openpyxl
```

Install them using:

```bash
pip install pandas numpy matplotlib seaborn openpyxl
```


# ▶️ How to Run the Project

### 1. Clone the repository

```bash
git clone <your-repository-link>
```

### 2. Navigate to the project folder

```bash
cd online-retail-data-analysis
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Open the notebook

Open:

```text
notebooks/Assignment_6.ipynb
```

You can run the notebook using **Jupyter Notebook, JupyterLab, VS Code, or Google Colab**.

### 5. Run the analysis

Execute the notebook cells sequentially to:

1. Load the dataset
2. Clean the data
3. Engineer new features
4. Explore the dataset
5. Perform statistical analysis
6. Generate visualizations
7. Extract business insights


# 🧠 Skills Demonstrated

This project demonstrates the following data science skills:

- Data Loading
- Data Cleaning
- Missing Value Handling
- Duplicate Removal
- Data Validation
- Feature Engineering
- Time-Based Analysis
- Exploratory Data Analysis
- Data Aggregation
- GroupBy Operations
- Statistical Analysis
- Data Visualization
- Business Insight Generation
- Python Programming
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Git & GitHub

The assignment evaluates these areas across data cleaning, feature engineering, data analysis, visualization, interpretation, and version control.

