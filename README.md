Aircraft Engine Predictive Maintenance Analysis

Project Overview

This project analyzes aircraft engine sensor data to identify degradation patterns and relationships with remaining useful life (RUL).

The goal was to use data analytics to examine how engine operating cycles and sensor measurements change as an engine approaches the end of its useful life.

Business Problem

Aircraft and other complex mechanical systems require effective maintenance strategies to reduce unexpected failures, improve maintenance planning, and maximize equipment availability.

Predictive maintenance uses equipment data to identify patterns that may indicate degradation before a failure occurs.

This project applies that approach to aircraft engine data.

Dataset

The analysis uses the NASA C-MAPSS FD001 dataset.

The dataset contains simulated aircraft engine run-to-failure data with multiple sensor measurements collected throughout each engine’s operating life.

Dataset Summary

* 100 engines
* 20,631 observations
* 27 columns
* 2,244,815 total engine cycles

Analysis Performed

The analysis examined:

* Engine operating cycles
* Sensor behavior over time
* Remaining useful life
* Sensor-to-RUL relationships
* Degradation patterns
* Variables that may provide useful predictive-maintenance indicators

Python and data-analysis techniques were used to explore and interpret the data.

Key Findings

Several variables showed relatively strong relationships with remaining useful life.

Stronger Negative Relationships

Variable	Correlation with RUL
Time in cycles	-0.736
Sensor 11	-0.696
Sensor 4	-0.679
Sensor 15	-0.643
Sensor 2	-0.606
Sensor 17	-0.606
Sensor 3	-0.585

Stronger Positive Relationships

Variable	Correlation with RUL
Sensor 12	+0.672
Sensor 7	+0.657
Sensor 21	+0.636
Sensor 20	+0.629

These relationships indicate that several sensor measurements change in ways associated with remaining useful life and may be useful for further predictive-maintenance modeling.

Project Structure

aircraft-engine-predictive-maintenance/
│
├── Analysis/
│   ├── README.md
│   └── Engine data.ipynb
│
├── Data/
│   ├── README.md
│   ├── RUL_FD001
│   └── TRAIN_FD001
│
├── Documentation/
│   ├── README.md
│   └── Aircraft Engine Predictive Maintenance Analysis
│
├── Results/
│   └── README.md
│
├── Visualizations/
│   ├── README.md
│   └── Analysis Visualizations
│
└── README.md

Results

The analysis identified sensor variables that demonstrated meaningful relationships with remaining useful life.

These findings can support future predictive models designed to estimate RUL and identify potential degradation before equipment failure.

The results are documented in the Results folder.

Visualizations

The Visualizations folder contains charts created during the analysis to illustrate:

* Sensor relationships with RUL
* Engine degradation patterns
* Operating-cycle behavior
* Other supporting analysis results

Maintenance Applications

The analysis demonstrates how sensor data can support:

* Condition-based maintenance
* Predictive maintenance
* Early identification of degradation
* Maintenance planning
* Reduction of unexpected equipment downtime
* Data-driven maintenance decisions

Tools & Skills

Technical Skills

* Python
* Pandas
* Matplotlib
* Data Cleaning
* Exploratory Data Analysis
* Correlation Analysis
* Data Visualization
* Predictive Maintenance
* Remaining Useful Life Analysis

Industry Knowledge

* Aircraft and engine systems
* Mechanical maintenance
* Preventive maintenance
* Equipment troubleshooting
* Reliability concepts
* Manufacturing and industrial equipment

Documentation

The complete project report is available in the Documentation folder.

The analysis notebook is available in the Analysis folder.

Conclusion

This project demonstrates the use of data analytics to examine aircraft engine degradation and remaining useful life.

The analysis combines technical maintenance knowledge with data analytics to identify patterns that could support more proactive maintenance strategies.

⸻

Author: Harold Wanton
