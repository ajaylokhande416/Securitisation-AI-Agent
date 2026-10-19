# Securitisation AI Agent — Power BI Analytics Project

## Project Overview

The Securitisation AI Agent is a financial data analytics and reporting project developed using Microsoft Power BI. It analyzes loan portfolio performance, delinquency, credit losses, expected credit loss (ECL), vintage performance, and stress-testing scenarios through interactive dashboards.

The project demonstrates how data modeling, DAX measures, KPI monitoring, and interactive visualizations can support portfolio analysis and financial risk monitoring.

**Note:** This project is a Power BI analytics dashboard. It does not currently implement an autonomous AI agent or a machine-learning prediction model.

## Project Objectives

- Analyze loan portfolio balances and performance.
- Monitor gross losses, recoveries, and net losses.
- Evaluate delinquency using Days Past Due (DPD) buckets.
- Analyze vintage performance and cumulative losses.
- Monitor Expected Credit Loss (ECL) provisions.
- Explore hypothetical stress scenarios using What-If parameters.
- Present financial metrics through interactive dashboards.

## Technology Stack

- **Business Intelligence:** Microsoft Power BI
- **Data Transformation:** Power Query
- **Data Modeling and Calculations:** DAX
- **Data Sources:** Structured CSV datasets
- **Documentation:** Microsoft Word
- **Presentation:** Microsoft PowerPoint

## Dashboard Modules

### 1. Portfolio Overview
Provides a high-level view of the loan portfolio, including total loans, outstanding balances, original loan amounts, gross losses, recoveries, net losses, ECL provisions, and portfolio loss ratios.

### 2. Delinquency Analysis
Examines delinquent loans, delinquency rates, overdue amounts, average Days Past Due, and loan distribution across DPD buckets.

### 3. Portfolio Performance
Tracks monthly gross losses, recoveries, net losses, and portfolio performance indicators.

### 4. Vintage Analysis
Analyzes loan vintages using original pool balances, remaining pool balances, cumulative losses, and vintage-level loss rates.

### 5. ECL Analysis
Displays ECL provisions and compares them with gross losses and loan-level financial measures.

### 6. Waterfall and Tranche Allocation
Presents supporting cash-flow metrics, including collections, scheduled amortization, prepayments, recoveries, excess spread, and losses.

**Limitation:** Senior, mezzanine, and equity tranche allocation values are placeholders. Actual tranche allocation and waterfall calculations require validated tranche balances and applicable waterfall rules.

### 7. Stress Testing and What-If Analysis
Uses interactive parameters to examine hypothetical increases in gross losses and reductions in recoveries, and compares baseline results with stressed net losses.

## Key Analytical Metrics

- Total Loan Balance
- Total Original Loan Amount
- Total Gross Loss
- Total Recoveries
- Total Net Loss
- Total ECL Provision
- Loan Loss Rate
- Recovery Rate
- Net Loss Rate
- Delinquency Rate
- Remaining Pool Balance
- Stressed Gross Loss
- Stressed Recoveries
- Combined Stressed Net Loss

## Data Quality and Validation

The project includes data-quality observations and validation checks.

- Duplicate records were identified in the DPD snapshot dataset.
- The cumulative defaults count field contains zero values despite positive cumulative default balances.
- The monthly loss dataset contains a duplicate May reporting date and a potentially missing November reporting period.
- These source-data issues were documented rather than silently corrected.
- Stress-testing calculations were checked using example parameter values.

Results should be interpreted in light of these data-quality limitations.

## Repository Structure

```text
Securitisation-AI-Agent/
├── README.md
├── dashboard/
│   └── Securitisation_AI_Agent_Dashboard.pbix
├── documentation/
│   └── Securitisation_AI_Agent_Project_Documentation.docx
├── presentation/
│   └── Securitisation_AI_Agent_Project_Presentation_With_Dashboard_Screenshots.pptx
├── screenshots/
│   ├── portfolio-overview.png
│   ├── delinquency-analysis.png
│   ├── portfolio-performance.png
│   ├── vintage-analysis.png
│   ├── ecl-analysis.png
│   ├── waterfall-tranche-allocation.png
│   └── stress-testing.png
└── dax/
    └── [Exported DAX files, if available]
```

*Update the filenames and folders to match the files actually uploaded to this repository.*

## How to Use

1. Clone or download this repository.
2. Open the Power BI file in Microsoft Power BI Desktop.
3. Review the dashboard pages and interact with available slicers and What-If parameters.
4. Refer to the documentation and presentation for project details and known limitations.

The Power BI Desktop application is required to interact with the `.pbix` dashboard.

## Limitations and Future Improvements

- Resolve and validate source-data quality issues.
- Validate delinquency calculations against the latest reporting snapshots.
- Add verified tranche balances and waterfall rules.
- Implement appropriate overcollateralization and trigger calculations once required data and thresholds are available.
- Improve automated data validation and refresh processes.
- Explore additional predictive analytics when suitable data and a validated modeling approach are available.

## Author

**Ajay Lokhande**

Electronics and Telecommunication Engineering Graduate | Aspiring Data Analyst

Skills demonstrated: Power BI, DAX, Power Query, data modeling, KPI analysis, financial reporting, and data visualization.
