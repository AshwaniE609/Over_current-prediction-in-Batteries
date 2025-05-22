# EV Battery Fault Analysis: Overcurrent Detection and Prediction


Overview

This project analyzes battery telemetry data from electric vehicles (EVs) to identify and predict overcurrent faults—a critical battery failure mode that can lead to safety risks or hardware damage. The workflow covers data exploration, fault labeling, pattern discovery, and machine learning-based prediction.


Features

Exploratory Data Analysis (EDA): Visualize and understand EV battery sensor data.

Fault Labeling: Automatically flag overcurrent events based on current thresholds.

Pattern Discovery: Analyze trends and correlations in battery behavior.

Machine Learning: Train models to predict overcurrent faults using historical data.


Dataset

The dataset contains time-series telemetry from EVs, including:

timestamp: Date and time of reading

device_id: Unique vehicle identifier

lat, lon: GPS coordinates

soc: State of Charge (%)

odo: Odometer (km)

v: Voltage (V)

i: Current (A)


Additional columns for imputed values and previous readings are generated during preprocessing.

Project Structure

Fault_analysis.ipynb    # Main analysis notebook

data/

  └── battery_data.csv  # (Example) Raw telemetry data

README.md               # Project documentation

How to Run

Clone the repository:

bash

git clone https://github.com/yourusername/ev-battery-fault-analysis.git

cd ev-battery-fault-analysis


Install dependencies:

Python 3.8+

pandas

seaborn

matplotlib

Install with pip:

bash

pip install pandas seaborn matplotlib

Open and run the notebook:

Use Jupyter Notebook or VSCode to open Fault_analysis.ipynb.

Follow the notebook cells for step-by-step analysis.

Usage

Data Exploration: Visualize sensor distributions and trends.

Fault Labeling: Identify overcurrent events using customizable thresholds.

Model Training: Build and evaluate predictive models for overcurrent detection.

Pattern Analysis: Discover operational patterns that precede faults.


Example Data Snapshot

timestamp	device_id	lat	lon	soc	odo	v	i

2024-11-22 19:05:00+05:30	4401084597612	22.60145	88.23076	98.0	547.8	53.19	0.0

2024-11-22 19:06:00+05:30	4401084597612	22.60145	88.23076	98.0	547.8	53.19	0.0


Contributing

Contributions are welcome! Please open an issue or submit a pull request for suggestions, bug fixes, or new features.

License

This project is released under the MIT License.

Acknowledgments

Battery data and problem statement inspired by real-world EV fleet challenges.

Built using open-source Python libraries: pandas, seaborn, matplotlib.
