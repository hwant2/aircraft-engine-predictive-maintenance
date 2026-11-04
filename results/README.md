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

## 7. Maintenance and Reliability Recommendations

Based on the exploratory analysis of NASA's C-MAPSS FD001 dataset, the following recommendations identify opportunities for future condition-monitoring and predictive maintenance development.

### Recommendation 1 — Prioritize Relevant Sensor Measurements

Evaluate Sensors 11, 4, 15, 12, 7, 21, and 20 as initial candidates for further condition-monitoring research because of their observed relationships with remaining useful life.

Sensor selection should be validated using predictive performance, engineering interpretation, and operating-condition sensitivity rather than correlation alone.

### Recommendation 2 — Monitor Degradation Trends

Analyze changes in sensor measurements across operating cycles to identify gradual degradation patterns.

Future monitoring systems should consider trends, rates of change, and combinations of sensor measurements rather than relying on individual readings.

### Recommendation 3 — Develop an RUL Prediction Model

Use the exploratory findings as a foundation for developing and evaluating a remaining useful life prediction model.

Potential approaches include regression models, random forests, gradient boosting, and sequence-based neural networks.

Model performance should be evaluated using held-out engines, appropriate error metrics, and leakage-resistant validation procedures.

### Recommendation 4 — Investigate Maintenance Decision Thresholds

After validating a predictive model, evaluate whether estimated RUL could support inspection planning, maintenance scheduling, and component replacement decisions.

Any proposed maintenance thresholds would require engineering validation and consideration of prediction uncertainty, failure consequences, and operational requirements.

### Recommendation 5 — Evaluate Operational Benefits

Future work should compare predictive maintenance recommendations with baseline maintenance strategies.

Relevant performance measures could include:

- Unplanned equipment downtime.
- Maintenance scheduling effectiveness.
- Inspection and replacement costs.
- Equipment availability.
- False alarms and missed failure warnings.
- Prediction accuracy and uncertainty.

### Recommendation Summary

The analysis provides evidence of statistical relationships between sensor measurements and calculated remaining useful life. These relationships support further predictive maintenance research but do not yet demonstrate operational failure prediction or measurable maintenance cost savings.
