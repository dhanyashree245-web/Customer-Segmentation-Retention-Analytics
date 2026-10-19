# Customer Segmentation & Retention Analytics — Sample Dataset

## Contents
- `Customers.csv`: one row per customer, including demographics and customer-level summary attributes.
- `Transactions.csv`: one row per purchase transaction, including quantity, unit price, sales amount, product category, and channel.
- `SupportTickets.csv`: optional simulated customer support tickets.

## Important data note
This is a **synthetic educational dataset** generated for a Power BI portfolio project. It does not represent real customers or a real company. Demographics, engagement scores, satisfaction scores, purchase records, and support tickets are simulated.

## Dataset size
- 300 customers
- 1328 transactions
- 117 support tickets

## Suggested Power BI relationships
- `Customers[Customer ID]` (one) → `Transactions[Customer ID]` (many)
- `Customers[Customer ID]` (one) → `SupportTickets[Customer ID]` (many)

Use single-direction filtering from Customers to the fact tables. Create a separate Date table for transaction-date analysis and relate it to `Transactions[Transaction Date]`.

## Definitions used in the sample
- `Purchase Frequency`: number of transactions for the customer.
- `Average Order Value`: customer total spend divided by number of transactions.
- `Retention Status`: based on days since last purchase as of 2025-12-31: Retained = 0–59 days, At Risk = 60–119 days, Churned = 120+ days.
- `Customer Segment`: based on sample total spend: High Value >= 12,000; Medium Value >= 6,000 and < 12,000; Low Value < 6,000.
- `Loyalty Tier`: Bronze < 6,000; Silver >= 6,000; Gold >= 12,000; Platinum >= 18,000.
- `Customer Type`: Returning if two or more transactions; otherwise New.

These thresholds are illustrative business rules, not universal industry standards. For a stronger analytical project, you can recreate selected classifications in Power BI using DAX and compare them with the supplied sample fields.

## Currency
Amounts are illustrative and expressed in Indian rupees (INR).
