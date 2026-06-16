# Chart Selection Justification

## Overview

Each visualization in the executive dashboard was selected based on the business question being addressed. The chosen chart types maximize clarity, support comparison, and help leadership make informed decisions.

---

# 1. Sales Trend View

## Business Question

How are sales changing over time?

## Chart Type

Line Chart

## Why This Chart Is Appropriate

Line charts are the most effective way to display trends across time periods. They clearly show increases, decreases, and seasonal patterns in sales performance.

## Fields Used

* X-Axis: Order Date (Month/Quarter)
* Y-Axis: Sales
* Color: Year (optional)
* Filter: Region, Category, Customer Segment

## Design Principle Applied

Trend data is displayed using a continuous visual form that highlights changes over time.

## Mistake Avoided

Avoided using bar charts for long time-series analysis because they make trend identification more difficult.

---

# 2. Regional Performance View

## Business Question

Which regions perform best in terms of sales and profit?

## Chart Type

Horizontal Bar Chart

## Why This Chart Is Appropriate

Bar charts allow easy comparison of performance across multiple regions and support ranking from highest to lowest performers.

## Fields Used

* Dimension: Region
* Measure: Sales
* Color: Profit
* Label: Sales Value
* Filter: Date, Customer Segment

## Design Principle Applied

Categories are sorted by performance to support rapid comparison.

## Mistake Avoided

Avoided pie charts because they become difficult to interpret when comparing multiple regions.

---

# 3. Category Profitability View

## Business Question

Which categories and sub-categories generate the highest profit?

## Chart Type

Bar Chart

## Why This Chart Is Appropriate

Bar charts make it easy to compare profitability across categories and identify top and bottom performers.

## Fields Used

* Dimension: Category/Sub-Category
* Measure: Profit
* Color: Profit Margin
* Label: Profit Value
* Filter: Region, Segment

## Design Principle Applied

Color is used to emphasize profitability differences while maintaining readability.

## Mistake Avoided

Avoided treemaps as the primary chart because exact value comparisons are harder than with bars.

---

# 4. Customer Segment View

## Business Question

Which customer segments contribute the most sales and profit?

## Chart Type

Side-by-Side Bar Chart

## Why This Chart Is Appropriate

Allows direct comparison of sales and profit across customer segments.

## Fields Used

* Dimension: Customer Segment
* Measure: Sales and Profit
* Color: Measure Names
* Label: Sales/Profit Values
* Filter: Region, Date

## Design Principle Applied

Uses consistent scaling to enable fair comparisons.

## Mistake Avoided

Avoided stacked charts that could obscure differences between measures.

---

# 5. Shipping Performance View

## Business Question

Which shipping modes are associated with longer delivery times?

## Chart Type

Bar Chart

## Why This Chart Is Appropriate

Bar charts clearly compare average delivery times across shipping methods.

## Fields Used

* Dimension: Ship Mode
* Measure: Average Delivery Days
* Color: Shipping Delay Bucket
* Label: Average Days
* Filter: Region, Date

## Design Principle Applied

Simplifies operational comparisons by displaying averages clearly.

## Mistake Avoided

Avoided excessive color usage that could distract from the delivery comparison.

---

# 6. Discount vs Profit View

## Business Question

How does discounting affect profitability?

## Chart Type

Scatter Plot

## Why This Chart Is Appropriate

Scatter plots are the best choice for examining relationships between two numerical variables.

## Fields Used

* X-Axis: Discount
* Y-Axis: Profit
* Color: Category
* Detail: Order ID
* Filter: Region, Segment

## Design Principle Applied

Individual observations are displayed to reveal patterns, clusters, and outliers.

## Mistake Avoided

Avoided line charts because discounts are not a time-based variable.

---

# 7. Return Analysis View

## Business Question

Which categories, regions, or customer segments experience the highest return rates?

## Chart Type

Bar Chart

## Why This Chart Is Appropriate

Bar charts allow straightforward comparison of return rates across business groups.

## Fields Used

* Dimension: Category / Region / Segment
* Measure: Return Rate
* Color: Return Rate
* Label: Percentage
* Filter: Date, Region

## Design Principle Applied

Color intensity highlights areas with elevated return activity.

## Mistake Avoided

Avoided tables as the primary visualization because patterns are more difficult to identify visually.

---

# Dashboard-Wide Design Principles

The following principles were applied across all visualizations:

* Consistent color usage
* Clear titles and labels
* Logical layout
* Minimal clutter
* Appropriate chart selection
* Readable formatting
* Interactive filtering

---

# Dashboard-Wide Mistakes Avoided

The dashboard intentionally avoids:

* 3D charts
* Decorative visualizations
* Overcrowded layouts
* Excessive colors
* Misleading scales
* Unsorted comparisons
* Pie charts with many categories

These decisions improve clarity and support executive decision-making.

---

# Conclusion

Each chart was selected to answer a specific business question using the most appropriate visualization type. The dashboard emphasizes clarity, comparability, and business usability while avoiding common visualization mistakes that can distort interpretation.
