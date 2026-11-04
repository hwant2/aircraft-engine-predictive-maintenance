# Aircraft Engine Predictive Maintenance — Visualizations

## Overview

This folder contains seven visualizations developed during the exploratory analysis of NASA's simulated C-MAPSS FD001 aircraft engine dataset.

The charts illustrate engine operating cycles, remaining useful life (RUL), sensor relationships, and degradation patterns.

## Visualization Files

| File | Analytical Purpose |
|---|---|
| `Sensor_11_vs_RUL.png` | Examine Sensor 11's relationship with RUL |
| `Sensor_15.png` | Explore Sensor 15 behavior |
| `Sensor_4.png` | Explore Sensor 4 behavior |
| `distribution.png` | Display the distribution of an analyzed variable |
| `remaining.png` | Visualize remaining useful life |
| `representative.png` | Compare RUL trends across representative engines |
| `top_10.png` | Summarize the top 10 variables selected in the analysis |

## Key Correlation Findings

**Negative correlations with RUL**

- Operating cycles: -0.736
- Sensor 11: -0.696
- Sensor 4: -0.679
- Sensor 15: -0.643

**Positive correlations with RUL**

- Sensor 12: +0.672
- Sensor 7: +0.657
- Sensor 21: +0.636
- Sensor 20: +0.629

## Maintenance Applications

These visualizations demonstrate how engine condition data can help identify degradation trends, evaluate potential condition-monitoring indicators, and support future RUL prediction research.

Correlations describe statistical relationships, not proof of causation or validated failure-prediction performance.

## Limitations

The dataset contains simulated turbofan engine data. The charts represent exploratory findings and should not be interpreted as validated maintenance thresholds or operational failure predictions.
