# Sony Headset Sales Performance Dataset

## Project Overview
This dataset provides a detailed log of sales transactions for Sony's premium headset lineup from **January 2023 through September 2025**. It is designed to support retail analytics, financial forecasting, and marketing ROI (Return on Investment) modeling.

## File Details
- **Filename:** `sony_headset_sales_1000_rows.csv`
- **Total Records:** 1,045 (including ~1,000 core transactions)
- **Primary Keys:** `Order_ID`, `Day_Index`

## Data Dictionary

| Column Name | Description | Data Type |
| :--- | :--- | :--- |
| **Date** | Date of transaction (YYYY-MM-DD). | Date |
| **Order_ID** | Unique alphanumeric identifier for each order. | String |
| **Region** | Market location: North, South, East, West. | Categorical |
| **Sales_Channel** | Distribution method: Online, Retail Store, Distributor. | Categorical |
| **Product_Model** | The specific Sony model (XM4, XM5, XB910N, CH720N). | Categorical |
| **Unit_Price_USD** | Price per unit (Ranges from $100 to $319). | Float |
| **Units_Sold** | Quantity sold per transaction. | Integer |
| **Revenue_USD** | Total sales value ($). | Float |
| **Marketing_Spend_USD** | Advertising/Marketing costs attributed to the day. | Float |
| **Customer_Rating** | User satisfaction score (3.5 to 5.0). | Float |
| **Day_Index** | Sequential day counter for time-series analysis. | Integer |

## Key Insights & Statistics
- **Top Models:** Includes high-end noise-canceling series (WH-1000XM5/XM4) and budget-friendly options (CH720N).
- **Average Revenue:** ~$10,734 per transaction.
- **Average Rating:** 4.27 / 5.0.
- **Geographic Coverage:** Balanced distribution across 4 major regions.

## Analysis Suggestions
1. **Marketing Efficiency:** Calculate the correlation between `Marketing_Spend_USD` and `Revenue_USD`.
2. **Seasonal Trends:** Use the `Date` column to identify peak sales months or holiday surges.
3. **Price Sensitivity:** Analyze how different `Unit_Price_USD` points affect the total `Units_Sold`.
4. **Channel Profitability:** Compare the average order value (AOV) between `Online` and `Retail Store`.

## Data Cleaning Notes
* **Missing Values:** There are a few rows at the end of the file containing projected data without `Order_IDs`. For historical analysis, filter where `Order_ID` is not null.
* **Normalization:** Ensure `Date` is converted to a datetime object before performing time-series calculations.

---
*Generated for Sony Dataset Dashboard Analysis.*
