# Understanding Uneven Food Price Increases in Nigeria (2007–2026)

## Project Overview

Food prices affect household budgets, business costs and market decisions. However, individual commodities do not always experience the same price movements, and national averages can hide differences between markets and locations.

This project analyses historical food-price records from selected Nigerian markets to examine long-term price movements, commodity-level differences, food-category growth and regional price disparities.

The analysis covers **74 markets, 18 states and eight food commodities**, from **January 2007 to August 2026**. It uses Microsoft Power BI to transform historical price records into an interactive dashboard for exploring trends and identifying patterns relevant to market monitoring and decision-making.

## Business Questions

The analysis investigates the following questions:

1. How have the recorded prices of selected food commodities changed between 2007 and 2026?
2. Which commodities have the highest average recorded prices?
3. How do price movements for staple foods compare with those of protein sources?
4. What differences appear between Northern Nigeria and other states represented in the dataset?
5. Which commodities and periods may warrant closer market monitoring?

## Dataset Scope

The project examines eight commodities grouped into two categories:

| Category | Commodities |
|---|---|
| Staples | Beans, Garri, Rice, Yam |
| Proteins | Beef, Eggs, Fish, Milk |

**Coverage:** 74 markets, 18 states  
**Period:** January 2007 – August 2026  
**Source:** World Bank Real-Time Food Prices (RTFP) Monitor – Nigeria

The regional comparison groups Northern Nigeria separately from other states represented in the dataset. The results should therefore be interpreted within the available geographical coverage.

## Tools and Technologies

- **Microsoft Power BI:** Data modelling, DAX calculations and interactive dashboard development.
- **Power Query:** Data cleaning, transformation and preparation.
- **DAX:** Measures for average recorded prices, percentage changes and category comparisons.

## Data Preparation and Methodology

The original dataset was inspected and prepared for analysis. Relevant commodity fields were selected and transformed from a wide structure into a normalized format, with separate fields for food commodity and recorded price.

The preparation and modelling process included:

1. Selecting the eight commodities included in the analysis.
2. Restructuring commodity columns using Power Query unpivoting.
3. Standardizing commodity names and preparing date fields.
4. Classifying commodities as staples or proteins.
5. Grouping geographical records into Northern Nigeria and other represented states.
6. Creating a dedicated Date Table for time-based analysis.
7. Establishing relationships between the date dimension and the food-price data.
8. Creating DAX measures to support price and category comparisons.

## Dashboard Analysis

The interactive dashboard is organized around four areas:

### 1. Historical Price Trends

Explores how recorded prices have changed over time and highlights periods of notable movement.

### 2. Commodity-Level Comparison

Compares average recorded prices across the eight selected commodities to identify which foods have higher average prices within the selected filters.

### 3. Staples Versus Proteins

Compares the price movements of staple foods and protein sources. The normalized price index uses 2007 as its baseline, while the separate category growth KPIs compare 2020 with 2026. These measures answer different questions and should not be treated as interchangeable.

### 4. Regional Price Comparison

Examines differences between Northern Nigeria and other states represented in the dataset.

## Preliminary Dashboard Observations

The dashboard currently displays the following figures under its selected filters:

| Indicator | Displayed value |
|---|---:|
| Average recorded price | ₦991 |
| Food price change | 1,553% |
| Protein price growth KPI | 1.92K |
| Staples price growth KPI | 1.48K |
| Northern average price | ₦995.52 |
| Other states average price | ₦963.93 |

The displayed regional averages indicate a higher average recorded price for Northern Nigeria under the current dashboard filters. The category growth figures and normalized index are still subject to DAX validation; they should not be presented as final comparative conclusions until the measures have been checked.

## Potential Applications and Recommendations

The analysis can help stakeholders:

- Strengthen commodity-level food-price monitoring across markets.
- Use regional price information to guide further investigation and distribution planning.
- Incorporate historical price movements into procurement and inventory decisions.
- Monitor staple and protein categories separately.
- Combine price records with production, transportation, supply and demand data to investigate possible drivers of price changes.

These are potential applications of the analysis, not claims that the dashboard independently proves the causes of price movements.

## Limitations

- The analysis covers eight selected commodities, not every food item sold in Nigeria.
- Geographical findings are limited to the markets and states represented in the dataset.
- Recorded prices alone do not measure household affordability or purchasing power.
- The analysis identifies patterns and associations; it does not establish the causes of price changes.
- Category growth and normalized-index calculations require validation before final comparative claims are made.
- Differences in market coverage, reporting frequency and available observations may affect comparisons.

## Repository Contents

```text
nigeria-food-price-analysis/
│
├── README.md
├── dashboard/
│   └── food_price_analysis.pbix
├── images/
│   ├── dashboard_overview.png
│   ├── price_trends.png
│   └── regional_comparison.png
└── documentation/
    ├── methodology.md
    ├── key_findings.md
    └── recommendations.md
```

*Update this structure to match the files actually included in the repository.*

## How to Explore the Project

1. Review the dashboard screenshots in the `images` folder.
2. Read the supporting methodology and findings documents.
3. Download the `.pbix` file from the `dashboard` folder.
4. Open the report in Microsoft Power BI Desktop to explore its filters and visualizations.

## Project Outcome

This project demonstrates how historical food-price records can be cleaned, modelled and analysed to make long-term trends, commodity-level differences and regional price patterns easier to explore.

**The objective is to move beyond presenting numbers and use data to support informed questions and decisions.**
