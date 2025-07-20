# Motorcycle Sales Analysis

![Parked motorcycle](motorcycle.jpg)

## 📊 Project Overview

This project analyzes sales data from a company that sells motorcycle parts through three warehouses—North, Central, and West. The focus is on understanding **net revenue** generated from **wholesale orders**, broken down by **product line**, **month**, and **warehouse**.

The analysis involves querying a SQL-style `sales` table that includes information such as order details, payment methods, and payment fees.

---

## 🧾 Dataset Description

The `sales` table includes the following columns:

| Column         | Description                                             |
|----------------|---------------------------------------------------------|
| order_number   | Unique order number                                     |
| date           | Date of the order (from June to August 2021)            |
| warehouse      | Warehouse location (`North`, `Central`, or `West`)      |
| client_type    | `Retail` or `Wholesale`                                 |
| product_line   | Category of motorcycle parts                            |
| quantity       | Number of products ordered                              |
| unit_price     | Price per product (USD)                                 |
| total          | Total price of the order (USD)                          |
| payment        | Payment method (`Credit card`, `Transfer`, or `Cash`)   |
| payment_fee    | Percentage fee applied based on the payment method      |

---

## 🎯 Goal

To calculate and visualize the **net revenue** from **wholesale clients** by:

- Product line
- Month
- Warehouse

Net revenue is computed as:

net_revenue = total - (total * payment_fee)

---

## ⚙️ Technologies Used

- Python
- Jupyter Notebook
- Pandas
- SQL (via SQLite or simulated queries)
- Data visualization (optional: Seaborn / Matplotlib)

---

## ✅ Results Summary

The output includes a grouped table of net revenues with the following columns:

- `product_line`
- `month`
- `warehouse`
- `net_revenue`

Filtered to include only `Wholesale` clients.

---

## 📌 Future Improvements

- Add interactive dashboards with Power BI or Plotly
- Include Retail analysis for comparison
- Automate the pipeline using Python scripts

---

## 📬 Contact

For feedback or collaboration, feel free to reach out!

---

### 📦 `requirements.txt`

```txt
pandas
jupyter
matplotlib
seaborn
sqlalchemy

