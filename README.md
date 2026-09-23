# Aircraft Engine Predictive Maintenance Analysis

## Project Overview

This project analyzes aircraft engine sensor data to identify patterns associated with engine degradation and remaining useful life (RUL).

The analysis uses the NASA C-MAPSS FD001 dataset and applies data analytics techniques to examine engine operating cycles, sensor behavior, and indicators of declining engine performance.

The goal is to demonstrate how data can be used to support predictive maintenance and maintenance planning in an aerospace and manufacturing environment.

## Business Problem

Unplanned equipment failures can result in production delays, increased maintenance costs, and reduced equipment availability.

Predictive maintenance uses historical and operational data to identify patterns that may indicate equipment degradation before failure occurs.

This project examines aircraft engine data to determine which measurements provide useful indicators of remaining useful life and how those indicators could support maintenance decisions.

## Objectives

The analysis focuses on the following questions:

1. How does engine condition change as operating cycles increase?
2. Which sensors show the strongest relationship with remaining useful life?
3. What patterns appear as engines approach failure?
4. Which engines have the shortest and longest useful operating lives?
5. How can the findings support predictive maintenance planning?

## Dataset

The project uses the NASA C-MAPSS FD001 dataset.

The dataset contains simulated turbofan engine degradation data collected across multiple engines and operating cycles.

The analysis dataset contains:

- 100 engines
- 20,631 observations
- 27 columns
- Engine operating cycles
- Multiple sensor measurements
- Remaining useful life (RUL)

## Tools Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Data analysis and visualization
- GitHub

## Key Analysis

The analysis examined:

- Engine operating cycles
- Sensor measurements
- Remaining useful life
- Correlations between sensor measurements and RUL
- Engine degradation patterns
- Differences in useful operating life
- Potential predictive maintenance indicators

## Key Findings

Several sensor measurements showed meaningful relationships with remaining useful life.

The strongest negative relationships with RUL included:

- Time in cycles
- Sensor 11
- Sensor 4
- Sensor 15
- Sensor 2
- Sensor 17
- Sensor 3

Several sensors showed positive relationships with RUL, including:

- Sensor 12
- Sensor 7
- Sensor 21
- Sensor 20

These relationships provide insight into which measurements may be useful when monitoring engine degradation.

## Maintenance Application

The results demonstrate how historical equipment data can be used to identify degradation patterns and support predictive maintenance.

In a manufacturing or aerospace environment, similar analytical approaches could help maintenance teams:

- Identify equipment showing signs of degradation
- Prioritize inspections
- Plan maintenance before failure
- Reduce unexpected downtime
- Improve equipment availability
- Support data-driven maintenance decisions

## Project Structure

```text
aircraft-engine-predictive-maintenance/
│
├── analysis/
├── data/
├── documentation/
├── results/
├── visualizations/
├── .gitignore
└── README.md

## Author

Harold Wanton

Data Analytics | Manufacturing | Maintenance | Predictive Maintenance
