# Superstore Data Analysis Project

## Project Overview
This project involves analyzing sales data from a superstore to gain insights into sales trends, customer behavior, and regional performance. The primary focus is on cleaning, exploring, and visualizing the data to inform business decisions.

---

## Dataset Overview
The dataset consists of transactional data from a superstore. Below are the key columns in the dataset:

| Column Name     | Description                              |
|-----------------|------------------------------------------|
| Row ID          | Unique identifier for each row.         |
| Order ID        | Unique identifier for each order.       |
| Order Date      | Date when the order was placed.         |
| Ship Date       | Date when the order was shipped.        |
| Ship Mode       | Mode of shipping (e.g., Standard Class).|
| Customer ID     | Unique identifier for each customer.    |
| Customer Name   | Name of the customer.                   |
| Segment         | Customer segment (e.g., Consumer).      |
| Country         | Country of the customer.                |
| City            | City of the customer.                   |
| State           | State of the customer.                  |
| Postal Code     | Postal code of the customer.            |
| Region          | Region of the customer.                 |
| Product ID      | Unique identifier for each product.     |
| Category        | Category of the product.                |
| Sub-Category    | Sub-category of the product.            |
| Product Name    | Name of the product.                    |
| Sales           | Sales amount for the transaction.       |

### Sample Data
Below is a sample of the dataset:

| Row ID | Order ID        | Order Date | Ship Date | Ship Mode       | Customer ID | Customer Name      | Segment     | Country       | City          | State       | Postal Code | Region | Product ID       | Category        | Sub-Category | Product Name                                                            | Sales   |
|--------|-----------------|------------|-----------|-----------------|-------------|--------------------|-------------|---------------|---------------|-------------|-------------|--------|------------------|-----------------|-------------|------------------------------------------------------------------------|---------|
| 1      | CA-2017-152156 | 08-11-2017 | 11-11-2017 | Second Class    | CG-12520    | Claire Gute       | Consumer    | United States | Henderson     | Kentucky    | 42420       | South  | FUR-BO-10001798  | Furniture       | Bookcases   | Bush Somerset Collection Bookcase                                     | 261.96  |
| 2      | CA-2017-152156 | 08-11-2017 | 11-11-2017 | Second Class    | CG-12520    | Claire Gute       | Consumer    | United States | Henderson     | Kentucky    | 42420       | South  | FUR-CH-10000454  | Furniture       | Chairs      | Hon Deluxe Fabric Upholstered Stacking Chairs, Rounded Back           | 731.94  |
| 3      | CA-2017-138688 | 12-06-2017 | 16-06-2017 | Second Class    | DV-13045    | Darrin Van Huff   | Corporate   | United States | Los Angeles   | California  | 90036       | West   | OFF-LA-10000240  | Office Supplies | Labels      | Self-Adhesive Address Labels for Typewriters by Universal             | 14.62   |
| 4      | US-2016-108966 | 11-10-2016 | 18-10-2016 | Standard Class  | SO-20335    | Sean O'Donnell    | Consumer    | United States | Fort Lauderdale| Florida     | 33311       | South  | FUR-TA-10000577  | Furniture       | Tables      | Bretford CR4500 Series Slim Rectangular Table                         | 957.58  |
| 5      | US-2016-108966 | 11-10-2016 | 18-10-2016 | Standard Class  | SO-20335    | Sean O'Donnell    | Consumer    | United States | Fort Lauderdale| Florida     | 33311       | South  | OFF-ST-10000760  | Office Supplies | Storage     | Eldon Fold 'N Roll Cart System                                        | 22.37   |
| 6      | CA-2015-115812 | 09-06-2015 | 14-06-2015 | Standard Class  | BH-11710    | Brosina Hoffman   | Consumer    | United States | Los Angeles   | California  | 90032       | West   | FUR-FU-10001487  | Furniture       | Furnishings | Eldon Expressions Wood and Plastic Desk Accessories, Cherry Wood      | 48.86   |

---

## Steps Performed

### 1. Data Cleaning
- Identified and handled missing values in the `Postal Code` column.
- Converted `Order Date` and `Ship Date` columns to the correct date format.
- Removed duplicate rows from the dataset.

### 2. Exploratory Data Analysis (EDA)
- **Univariate Analysis:**
  - Visualized sales distribution using histograms.
  - Analyzed category frequency using bar charts.
- **Bivariate Analysis:**
  - Examined the relationship between sales and region.
  - Analyzed the relationship between sales and product category.
- **Time Series Analysis:**
  - Created a `YearMonth` column and plotted monthly sales trends.

### 3. Feature Engineering
- Created new features such as:
  - **Shipping Time:** Days between order and shipping.
  - **Average Order Value (AOV):** Average sales per order.

### 4. Data Visualization
- Visualized top 10 products by sales using horizontal bar charts.
- Created a heatmap of sales by region and category.

### 5. Automation
- Scheduled the analysis to run daily at a specific time using Python's `schedule` library.

---

## Findings and Insights
- Sales are highest in the "West" region and lowest in the "South" region.
- The "Office Supplies" category has the highest number of sales transactions.
- Monthly sales exhibit a consistent upward trend over the years.
- Products with faster shipping times tend to have higher sales.

---

## Technologies Used
- **Python Libraries:** pandas, numpy, matplotlib, seaborn, schedule
- **Tools:** Jupyter Notebook

---

## How to Run the Project
1. Clone this repository.
2. Ensure all required Python libraries are installed.
3. Run the Jupyter Notebook `superstore_analysis.ipynb` to execute the analysis.

---

## Future Scope
- Incorporate machine learning models to predict sales trends.
- Add analysis on customer lifetime value.
- Explore profitability analysis by adding profit margin data.

---

## Contact
For any questions or suggestions, please reach out to [priyankakshayrajput@gmail.com].

