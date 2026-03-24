# Court Backlog Intelligence Platform 🏛️

An AI & data platform built on Databricks to analyze India's 50M+ pending court cases.

## Problem

India has 50 million pending court cases. Citizens wait decades for justice. Prayagraj alone has 130,344 cases pending over 10 years.

## Solution

A Databricks-native data product that identifies backlog hotspots, predicts clearance timelines, and simulates policy interventions.

## How to Run

1. Upload the dataset CSV files to a Databricks Volume at `/Volumes/workspace/default/court_data/`
2. Open the `court_pipeline.ipynb` notebook in your Databricks workspace
3. Run all cells top to bottom
4. Open AI/BI Dashboard to view the 3 charts
5. Open Genie and connect it to the `court_cases_delta` table

## Demo Steps

**Dashboard:** Open the AI/BI Dashboard — view top 10 states bar chart, year trend line chart, criminal vs civil donut chart.

**Genie queries to run:**
1. "Which state has the most pending cases?" → Uttar Pradesh: 19,177,242
2. "How many cases have been pending for over 30 years in Bihar?" → 22,420
3. "Show me the top 5 districts with highest pending cases in Uttar Pradesh"
4. "Which districts have more than 10000 cases pending for over 10 years?" → 142 districts

**Simulation:** Scroll to the simulation cell in the notebook — output shows 30% more judges cuts UP backlog from 19.1M → 13.4M.

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

District and Taluka Court Cases — sourced from NJDG (National Judicial Data Grid, Supreme Court of India)
