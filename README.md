# 📊 Retail Store Sales Data Analysis

This project involves an end-to-end analysis of a sample retail store sales dataset to uncover key performance metrics, customer behavior patterns, and sales trends using Python and popular data science libraries.

## 🎯 Project Objectives

* **Data Exploration:** Understand the dataset structure, dimensions, and data types.
* **Data Cleaning & Preprocessing:** Handle missing values, garbage values, and outliers to ensure data quality.
* **Feature Engineering:** Extract time-based features (`Year`, `Month`, `Day`) from the transaction date for deeper analysis.
* **Exploratory Data Analysis (EDA):** Generate meaningful business insights through visualization and aggregation.
* **Strategic Insights:** Provide actionable recommendations based on the findings.

## 💾 Dataset Details

The dataset contains sales information with the following key columns:

| Column Name | Description | Data Type (Post-Cleaning) |
| :--- | :--- | :--- |
| **Transaction ID** | Unique identifier for each transaction. | `Object` |
| **Customer ID** | Unique identifier for each customer. | `Object` |
| **Category** | Product category (e.g., Patisserie, Butchers, Food). | `Object` |
| **Price Per Unit** | Price of the item. | `Float64` |
| **Quantity** | Number of units sold. | `Float64` |
| **Total Spent** | Total revenue from the transaction. | `Float64` |
| **Payment Method** | Method used for payment (Cash, Credit Card, Digital Wallet). | `Object` |
| **Location** | Purchase location (Online, In-store). | `Object` |
| **Transaction Date** | Date of the transaction. | `Datetime` |
| **Discount Applied** | Boolean flag indicating if a discount was applied. | `Boolean` |

## ✨ Key Analysis & Insights

The analysis was performed after rigorous data cleaning, including filling missing values in `Item` (with mode), `Price Per Unit`, `Quantity`, `Total Spent` (calculated), and removing 60 outliers in the `Total Spent` column.

### Top Findings:

* **Highest Sales Month:** **January** showed the maximum total sales, significantly outperforming other months.
* **Top Revenue Category:** The **Butchers** category generated the highest total revenue, followed closely by **Electric Household Essentials**.
* **Top Volume Category:** **Furniture** and **Food** were the most sold categories in terms of quantity.
* **Payment & Location Trends:**
    * **Cash** is the dominant payment method, especially on high-sales days (Friday, Saturday, Sunday).
    * **In-store** purchases are preferred for categories like **Furniture** and **Milk Products**.
    * **Online** purchases dominate for **Computers and Electric Accessories**.
* **High Sales Days:** **Friday, Saturday, and Sunday** are the peak days for sales amount.

## 🛠️ Tools and Libraries Used

* **Python**
* **Pandas:** For data manipulation and cleaning.
* **NumPy:** For numerical operations.
* **Matplotlib:** For static visualizations.
* **Seaborn:** For enhanced statistical data visualization.

## 🖼️ Visualizations

Below are some of the key visualizations generated during the EDA phase:

| Visualization | Description |
| :--- | :--- |
| **Total Sales By Month** | Bar chart showing January as the clear leader. |
| **Total Amount of Purchase by Category** | Bar chart highlighting Butchers as the top revenue generator. |
| **Usage of Payment Method (Pie Chart)** | Showing the near-equal split, with Cash slightly dominating. |
| **Total Quantity by each Category** | Line plot indicating Furniture and Food volume dominance. |
| **Mostly Used Location for each Category** | Count plot revealing In-store vs. Online preferences. |
| **Sales by Days of Week** | Bar plot confirming weekend spikes in sales. |

## 🚀 How to Run the Project

1.  **Clone the Repository:**
    ```bash
    git clone [Your-Repo-Link]
    ```
2.  **Install Dependencies:**
    ```bash
    pip install pandas numpy matplotlib seaborn
    ```
3.  **Run the Notebook:**
    Open the `retail_store_sales_analysis.ipynb` file in Jupyter Notebook or JupyterLab and run the cells sequentially.

## 📝 Future Scope

* Perform customer segmentation (e.g., using RFM analysis).
* Implement time series forecasting to predict future sales.
* Analyze the impact of 'Discount Applied' on 'Quantity' and 'Total Spent'.
