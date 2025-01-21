# SQL--sales_Analysis
# Madhav Shop Sales Analysis

This project analyzes sales data from Madhav Shop to understand customer behavior and product performance. The analysis focuses on identifying key demographic trends and product preferences to provide actionable business insights.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Data Cleaning (If Applicable)](#data-cleaning)
- [Tools and Technologies](#tools-and-technologies)
- [Project Structure](#project-structure)
- [Installation and Setup](#installation-and-setup)
- [Data Analysis Process](#data-analysis-process)
- [Key Findings](#key-findings)
- [Visualizations](#visualizations)
- [Future Improvements](#future-improvements)

## Project Overview

This project analyzes Madhav Shop's sales data to understand customer purchasing patterns and product popularity. By examining sales trends based on state, gender, marital status, occupation, product, and product ID, the project aims to generate actionable insights into customer demographics and product preferences. These insights can inform targeted marketing campaigns, optimize inventory management, and contribute to overall business strategy.

## Dataset

The dataset used is "Madhav Sales Data," stored as an Excel file (`Madhav Sales Data.xlsx`). It includes the following information:

*   `Product-ID`: A unique identifier for each product.
*   `Product Bought`: The name or description of the purchased product.
*   `State`: The state where the purchase was made.
*   `Gender`: The customer's gender.
*   `Marital Status`: The customer's marital status.
*   `Occupation`: The customer's occupation.

* The dataset contains approximately 11239 rows and 13 columns.

## Data Cleaning 

*   Identified and addressed missing values (e.g., through imputation or removal).
*   Ensured consistent data types (e.g., converting dates to datetime format).
*   Resolved any data inconsistencies or errors.

## Tools and Technologies

*   **Programming Language:** Python
*   **Libraries/Packages:**
    *   `mysql-connector-python`: For connecting to a MySQL database (if applicable).
    *   `NumPy`: For numerical computing.
    *   `Pandas`: For data manipulation and analysis.
    *   `Matplotlib`: For creating static, interactive, and animated visualizations in Python.
    *   `Seaborn`: For data visualization based on matplotlib, providing a high-level interface for drawing attractive and informative statistical graphics.
*   **Data Storage:** Excel file (`Madhav Sales Data.xlsx`)

## Project Structure

The project files are organized as follows:

*   `Madhav Sales Data.xlsx`: Contains the sales data.
*   `Python-sql project.ipynb`: The Jupyter Notebook containing the Python code for data analysis and visualization.

## Installation and Setup

To run the Jupyter Notebook, you'll need to install the required Python packages. Using a virtual environment is strongly recommended:

1.  **Create a virtual environment (recommended):**
    *   Linux/macOS: `python3 -m venv venv`
    *   Windows: `python -m venv venv`
2.  **Activate the virtual environment:**
    *   Linux/macOS: `source venv/bin/activate`
    *   Windows: `venv\Scripts\activate`
3.  **Install the necessary packages:**
    ```bash
    pip install pandas numpy matplotlib seaborn mysql-connector-python
    ```
4.  **Ensure the `Madhav Sales Data.xlsx` file is in the same directory as the `Sales-data- Analysis.ipynb` file.**

## Data Analysis Process

1.  **Data Loading:** The sales data was loaded from the Excel file into a Pandas DataFrame.
2.  **Data Exploration:** Initial data exploration was performed to understand the data's structure and identify any potential issues.
3.  **Data Cleaning (If Applicable):** **   Identified and addressed missing values (e.g., through imputation or removal).
*   Ensured consistent data types (e.g., converting dates to datetime format).
*   Resolved any data inconsistencies or errors.*
4.  **Data Analysis and Visualization:** Python libraries (Pandas, Matplotlib, and Seaborn) were used to analyze the data and create visualizations to reveal key trends and patterns. This included analyzing sales by state, gender, marital status, occupation, product, and product ID.
5.  **SQL Queries:**
SELECT * FROM sales.madhav_sales_data;
use madhav_sales_data;
use sales;
select count(*) from sales.madhav_sales_data;

## Key Findings

The analysis indicated that unmarried women aged 26-30 from Uttar Pradesh working in the IT sector are the most frequent purchasers at Madhav Shop.

*   Uttar Pradesh demonstrated the highest sales volume compared to other states.
*   Product ID [P00265242] was the top-selling product within this demographic.
*   Women Gender were spending more.

## Visualizations

Sales according to State
![Screenshot 2025-01-21 113927](https://github.com/user-attachments/assets/6cd63bc5-6de4-46d6-b96a-a80bad968126)

Sales according to Marrital Status Using Heat Map 1- Married, 0- unmarried
![Screenshot 2025-01-21 115039](https://github.com/user-attachments/assets/dcd8ecb9-11bc-4c2b-98cc-3016ddb0bad5)

Sales according to the Occupation of Customers
![Screenshot 2025-01-21 115322](https://github.com/user-attachments/assets/44045b54-c876-4007-b63a-ad1e2032ffe8)

Sales according to the products

![Screenshot 2025-01-21 115457](https://github.com/user-attachments/assets/a8b89746-69b6-4e5c-88d1-72bb2f6492be)
