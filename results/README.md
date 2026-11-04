# Aircraft Engine Predictive Maintenance — Analysis Results

## 1. Dataset Overview

This project analyzes NASA's simulated C-MAPSS FD001 turbofan engine dataset to investigate equipment degradation and remaining useful life (RUL).

| Dataset Metric | Value |
|---|---:|
| Engines analyzed | 100 |
| Observations | 20,631 |
| Original dataset columns | 26 |
| Analysis columns including RUL | 27 |
| Sum of recorded operating-cycle values | 2,244,815 |
| Missing values in original dataset | 0 |
| Minimum calculated RUL | 0 cycles |
| Maximum calculated RUL | 361 cycles |

RUL was calculated by subtracting each engine's current operating cycle from its final observed cycle in the training dataset.

The calculation was validated across all observations. All 100 engines reached an RUL value of zero, and no negative RUL values were found.

## 2. Sensor Correlation Analysis

The analysis examined relationships between engine operating cycles, sensor measurements, and calculated RUL.

### Strongest Negative Correlations

| Variable | Correlation with RUL |
|---|---:|
| Time in cycles | -0.736 |
| Sensor 11 | -0.696 |
| Sensor 4 | -0.679 |
| Sensor 15 | -0.643 |
| Sensor 2 | -0.606 |
| Sensor 17 | -0.606 |
| Sensor 3 | -0.585 |

### Strongest Positive Correlations

| Variable | Correlation with RUL |
|---|---:|
| Sensor 12 | +0.672 |
| Sensor 7 | +0.657 |
| Sensor 21 | +0.636 |
| Sensor 20 | +0.629 |

These correlations are reported from the existing exploratory analysis. They describe associations within the simulated training dataset and do not establish causation.

## 3. Interpretation of Findings

Several sensor measurements demonstrate meaningful statistical relationships with remaining useful life.

Negative correlations indicate that higher measurements tend to be associated with lower RUL, while positive correlations indicate that higher measurements tend to be associated with higher RUL.

These relationships suggest that selected sensor measurements may be useful candidates for further condition-monitoring research and predictive modeling.

The correlations do not independently establish reliable failure-warning thresholds or prediction accuracy.

## 4. Maintenance Applications

The analysis demonstrates potential applications of equipment condition data in:

- Monitoring engine degradation over operating cycles.
- Identifying candidate sensors for condition monitoring.
- Supporting reliability analysis and maintenance planning.
- Developing future RUL estimation models.
- Evaluating opportunities for condition-based maintenance.

## 5. Analytical Limitations

- The dataset contains simulated turbofan engine measurements rather than live operational aircraft data.
- The reported findings are primarily descriptive and correlational.
- No validated predictive model performance metrics are reported.
- Sensor correlations may vary across operating conditions and different engine populations.
- Maintenance cost savings and downtime reductions have not been quantified or demonstrated.

## 6. Conclusion

The analysis identifies relationships between engine operating cycles, sensor measurements, and remaining useful life across 100 simulated turbofan engines.

The findings provide an exploratory foundation for future predictive maintenance development, including sensor selection, degradation monitoring, and machine-learning-based RUL estimation.
