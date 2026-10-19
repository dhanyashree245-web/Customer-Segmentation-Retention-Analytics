# Customer Segmentation & Retention Analytics

## Project Overview
This project uses Power BI to analyze customer purchasing behavior, customer segments, retention status, and transaction activity. The goal is to help businesses understand their customers and identify opportunities to improve retention.

## Business Objectives
- Segment customers by spending behavior.
- Analyze retained, at-risk, and churned customers.
- Track monthly active customer trends.
- Analyze revenue contribution by customer segment.
- Explore customer cohorts by joining month.
- Examine customer support ticket patterns.

## Tools & Technologies
- Microsoft Power BI Desktop
- Power Query
- DAX
- CSV datasets
- GitHub

## Dataset
The project includes three tables:
- **Customers:** Customer demographics, region, join date, and customer attributes.
- **Transactions:** Purchase dates, products, quantities, prices, and sales amounts.
- **SupportTickets:** Customer issues, ticket dates, resolution times, and ticket status.

The datasets are synthetic and intended for learning and portfolio demonstration.

## Dashboard Features
- Total Sales
- Total Customers
- Retention Rate
- Average Customer Lifetime Value proxy
- Revenue contribution by customer segment
- Monthly active customer trend
- New versus returning customer distribution
- Customer cohort retention heatmap
- Region, age group, and gender filters

## Data Model
The model uses relationships between Customers and Transactions, Customers and SupportTickets, and a DateTable connected to Transactions.

## Important Notes
Customer retention categories and cohort metrics are based on the available sample data and project definitions. The Average CLV metric is a historical spending proxy, not a predictive lifetime value model. Cohort retention calculations should be validated before using them for business decisions.

## Project Structure
- `data/` — CSV datasets
- `screenshots/` — Dashboard screenshots
- `README.md` — Project documentation
- `Customer_Segmentation_Retention_Analytics.pbix` — Power BI report

## Learning Outcomes
- Data modeling and relationships
- Power Query data preparation
- DAX measures and calculated columns
- Customer segmentation and retention analysis
- Dashboard design and business reporting

## Disclaimer
This is an educational portfolio project using synthetic data. The findings do not represent a real company's customers or business performance.
