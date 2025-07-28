# task3_rfm
📊 Customer Segmentation using RFM Analysis – Step by Step
1. Dataset Selection
I used the Online Retail Dataset from UCI Machine Learning Repository. This dataset contains transactional data from an online store, including InvoiceNo, CustomerID, Quantity, UnitPrice, and InvoiceDate.

2. Data Cleaning

Removed missing CustomerID values

Excluded canceled orders (those starting with 'C')

Created a new column TotalPrice = Quantity × UnitPrice

3. Snapshot Date

Selected a fixed reference date (one day after the last invoice date) to calculate Recency.

4. RFM Metrics Calculation
Grouped data by each CustomerID and calculated:

Recency: How recently the customer purchased

Frequency: How many orders they placed

Monetary: Total money spent

5. RFM Scoring

Assigned scores (1 to 4) to Recency, Frequency, and Monetary using quantiles

Combined scores to create customer segments

6. Customer Segmentation
Based on RFM scores, customers were grouped into segments such as:

Champions

Loyal Customers

At Risk

Need Attention

Potential Loyalists

7. Visualizations
Used Seaborn and Matplotlib to create:

Bar plots of RFM segments

Heatmaps of RFM scores

Count plots to show customer distribution across segments

8. Marketing Suggestions
For each group, I suggested simple marketing strategies like:

Discounts for Loyal Customers

Re-engagement emails for Inactive or At-Risk customers

Special rewards for Champions
