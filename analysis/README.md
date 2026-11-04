# Aircraft Engine Predictive Maintenance — Python Analysis

## Overview

This folder contains the Jupyter notebook used to analyze NASA's simulated C-MAPSS FD001 turbofan engine dataset.

The analysis examines engine operating cycles, sensor measurements, degradation patterns, and remaining useful life (RUL).

## Notebook

**File:** `Engine Data.ipynb`

The notebook contains exploratory data analysis, RUL calculations, sensor correlation analysis, and data visualizations.

## Technology Stack

- Python 3
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook / Google Colab

## Dataset

The training dataset is located at:

`../data/train_FD001.txt`

The repository also contains:

`../data/RUL_FD001.txt`

The training dataset contains:

- 100 simulated turbofan engines
- 20,631 observations
- 26 original columns
- 3 operational settings
- 21 sensor measurements

The analysis creates an additional RUL column, bringing the working dataset to 27 columns.

## Reproducing the Analysis

1. Open `Engine Data.ipynb` in Google Colab or Jupyter Notebook.
2. Ensure the required Python libraries are installed.
3. Load `train_FD001.txt` from the repository's `data` folder.
4. Run the notebook cells in sequence.
5. Review the generated sensor correlations, degradation trends, and RUL visualizations.
6. Compare the findings with the documentation in `../results/README.md`.

**Important:** If the notebook uses an interactive file-upload step, upload `train_FD001.txt` when prompted. Local file paths may need adjustment depending on the execution environment.

## RUL Calculation

For each training engine:

**RUL = Final Observed Engine Cycle − Current Engine Cycle**

The calculation was validated across all 20,631 observations, with no negative RUL values and all 100 engines reaching RUL zero.

## Analysis Outputs

The notebook supports:

- Dataset inspection and exploratory analysis.
- Sensor-to-RUL correlation analysis.
- Visualization of engine degradation trends.
- Comparison of representative engine lifecycles.
- Identification of candidate sensors for future predictive modeling.

Generated charts are available in the repository's `visualizations` folder.

## Limitations

This project uses simulated engine data. The notebook performs exploratory analysis and does not report independently validated predictive-model accuracy or operational maintenance outcomes.
