# Madhav E-Commerce Sales Dashboard 📊

## 📌 Project Overview
This project involves building an interactive **Sales Dashboard** using **Power BI** for "Madhav Store," an e-commerce business. The dashboard analyzes sales data to track key performance indicators (KPIs), identify regional trends, and monitor customer purchasing behavior.

The goal is to provide stakeholders with actionable insights to improve decision-making regarding inventory, sales strategies, and customer targeting.

## 🚀 Key Features
- **Interactive Dashboard:** Dynamic slicers for filtering data by **Quarters** and **States**.
- **KPI Tracking:** Real-time visualization of:
  - Total Revenue (Amount)
  - Total Profit
  - Total Quantity Sold
  - Average Order Value (AOV)
- **Advanced Visualizations:**
  - **Profit by Month:** Seasonal trend analysis using Bar Charts.
  - **Sales by Sub-Category:** identifying top-performing product categories.
  - **Customer Insights:** Top 4 high-value customers.
  - **Geographical Analysis:** Sales performance by State.
  - **Payment Mode Analysis:** Distribution of COD, UPI, Debit Card, etc.

## 🛠️ Tech Stack
- **Tool:** Power BI Desktop
- **Data Transformation:** Power Query Editor
- **Data Modeling:** Star Schema (connecting Orders and Details tables)
- **Calculations:** DAX (Data Analysis Expressions) for Custom Columns & Measures

## 📂 Dataset
The project uses sample data from "Madhav Store" containing two main tables:
1.  **Orders Table:** Order ID, Date, Customer Name, State, City.
2.  **Details Table:** Amount, Profit, Quantity, Category, Sub-Category, Payment Mode.

## ⚙️ Process Workflow
1.  **Data Import:** Imported raw CSV files (`Orders.csv` and `Details.csv`) into Power BI.
2.  **Data Cleaning (Power Query):**
    - Removed null values and duplicates.
    - Corrected data types (Dates, Numerical values).
    - Created custom columns for `Amount` and `Profit` calculations.
3.  **Data Modeling:** Established relationships between the `Orders` and `Details` tables using `Order ID`.
4.  **DAX Calculations:** Created Measures for `Average Order Value (AOV)` using the formula:
    ```DAX
    AOV = DIVIDE(SUM(Details[Amount]), SUM(Details[Quantity]))
    ```
5.  **Dashboard Design:** Implemented consistent theme, formatting, and navigation filters.

## 💡 Insights Derived
- Identify which months generate the highest profit to plan inventory.
- Determine the most popular payment modes (e.g., COD vs. Online) to optimize checkout processes.
- Recognize top-performing states to focus marketing efforts.

## 🤝 Contributing
Feel free to fork this repository and submit pull requests to improve the dashboard or add new features!

## 👤 Author
**Abhishek Singh**
- [LinkedIn](Your_LinkedIn_URL_Here)
- [Portfolio](Your_Portfolio_URL_Here)
