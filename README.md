# Layoffs Time Series Analysis (Interactive)

A small data-exploration notebook that cleans a layoffs dataset, engineers time features, and produces **time-series + breakdown visualizations** using **Plotly**, plus an **interactive filter dashboard** (industry / country / stage) using **ipywidgets**.

## What this notebook does

- Loads a layoffs CSV dataset
- Cleans and standardizes columns
- Parses the `date` column and creates:
  - `year`
  - `month`
  - `year_month` (monthly period)
- Computes quick headline stats:
  - Total people laid off
  - Number of layoff events
  - Average % laid off
  - Median funds raised (millions)
- Builds monthly trends:
  - Layoff events per month
  - Total laid off per month
  - Avg % laid off per month
- Breakdowns (Top 15):
  - By **industry**
  - By **country**
  - By **company stage**
- Distributions:
  - `% laid off`
  - `total_laid_off`
  - `funds_raised_millions`
  - Severity buckets based on `% laid off`
- Interactive view:
  - Dropdown filters for **industry**, **country**, **stage**
  - Updates monthly event and total-laid-off trend lines

## Outputs (visuals)

- Line charts (monthly): events, total laid off, avg % laid off
- Bar charts: top industries, countries, stages
- Histograms: percent laid off, total laid off, funds raised
- Widget-driven filtered time-series charts

## Requirements

Install dependencies:

```bash
pip install pandas numpy plotly ipywidgets
