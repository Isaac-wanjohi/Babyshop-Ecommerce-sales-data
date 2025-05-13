# 🍼 Babyshop-Ecommerce-sales-data

📈 A deep-dive analysis of sales performance for an e-commerce venture that sells baby products to uncover trends and find useful insights to drive business decisions by the proprietors.


## 📂 Data Source

This project uses data from [Kaggle: Ecommerce sales data](https://www.kaggle.com/datasets/kaninigichuyia/ecommerce-sales-data?select=Sales+Data+November+2020+-+October+2023.xlsx), © Kaggle.
Please review the license and terms of use on Kaggle before using or distributing the data.

## 🔠 Project Description


This authentic retail transaction dataset meticulously compiles every transaction recorded over three years (November 2020 to October 2023) for a Kenyan-based and registered business specializing in selling baby products and related items. The dataset draws its specificity from actual operations of this venture, providing a comprehensive glimpse into the dynamics of its sales, sources, and overall business activities during the specified timeframe.


The dataset utilized for analysis originates from their Point of Sale (POS) system. This system captures a detailed account of various transactions, including product purchases, customer details, and timestamps, providing a rich and authentic source of data. The data collected from the POS system undergoes minimal transformations to ensure consistency and usability, maintaining the integrity of the information. This explicit provenance clarifies that the dataset is directly derived from the ecommerce venture's operational records at the point of sale, offering users a clear understanding of its source and enhancing its reusability for diverse analytical applications.

<details>
<summary><strong> 🧩Column Descriptions (Click to expand)</strong></summary>

<br>

- **`Order ID`**  
  A unique identifier assigned to each customer order for tracking and reference purposes.

- **`Sale ID`**  
  Identifier for the specific sale transaction, used to link related records.

- **`Date`**  
  The calendar date when the sale was completed or recorded.

- **`Order`**  
  Details of the customer’s order, typically linked to a **salesperson** for commission tracking.

- **`Transaction Type`**  
  Specifies the nature of the transaction — e.g., *Product Purchase*, *Shipping*, etc.

- **`Sale Type`**  
  Indicates the classification of the sale, such as a **purchase** or a **return**.

- **`Sales Channel`**  
  Platform used for the sale — e.g., **In-store**, **Online**, or payment methods like **Mpesa**, **Card**, or **Cash**.

- **`Product`**  
  Name or identifier of the specific item(s) sold.

- **`Net Quantity`**  
  Total units sold **excluding** any returned or discounted items.

- **`Gross Sales`**  
  Revenue **before** accounting for returns, discounts, or adjustments.

- **`Discounts`**  
  Total **discount value or percentage** applied to a transaction.

- **`Returns`**  
  Any product(s) returned by customers, including quantity and value details.

- **`Net Sales`**  
  Revenue **after** subtracting discounts and returns from gross sales.

- **`Shipping`**  
  Cost incurred for delivering the products to the customer (if applicable).

- **`Taxes`**  
  Tax component of the sale. *(Set to 0 in this dataset as all sales are VAT-inclusive.)*

- **`Total Sales`**  
  The complete sum of **Net Sales**, **Shipping**, and **Taxes**.  
  ⚠️ *In this dataset, `Gross Sales`, `Net Sales`, and `Total Sales` often appear identical due to inclusive pricing and zero taxes.*

</details>

## 🔍 Key Insights

✅ **Top 5 Selling Products**  
✅ **Region-wise Performance Heatmap**  
✅ **Customer Retention Analysis**  
✅ **Revenue Trends (Monthly)**  
✅ **High-value customer segmentation**

---

## 📊 Visuals

| Sales by Region | Monthly Revenue Trends |
|-----------------|------------------------|
| ![Region Heatmap](outputs/region_heatmap.png) | ![Monthly Trend](outputs/monthly_trend.png) |

---

## ⚙️ Tools Used

- **Python** (Pandas, NumPy, Matplotlib, Seaborn)
- **Power BI** for dashboard visualizations
- **Jupyter Notebook** for EDA
- **Streamlit** for web dashboard

---

## 🚀 How to Run

```bash
# Clone the repo
git clone https://github.com/yourusername/babyshop-sales-analysis.git
cd babyshop-sales-analysis

# Install dependencies
pip install -r requirements.txt

# Launch Streamlit app
streamlit run streamlit_app/app.py
