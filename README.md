# FRAJO-ENTERPRISE-LIMITED-SALES-ANALYSIS-ON-MOCROSOFT-EXCEL
A data analytics project exploring Frajo Enterprise Limited Sales performance, sales by subcategory, Profit gained overtime, Monthly, Top 5 customers, Sales by State, Unique Customers, insights through data visualization.
The data was gotten from gaggle.com and below are the steps i took working on the dataset before the eventual visualization
1. Data Collection / Import
Imported the raw US Sales dataset into Excel.
Identified the available fields and the structure of the dataset.
Established that the dataset contains sales transaction-level information.
2. Data Understanding

I first identified what each column represents:

Field	Purpose
Order Date	Determines when the sale occurred
Customer Name	Identifies the customer
State	Identifies the customer's/location's state
Category	Groups products into major product categories
Sub-Category	Provides a more detailed product classification
Product Name	Identifies the individual product
Sales	Measures revenue generated
Quantity	Measures units sold
Profit	Measures profitability

This establishes the dimensions and measures needed for analysis.
3. Data Quality Assessment

Before transforming anything, the dataset was checked for quality issues.

Missing values
Checked every column for blanks/null values.
The dataset does not have missing values in these nine fields.
Duplicate records
Checked for duplicate rows.
A duplicate record was identified and should be investigated/removed if confirmed to be an accidental duplicate.
Data consistency

Checked for:

Consistent category names
Consistent state names
Consistent customer names
Consistent product names
Appropriate numerical values
Correct date entries
4. Data Type Validation

Each field was assigned the appropriate data type.

Categorical/Text fields
Customer Name
State
Category
Sub-Category
Product Name
Date field
Order Date
Numerical fields
Sales → Decimal/Currency
Quantity → Whole Number
Profit → Decimal/Currency

This is important because incorrect data types can affect calculations and visualizations.

5. Date Transformation
6. The Order Date field is particularly important because it allows us to analyze sales and profit over time.

I would transform it into:
Year
Month

This allows analysis such as:

Sales by Year → Sales by Quarter → Sales by Month

and makes it possible to identify trends and seasonality.
6. Product Categorization

The dataset already contains:

Category → Sub-Category → Product Name

This gives us a natural hierarchy.

For example:

Category
↓
Sub-Category
↓
Product

This allows us to analyze performance at different levels rather than treating every product individually.
7. Geographic Transformation

The State field was identified as the primary geographical dimension.

This allows the data to be analyzed according to:

State → Sales → Quantity → Profit
8. Customer Analysis Preparation

Customer Name was identified as a key customer dimension.

This allows us to determine:

Top customers by sales
Top customers by profit
Customer contribution to total sales
Customer purchasing patterns

A unique customer count can also be created as a KPI.
9. Creation of Analytical Measures

The raw fields are not enough for a complete analysis, so key measures should be created.

Total Sales

Sum of all sales transactions.

Total Profit

Sum of all profit generated.

Total Quantity

Total units sold.

Unique Customers

Distinct count of customers.

Average Sales

Average sales per transaction.

Profit Margin

A particularly useful measure:

Profit Margin = Total Profit ÷ Total Sales

This helps distinguish between products that generate high sales and products that generate high profitability.
10. Exploratory Data Analysis

Before deciding on visualizations, the dataset was explored from several perspectives.

Sales analysis
Sales over time
Sales by category
Sales by sub-category
Sales by product
Sales by state
Sales by customer
Profit analysis
Profit over time
Profit by category
Profit by sub-category
Profit by product
Profit by state
Quantity analysis
Quantity by category
Quantity by sub-category
Quantity by product
Customer analysis
Top customers
Customer sales contribution
Customer profitability
11. Identify Business Questions

After exploring the dataset, the analysis should move from:

"What does the data contain?"

to:

"What business questions can the data answer?"

For this dataset, the major questions are:

Sales Performance

How are sales performing over time?

Product Performance

Which categories, sub-categories and products drive sales?

Profitability

Which products generate profit and which may be hurting profitability?

Customer Performance

Which customers contribute most to revenue and profit?

Geographic Performance

Which states are the strongest and weakest markets?

Volume

Which products/categories have the highest quantities sold?
12. Identify Key Insights

This is where the analysis becomes meaningful.

You compare dimensions against measures:

Category → Sales

Category → Profit

Sub-Category → Sales

Sub-Category → Profit

Product → Sales

Product → Profit

Customer → Sales

State → Sales

State → Profit

Date → Sales

Date → Profit

The purpose is to identify patterns, trends, relationships, outliers and underperforming areas.
13. Determine the Appropriate Visualization

Only after the analysis do we decide what should become a visual.
14. Build Pivot Tables / Analytical Summaries

Before the final dashboard, the data can be summarized using PivotTables.

For example:

Sales by Category

Rows: Category
Values: Sum of Sales

Profit by Sub-Category

Rows: Sub-Category
Values: Sum of Profit
15. Validate the Results

Before creating the final dashboard:

Verify total sales against the original dataset.
Verify total profit.
Check total quantity.
Confirm customer counts.
Confirm categories and sub-categories.
Check date groupings.
Check that duplicate records have been handled.
Check calculations and measures.
Investigate unusual/outlier results.

This ensures the dashboard is accurate before it is presented.
16. Data Visualization

Only after completing all those steps do we move to visualization.

So your actual project workflow can be presented very simply as:

Raw Data
↓
Data Understanding
↓
Data Quality Check
↓
Data Cleaning
↓
Data Type Validation
↓
Data Transformation
↓
Calculated Measures
↓
Exploratory Analysis
↓
Business Questions
↓
Key Insights
↓
Pivot Tables / Data Summaries
↓
Validation
↓
Visualization.
