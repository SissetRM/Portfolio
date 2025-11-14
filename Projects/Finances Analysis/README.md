# Financial Spend Analysis – Visa & Amex (2023–2024)

This project analyses a year of Visa and Amex transaction data to uncover spending trends, identify anomalies, and create a clean, well-structured dataset suitable for dashboards and reporting.
It demonstrates practical data cleaning, transformation, exploratory analysis, and dashboard-building skills using Excel, Python, SQL, and Tableau.

## Project Overview

Financial transaction data is notoriously messy: duplicated entries, inconsistent formats, translation issues, and fragmented monthly CSVs.
My goal in this project was to:

Merge 12+ monthly statements into a single unified dataset.

Translate Japanese transaction fields into English using a dynamic mapping table.

Categorise and structure transactions for analysis.

Identify monthly and category-level spending trends.

Build an interactive dashboard to assist with budgeting and insight generation.

This is a full end-to-end data pipeline project with real-world constraints.

## Key Objectives

Consolidate Visa and Amex monthly CSV files into a single dataset.

Translate non-English fields using an automated mapping approach.

Perform data cleaning (duplicates, invalid values, normalisation).

Engineer analytical fields such as category, subcategory, month, and vendor.

Produce exploratory visualisations to detect spending patterns.

Build an interactive dashboard in Tableau/Excel for final presentation.

## Data Sources

Visa credit card CSVs (monthly, Japanese format)

Amex credit card CSVs (monthly)

Translation mapping table for JP → EN column names

Manually corrected classifications for ambiguous transaction descriptions

Total raw files processed: 10+
Final clean dataset: ~500 rows

##Tools Used

###Software

Excel (PowerQuery + advanced cleaning functions)

Tableau (dashboard creation)

GitHub (version control + portfolio organisation)

## Data Cleaning & Transformation Process
### Consolidation

Loaded monthly Visa/Amex CSVs into PowerQuery.

Normalised schema across different providers.

Created a dynamic pipeline so new monthly data requires zero manual rework.

### Translation

Used a lookup table to automatically convert Japanese column headers into English.
Example mapping:

Japanese	English
利用日	Transaction Date
金額	Amount
店名	Merchant

5.3 Cleaning Steps

Removed duplicates.

Standardised date formats across providers.

Fixed category mismatches using custom rules.

Normalised vendor names for better grouping.

### Feature Engineering

Added:

Month

Year

Category

Card Provider

Transaction Type

Spend Buckets

## Exploratory Analysis (EDA)

Key insights from the clean dataset:

### Monthly Trends

Average monthly spend

Highest spend month

Lowest spend month

### Category Breakdown

Food & Drink

Subscriptions

Travel

Health/Pharmacy

### Anomalies

Spikes in income where loans were taken out

### Provider Comparison

Visa represented majority of total spend.

Amex had fewer transactions but higher average per-transaction cost.

## Dashboard

A multi-page Tableau dashboard was created including:

Monthly Spend Overview

Category Trends

Top Vendors

Provider Comparison (Visa vs Amex)

Transaction Heatmap

Dashboard supports:

Filtering by date range

Comparison across categories

Merchant-specific analysis

Screenshots and dashboard links go here if available.

## Key Takeaways

This project demonstrates:

Ability to clean multilingual financial datasets.

Experience handling messy, real-world CSVs.

Strong understanding of classification, normalisation, and dataset consolidation.

Practical storytelling through visualisation.

Use of multiple analytical tools in a coherent workflow.

It’s a realistic example of the type of work involved in financial analytics, budgeting tools, fintech data pipelines, and customer behaviour analysis.

## Folder Structure
project-financial-analysis/
     README.md
     data_raw
     data_clean/
     images/

## Future Improvements

Add predictive modelling.
