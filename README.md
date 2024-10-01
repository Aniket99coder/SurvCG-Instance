# SurvCG-Instance
This repository contains an instance to run SurvCG - data related to flight operations, including details about flights, costs associated with connections, and the arcs representing connections between various flight segments. 

## Files Included

- **`filtered_df_top_-1_2-5_12_9E_60.csv`**: A dataset of flight operations with various features, including year, month, airline, and scheduled times.
- **`cost_elapsed_top_-1_2-5_12_9E_60.npy`**: NumPy array containing elapsed costs for flight connections.
- **`cost_connections_top_-1_2-5_12_9E_60.npy`**: NumPy array with cost details related to different flight connections.
- **`arcs_top_-1_2-5_12_9E_60.npy`**: NumPy array representing the arcs connecting flight segments.

## Usage

To load the data, use the following Python code:

```python
import pandas as pd
import numpy as np

# Load the dataset
df_instance = pd.read_csv('path/to/filtered_df_top_-1_2-5_12_9E_60.csv')
cost_elapsed = np.load('path/to/cost_elapsed_top_-1_2-5_12_9E_60.npy')
cost_connections = np.load('path/to/cost_connections_top_-1_2-5_12_9E_60.npy')
arcs = np.load('path/to/arcs_top_-1_2-5_12_9E_60.npy')
