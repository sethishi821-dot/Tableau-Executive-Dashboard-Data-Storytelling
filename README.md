# README

## Task 1: Connect and Inspect Data

### Dataset Overview

The dataset was loaded into Tableau from the Excel workbook:

`dashboard_sales_data.xlsx`

The workbook contains:

1. `dashboard_sales_data` – Main transactional dataset
2. `data_dictionary` – Field descriptions

The main dataset contains:

* 4,200 records
* 20 fields

---

## Field Classification

### Date Fields

| Field      | Data Type |
| ---------- | --------- |
| order_date | Date      |
| ship_date  | Date      |

These fields can be used for time-series analysis and trend reporting.

---

### Geographic Fields

| Field  | Data Type |
| ------ | --------- |
| region | String    |
| state  | String    |
| city   | String    |

These fields support geographic analysis and regional performance reporting.

---

### Categorical Fields (Dimensions)

| Field            |
| ---------------- |
| order_id         |
| customer_id      |
| customer_segment |
| category         |
| sub_category     |
| product_name     |
| ship_mode        |
| campaign_channel |

These fields are suitable for grouping, filtering, and segmentation analysis.

---

### Numerical Measures

| Field           | Data Type |
| --------------- | --------- |
| sales           | Decimal   |
| quantity        | Integer   |
| discount        | Decimal   |
| profit          | Decimal   |
| delivery_days   | Integer   |
| customer_rating | Decimal   |

These fields are suitable for aggregation and KPI calculations.

---

### Binary / Flag Fields

| Field       | Data Type     |
| ----------- | ------------- |
| return_flag | Integer (0/1) |

Interpretation:

* 0 = Order not returned
* 1 = Order returned

This field can be used for return-rate analysis.

---

## Assumptions

### Date Assumptions

* order_date represents the date the order was placed.
* ship_date represents the date the order was shipped.

### Geographic Assumptions

* Region, State, and City values are valid geographic classifications.
* Tableau geographic roles may be assigned to State and City if required.

### Return Flag Assumption

* return_flag is treated as a binary field.
* Value 1 indicates a returned order.
* Value 0 indicates a non-returned order.

### Customer Rating Assumption

* customer_rating is assumed to be measured on a consistent rating scale across all records.

### Sales and Profit Assumption

* sales represents total revenue for an order.
* profit represents profit earned from the order.

### Delivery Days Assumption

* delivery_days represents the number of days between order placement and shipment or delivery processing.

---

## Data Quality Notes

* Date fields were successfully recognized as date data types.
* Geographic fields were identified and can be assigned Tableau geographic roles.
* Numerical measures are available for KPI and dashboard calculations.
* The dataset structure is suitable for sales, profitability, customer, and operational performance analysis.
