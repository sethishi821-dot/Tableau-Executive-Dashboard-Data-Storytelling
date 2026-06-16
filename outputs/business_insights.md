# Calculated Fields Documentation

## Overview

Several calculated fields were created in Tableau to support business analysis, KPI tracking, and dashboard development.

---

# 1. Profit Margin

## Formula

```tableau
SUM([profit]) / SUM([sales])
```

## Purpose

Profit Margin measures the percentage of sales revenue retained as profit after costs.

## Business Value

* Identifies profitable products, categories, and regions.
* Helps management evaluate operational efficiency.
* Supports pricing and discount decisions.

---

# 2. Cost

## Formula

```tableau
[sales] - [profit]
```

## Purpose

Cost estimates the amount spent to generate sales revenue.

## Business Value

* Helps evaluate profitability.
* Supports cost-control initiatives.
* Allows comparison between revenue and expenses.

---

# 3. Average Order Value (AOV)

## Formula

```tableau
SUM([sales]) / COUNTD([order_id])
```

## Purpose

Average Order Value measures the average revenue generated per order.

## Business Value

* Indicates customer purchasing behavior.
* Helps assess effectiveness of upselling and cross-selling strategies.
* Useful for monitoring sales performance over time.

---

# 4. Return Rate

## Formula

```tableau
SUM([return_flag]) / COUNT([order_id])
```

## Purpose

Return Rate measures the proportion of orders that were returned.

## Business Value

* Highlights product quality issues.
* Helps identify operational problems.
* Supports customer satisfaction monitoring.

## Interpretation

* Higher values indicate more product returns.
* Lower values indicate stronger customer retention and product acceptance.

---

# 5. Shipping Delay Bucket

## Formula

```tableau
IF [delivery_days] <= 2 THEN "Fast Delivery"
ELSEIF [delivery_days] <= 5 THEN "Standard Delivery"
ELSEIF [delivery_days] <= 8 THEN "Delayed Delivery"
ELSE "Severely Delayed"
END
```

## Purpose

Groups delivery performance into meaningful categories.

## Business Value

* Simplifies logistics analysis.
* Identifies operational bottlenecks.
* Supports service-level monitoring.

---

# Additional Calculated Field 6: Profit Category

## Formula

```tableau
IF [profit] > 0 THEN "Profitable"
ELSE "Loss Making"
END
```

## Purpose

Classifies transactions based on profitability.

## Business Value

* Quickly identifies loss-making sales.
* Supports profitability analysis by product and region.

---

# Additional Calculated Field 7: Sales Category

## Formula

```tableau
IF [sales] >= 1000 THEN "High Sales"
ELSEIF [sales] >= 500 THEN "Medium Sales"
ELSE "Low Sales"
END
```

## Purpose

Groups transactions into sales-performance categories.

## Business Value

* Helps identify high-value orders.
* Simplifies dashboard filtering and reporting.

---

# Summary of Calculated Fields

| Calculated Field      | Purpose                                         |
| --------------------- | ----------------------------------------------- |
| Profit Margin         | Measure profitability percentage                |
| Cost                  | Estimate business cost                          |
| Average Order Value   | Measure average revenue per order               |
| Return Rate           | Measure returned-order percentage               |
| Shipping Delay Bucket | Categorize delivery performance                 |
| Profit Category       | Classify profitable vs loss-making transactions |
| Sales Category        | Classify sales performance levels               |

These calculated fields provide additional business insights and support the development of interactive Tableau dashboards for sales, profitability, customer behavior, and operational performance analysis.
