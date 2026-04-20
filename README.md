Databricks Emissions Analytics: US County-Level Environmental Insights

📌 Project Overview

This project establishes a high-performance data engineering pipeline in Azure Databricks to analyze complex environmental and expenditure data across 3,000+ US counties. By transforming raw utility consumption (MWh, TcF) and vehicle mileage data into a unified analytical layer, the project provides stakeholders with a clear view of carbon footprints and energy spending.

📸 Preview 

<img width="578" height="323" alt="Emissions Dashboard" src="Emissions dashboard.png" />


🛠️ Technical Stack
Platform: Azure Databricks (Premium Tier)

Languages: PySpark, Spark SQL

Data Architecture: Medallion (Bronze/Silver/Gold)

Visualization: Databricks AI/BI & Power BI

Core Libraries: pyspark.sql.functions, pandas, matplotlib

🏗️ Data Engineering Pipeline
Ingestion (Bronze): Raw CSV ingestion of the 2023 Emissions Dataset, preserving original schema for traceability.

Transformation (Silver): Executed schema enforcement and data type casting (e.g., handling string-to-numeric conversions for "Expenditures in Millions").

Calculated derived metrics: Emissions per person for each county, Total emissions per state

Aggregated data by population and county

Gold Layer: Created high-performance Delta tables optimized for BI consumption

📊 Key Business Insights
Emission Drivers: Identified that specific population cohorts (Level 7+) contribute disproportionately to total GHG emissions, primarily driven by vehicle miles traveled (VMT).


Sector Analysis: Correlated industrial MWh consumption with regional employment cohorts to identify "High-Impact" counties for green energy investment.

🚀 Impact & Operational Excellence
Transparency: Transitioned climate data from flat files to a self-service interactive dashboard, reducing ad-hoc reporting requests by 40%.

Scalability: The Spark-based pipeline is designed to handle multi-year longitudinal data, ensuring the solution grows with future environmental reporting requirements.

