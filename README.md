 Weather Data Quality Audit Pipeline

## Overview
This script automates quality control checks on environmental sensor logs stored in a CSV format. It evaluates total row counts, detects data gaps, and runs descriptive statistics to assess metric baselines and volatility.

## Script Features
* **Structural Inspection:** Counts total records processed and features tracked using dataset shape metrics.
* **Missing Value Detection:** Scans every column for null entries using `.isnull().sum()` to pinpoint data gaps.
* **Temperature Audit:** Calculates baseline average, maximum threshold, minimum threshold, and standard deviation (volatility) for the Temperature column.
* **Humidity Audit:** Calculates average, maximum, and minimum levels for the Humidity column.