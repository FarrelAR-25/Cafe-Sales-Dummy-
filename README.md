# Cafe Sales Data Analysis & Data Cleaning

## Project Overview

This project focuses on analyzing cafe sales data through data cleaning, exploratory data analysis (EDA), and data visualization using Python.

The dataset contains cafe transaction records with several data quality issues, including missing values, inconsistent entries (`UNKNOWN` and `ERROR`), and incorrect data types.

The main objective of this project is to transform raw transaction data into a clean and structured dataset, explore sales performance, identify customer purchasing patterns, and generate business insights that can support better decision-making.

## Objectives

- Understand the structure and characteristics of the cafe sales dataset.
- Identify and handle missing values and inconsistent data.
- Convert columns into appropriate data types.
- Perform data cleaning and data preprocessing.
- Explore sales performance across different products.
- Analyze customer payment methods and purchasing locations.
- Visualize sales distributions, trends, and correlations.
- Generate actionable business insights and recommendations.

## Dataset

**Dataset:** `dirty_cafe_sales.csv`

The dataset consists of 10,000 transaction records and 8 columns.

| Column | Description |
|---|---|
| Transaction ID | Unique transaction identifier |
| Item | Product purchased by the customer |
| Quantity | Number of products purchased |
| Price Per Unit | Price of each product |
| Total Spent | Total transaction amount |
| Payment Method | Payment method used |
| Location | Purchasing method or location |
| Transaction Date | Date of the transaction |

**Data Source:** Cafe Sales Dummy Dataset.

## Tools & Technologies

The following tools and Python libraries were used:

- **Python** – Main programming language.
- **Google Colab / Jupyter Notebook** – Development environment.
- **Pandas** – Data manipulation and cleaning.
- **NumPy** – Numerical operations.
- **Matplotlib** – Data visualization.
- **Seaborn** – Statistical data visualization.

## Project Workflow

### 1. Data Understanding

The initial stage involves understanding the dataset structure and identifying potential data quality issues.

Activities:
- Display the first and last five records.
- Check dataset dimensions.
- Inspect column names and data types.
- Generate descriptive statistics.
- Identify missing values.
- Detect inconsistent entries such as `UNKNOWN` and `ERROR`.

### 2. Data Cleaning

Several preprocessing techniques were applied to improve data quality.

**Handling inconsistent values**
- Replace `UNKNOWN` with `NaN`.
- Replace `ERROR` with `NaN`.

**Data type conversion**
- Convert `Quantity` into numeric.
- Convert `Price Per Unit` into numeric.
- Convert `Total Spent` into numeric.
- Convert `Transaction Date` into datetime format.

**Handling missing values**
- Numerical columns were filled using the median.
- Categorical columns were filled using the mode.
- Missing transaction dates were filled using the mode.

**Duplicate and missing value validation**
- Check duplicated records.
- Recheck missing values after preprocessing.

### 3. Exploratory Data Analysis (EDA)

EDA was performed to understand cafe sales performance and customer purchasing behavior.

The analysis includes:

- Product sales frequency.
- Total sales by product.
- Customer payment methods.
- Purchasing locations.
- Transaction amount distribution.
- Outlier identification.
- Daily sales trends.
- Correlation between numerical variables.

### 4. Data Visualization

Several visualizations were created to communicate the analytical findings:

| Visualization | Purpose |
|---|---|
| Count Plot | Identify the most frequently purchased products |
| Bar Chart | Compare total sales by product |
| Bar Chart | Analyze payment methods |
| Bar Chart | Compare purchasing locations |
| Histogram | Understand transaction amount distribution |
| Box Plot | Identify potential outliers |
| Line Chart | Analyze daily sales trends |
| Heatmap | Examine correlations between numerical variables |

## Key Findings & Business Insights

Based on the exploratory data analysis, several findings were identified:

**1. Product Performance**

Juice recorded the highest total sales, followed by Salad and Sandwich. Meanwhile, Cookie had the lowest total sales.

*Business Recommendation:* Prioritize inventory management for high-performing products such as Juice. Consider promotional campaigns and product bundling to increase sales of lower-performing products.

**2. Product Purchase Frequency**

Juice was also identified as the most frequently purchased product.

*Business Recommendation:* Maintain sufficient stock availability to meet customer demand.

**3. Customer Purchasing Behavior**

The analysis compared payment methods and purchasing locations to understand customer preferences.

*Business Recommendation:* Improve payment convenience and optimize takeaway services based on customer purchasing patterns.

**4. Transaction Distribution**

The histogram and box plot were used to examine transaction values and identify potential outliers.

*Business Recommendation:* Investigate unusually high transaction values to better understand customer purchasing behavior.

**5. Daily Sales Trends**

Daily sales were analyzed throughout 2023 to observe fluctuations in cafe revenue.

*Business Recommendation:* Use sales trends to support inventory planning and promotional scheduling.

**6. Correlation Analysis**

The correlation heatmap indicates a positive relationship between Quantity and Total Spent.

*Business Recommendation:* Consider product bundling and promotional strategies to encourage customers to purchase more items per transaction.

## Data Cleaning Results

After the preprocessing process:

- Total records: 10,000.
- Total columns: 8.
- Missing values: 0.
- Duplicate records detected: 0.
- Numerical and date columns converted into appropriate data types.
- Inconsistent values handled through preprocessing.

The cleaned dataset was exported as:

`clean_cafe_sales.csv`

## Project Files

```text
Cafe-Sales-Data-Analysis/
│
├── Data Cafe (Dummy).ipynb
├── dirty_cafe_sales.csv
├── clean_cafe_sales.csv
└── README.md
```

## How to Run the Project

1. Clone this repository:

```bash
git clone https://github.com/your-username/your-repository.git
```

2. Navigate to the project directory:

```bash
cd your-repository
```

3. Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn
```

4. Open the notebook using Google Colab or Jupyter Notebook.

5. Make sure `dirty_cafe_sales.csv` is located in the same directory as the notebook.

6. Run the notebook cells sequentially to reproduce the data cleaning, analysis, and visualization process.

## Conclusion

This project demonstrates the application of Python for data cleaning, exploratory data analysis, and data visualization in a cafe sales context.

Through this analysis, raw transaction data was transformed into a cleaner and more structured dataset, allowing sales performance and customer purchasing patterns to be explored.

The findings can provide useful insights for cafe management, particularly in product inventory planning, sales optimization, and customer service improvement.

---

**Project Category:** Data Analytics / Exploratory Data Analysis (EDA)  
**Programming Language:** Python  
**Environment:** Google Colab  
**Dataset Type:** Dummy Cafe Sales Dataset
