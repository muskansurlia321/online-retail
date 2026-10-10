# Retail Sales and Product Demand Analysis

## Project Overview
This project analyzes retail transaction data using Python to identify sales trends, top-performing products, category-wise revenue, and city-level performance. The goal is to generate useful business insights that can support better inventory planning and sales decisions.

## Dataset Information
- **Original records:** 10,000
- **Records after cleaning:** 9,568
- **Columns:** 14
- **Date range:** January 2023 – August 2024
- **Unique cities:** 23
- **Product categories:** Electronics, Clothing, Home, Sports, Beauty

### Key Columns
| Column | Description |
|---|---|
| `order_id` | Order identifier |
| `order_date` | Date of purchase |
| `customer_id` | Customer identifier |
| `product_id` | Product identifier |
| `product_name` | Name of the product |
| `category` | Product category |
| `quantity` | Units purchased |
| `price` | Recorded product price |
| `amount` | Recorded transaction amount |
| `payment_method` | Payment method |
| `city` | City associated with the transaction |
| `state` | State or region |
| `coupon_used` | Coupon usage information |
| `order_status` | Delivered, Shipped, or Cancelled |

## Tools and Technologies
- Python
- Pandas and NumPy
- Matplotlib
- Seaborn
- Google Colab / Jupyter Notebook

## Data Cleaning
- Standardized column names and text values.
- Converted dates and numeric columns to appropriate data types.
- Removed records with missing values in essential fields.
- Filtered out non-positive quantities and negative prices or amounts.
- Checked for missing values and duplicate records.

## Analysis Performed
1. **City-wise Revenue Analysis:** Identifies cities with the highest recorded revenue.
2. **Product Demand Analysis:** Ranks products by quantity sold.
3. **Category Performance:** Compares revenue across product categories.
4. **Monthly Sales Trends:** Examines changes in recorded sales over time.
5. **Coupon Analysis:** Compares transaction amounts by coupon usage.
6. **City–Category Analysis:** Uses a heatmap to compare category revenue across cities.

## Visualizations
The project includes:
- Top 10 cities by revenue
- Top 10 products by quantity sold
- Revenue by product category
- Monthly revenue trend
- Average transaction amount by coupon usage
- Revenue by city and product category heatmap

## Key Findings
- Electronics has the highest recorded category revenue in the analyzed dataset.
- Bluetooth Headphones is the top product by recorded quantity sold.
- Surat has the highest recorded city revenue in the current city summary.
- Transactions marked as coupon-used have a slightly higher average recorded amount than those without coupons.

These findings are descriptive and do not establish causation.

## How to Run
1. Clone or download this repository.
2. Open the notebook in Google Colab or Jupyter Notebook.
3. Upload the dataset CSV file.
4. Run the notebook cells in order.
5. Review the tables, charts, and business insights.

## Limitations
- The dataset covers January 2023 to August 2024, not the full 2020–2025 period.
- The city list includes international locations, so the current analysis is not India-only.
- Revenue figures use the dataset's `amount` field; the currency and original data provenance have not been independently verified.
- Unless filtered by order status, recorded amounts may include shipped and cancelled orders.
- The analysis is exploratory and does not use machine learning or predictive modeling.

## Future Improvements
- Restrict analysis to verified Indian cities.
- Separate delivered, shipped, and cancelled orders.
- Add profit and discount analysis if the required data becomes available.
- Build an interactive sales dashboard.


## License
Specify a license if you choose to distribute this project publicly.
