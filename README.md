
# Procurement-Insight-Analysis

Procurement Analysis Project, used to teach **Excel & Power BI** skills to a new data analyst.

# Project Overview

This project uses a **Procurement KPI dataset** sourced from Kaggle. The dataset contains purchase order (PO) details from suppliers and allows analysis of delivery timelines, order statuses, negotiated savings, compliance, and procurement performance.

# Objective

The objectives of this project are to:

1. Calculate the **duration between Order Date and Delivery Date**.
2. Analyze the **number of orders delivered, cancelled, or pending**.
3. Measure the **total negotiated savings** (Unit Price vs Negotiated Price).


# Data Understanding

The dataset consists of **777 rows and 11 columns**.

| Column                | Description                                                              |
| --------------------- | ------------------------------------------------------------------------ |
| **PO\_ID**            | Unique purchase order ID                                                 |
| **Supplier**          | Supplier/Company fulfilling the order                                    |
| **Order\_Date**       | Date when order was placed                                               |
| **Delivery\_Date**    | Date when order was delivered (if applicable)                            |
| **Item\_Category**    | Category of the purchased item (e.g., Office Supplies, Raw Materials)    |
| **Order\_Status**     | Status of the order (Delivered, Pending, Cancelled, Partially Delivered) |
| **Quantity**          | Number of units ordered                                                  |
| **Unit\_Price**       | Original price per unit                                                  |
| **Negotiated\_Price** | Final negotiated price per unit                                          |
| **Defective\_Units**  | Number of units received as defective                                    |
| **Compliance**        | Whether the order met compliance standards (Yes/No)                      |

**Missing Data:**

* Delivery Date → 87 missing values (likely pending or cancelled orders).
* Defective Units → 136 missing values (may indicate no defect report).


# Methodology

# Excel

* Data cleaning: removed duplicates, handled blanks, standardized formatting.
* Created calculated fields (e.g., delivery duration, amount saved).

# Power BI & Power Query

* Created new columns for delivery duration and negotiated savings.
* Built interactive dashboards for visualization.
* Applied DAX for KPIs (e.g., average delivery period, amount saved, total orders delivered).


# The Dashboard
<img width="1278" height="714" alt="Screenshot 2025-09-17 191006" src="https://github.com/user-attachments/assets/165e2a2f-8842-492d-bc8d-db42494066ac" />



# The Insights

* **Average Delivery Period:** 53.68 days.
* **Total Orders Delivered:** 560 (out of 777 orders).
* **Amount Saved:** \~4 million through negotiated prices.

   **Delivery Timelines:**

  * 691 orders delivered **in time**.
  * 76 orders had **unknown delivery periods** (likely pending/cancelled).
  * 8 orders were **above/extra time**.

   **Amount Saved by Categories:**

  * MRO → 902K
  * Office Supplies → 844K
  * Electronics → 743K
  * Packaging → 733K
  * Raw Materials → 709K

 **Order Status Breakdown:**

  * Delivered → 560
  * Pending → 81
  * Partially Delivered → 73
  * Cancelled → 63


# Recommendations

1. Focus on categories like **MRO and Office Supplies**, which generate the highest savings.
2. Investigate suppliers associated with **delayed or unknown delivery timelines**.
3. Develop stricter follow-up processes for **pending and partially delivered orders**.
4. Reduce defective unit rates through **supplier performance reviews**.
5. Expand negotiations in **low-saving categories** like Raw Materials to improve cost efficiency.


# Conclusion

This procurement analysis shows how **Excel & Power BI** can be applied to monitor supplier performance, track delivery efficiency, and optimize cost savings. With an average delivery period of **54 days** and savings of **4 million**, organizations can leverage these insights to **improve compliance, negotiate smarter, and streamline procurement operations**.

