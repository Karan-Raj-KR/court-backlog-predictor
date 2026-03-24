# Court Backlog Intelligence Platform 🏛️

An AI & data platform built on Databricks to analyze India's 50M+ pending court cases.

## Problem
India has 50 million pending court cases. Citizens wait decades for justice.
Prayagraj alone has 130,344 cases pending over 10 years.

## Solution
A Databricks-native data product that identifies backlog hotspots, predicts 
clearance timelines, and simulates policy interventions.

## Tech Stack
- PySpark — data pipeline & transformation
- Delta Lake — storage with time-travel versioning
- Spark MLlib — backlog prediction model
- Databricks AI/BI Dashboard — visualization
- Genie — natural language querying
- MLflow — experiment tracking

## Key Insights
- Uttar Pradesh: 19.1M pending cases (highest in India)
- 142 districts have 10,000+ cases pending over 10 years
- Prayagraj: 130,344 decade-old cases
- Bihar: 22,420 cases pending over 30 years
- Simulation: 30% more judges cuts UP backlog from 19M → 13.4M

## Data Source
District and Taluka Court Cases — sourced from NJDG 
(National Judicial Data Grid, Supreme Court of India)
