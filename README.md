# Library

To conduct data analysis and visualization, the following libraries are utilized:

- `pandas`: A powerful data manipulation tool for data analysis.
- `numpy`: A library for numerical computations.
- `matplotlib.pyplot`: A plotting library for creating static, interactive, and animated visualizations.
- `seaborn`: A statistical data visualization library based on matplotlib for visually appealing statistical graphics.

# Read Data and Cleaning Data

## Read Data
To access and read the data from Google Sheets, the provided URL is transformed into a downloadable CSV format using the `replace()` method.

## Cleaning Data
1. The 'Date' column is converted to datetime format for time-series analysis.
2. A new column 'Revenue' is created by multiplying 'Unit price' with 'Quantity'.
3. Typos in categorical columns ('City' and 'Gender') are identified and corrected.

# Exploratory Data Analysis (EDA)

## Daily Trend Overall
The daily trend of revenue and quantity sold is examined to understand overall sales patterns.

1. **Matplotlib**: Line plots are utilized to visualize the trend of revenue over time.
2. **Seaborn**: Line plots are employed again for visualizing the trend of quantity sold over time.

## By Payment
Analysis is performed based on payment methods to understand revenue distribution and transaction volume.

1. Aggregation is done on payment methods to analyze total revenue and the count of unique invoices.
2. **Seaborn**: Bar plots are used to visualize revenue and invoice count by payment method.
3. **Pie Chart**: A pie chart is utilized to depict the distribution of revenue across different payment methods.

## By Gender and By Product Type
Analysis is conducted to understand sales patterns based on gender and product line.

1. Aggregation is performed on gender and product line to analyze the count of unique invoices.
2. **Seaborn**: Bar plots with hue differentiation are utilized to visualize the distribution of invoice counts by product line and gender.
