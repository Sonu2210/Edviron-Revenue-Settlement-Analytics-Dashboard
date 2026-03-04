# Edviron-Revenue-Settlement-Analytics-Dashboard
Overview

This project analyzes transaction data from Edviron’s payment platform to understand revenue generation, transaction behavior, and settlement exposure. The goal of the project is to transform raw transactional data into meaningful financial insights using data modeling and interactive visualization.

The dataset includes information about payment transactions, pricing layers, ERP partners, payment gateways, and settlement details. Using this data, a structured analytical model was built to compute revenue metrics and visualize key business insights through an interactive dashboard.

This project demonstrates skills in data cleaning, financial modeling, analytics, and dashboard development using Excel and Power BI.

Business Context

Each transaction processed through Edviron’s platform involves three pricing layers:

Pricing Layer	Description
Edviron Buying Price	Cost at which Edviron purchases payment processing
Partner Pricing	Price at which Edviron sells processing to ERP partners
Merchant Pricing	Price charged by ERP partners to schools

These pricing layers determine how revenue is distributed between Edviron and ERP partners.

Revenue Calculation Logic

The following financial metrics were derived from the pricing structure.

ERP Revenue

ERP Revenue = Merchant Pricing − Partner Pricing

Edviron Net Revenue

Edviron Net Revenue = Partner Pricing − Edviron Buying

Edviron Gross Revenue

Edviron Gross Revenue = ERP Revenue + Edviron Net Revenue

These calculations help measure the revenue distribution across the payment ecosystem.

Project Workflow

The project was implemented in several stages.

1. Data Cleaning

Raw transactional data was cleaned and standardized by:

Ensuring consistent data types for numeric fields

Normalizing pricing values

Handling missing or inconsistent values

Structuring the dataset for analytical modeling

2. Data Modeling

Additional columns were created to compute financial metrics such as:

ERP Revenue

Edviron Net Revenue

Edviron Gross Revenue

Gateway Fees

Settlement amounts

Revenue take rates

These calculations enabled deeper financial analysis of the platform.

3. Dashboard Development

An interactive analytics dashboard was created to visualize the most important business insights.

The dashboard focuses on:

Platform transaction performance

Revenue generation and distribution

Payment gateway usage

Payment method trends

ERP partner performance

Settlement exposure

Dashboard Metrics

The dashboard displays the following key performance indicators:

Total Transactions

Total GMV (Gross Merchandise Value)

ERP Revenue

Edviron Net Revenue

Edviron Gross Revenue

Pending Exposure

Unique Users

These metrics provide a quick snapshot of platform activity and financial performance.

Key Visualizations

The dashboard includes several visual components to highlight business insights.

Revenue Split

Shows how revenue is distributed between ERP partners and Edviron.

Revenue Trend

Displays how revenue changes over time.

Gateway Contribution

Identifies which payment gateways process the highest transaction volume.

Payment Method Distribution

Shows the usage of different payment methods such as UPI, card, and net banking.

ERP Partner Performance

Highlights which partners contribute the most revenue.

Tools & Technologies

This project was built using the following tools:

Microsoft Excel – Data cleaning and financial modeling

Power BI – Interactive dashboard and data visualization

DAX – Creating measures for dashboard metrics

GitHub – Project documentation and version control

Project Structure
project/
│
├── data/
│   └── edviron_transactions.xlsx
│
├── excel_model/
│   └── Revenue_Analytics_Model.xlsm
│
├── dashboard/
│   └── Edviron_Revenue_Dashboard.pbix
│
├── docs/
│   └── Revenue_Settlement_Explanation.pdf
│
└── README.md
Key Insights

The analysis provides several important insights about the payment ecosystem:

Revenue is generated through a layered pricing structure involving ERP partners and Edviron.

Payment gateways contribute differently to transaction volumes.

Payment method usage highlights customer behavior patterns.

Pending transactions represent potential settlement exposure and operational risk.

These insights help monitor platform performance and identify areas for operational improvement.

Conclusion

This project demonstrates how transactional payment data can be transformed into actionable financial insights through data modeling and interactive analytics dashboards.

By combining structured data preparation with business-focused visualizations, the dashboard provides a comprehensive view of revenue performance, partner contributions, and operational risks within Edviron’s payment ecosystem.
