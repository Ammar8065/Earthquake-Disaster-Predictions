# Earthquake Impact Prediction and Resource Allocation System

![Earthquake Prediction](https://img.shields.io/badge/Python-3.11-blue) ![License](https://img.shields.io/badge/License-MIT-green) ![Status](https://img.shields.io/badge/Status-Completed-success)

## Overview

This project develops a machine learning system to predict earthquake magnitudes, assess their impact, and allocate resources to affected areas. Using historical earthquake data from the USGS (sourced from Kaggle), the system employs an LSTM model for magnitude prediction, a Random Forest classifier for impact assessment, and a greedy algorithm for resource allocation. Visualizations are created using Plotly (time-series plots) and Folium (interactive maps), displayed directly in a Jupyter Notebook environment.

The project was built as a zero-cost solution, leveraging free tools and datasets, making it accessible for educational and portfolio purposes.

---

## Features

- **Magnitude Prediction**: Uses an LSTM model to predict future earthquake magnitudes based on historical data.
- **Impact Assessment**: Classifies earthquake impact into Low, Moderate, and Severe categories using a Random Forest classifier.
- **Resource Allocation**: Allocates resources (e.g., food, water, rescue teams) to Moderate and Severe quakes using a greedy algorithm.
- **Visualizations**:
  - Time-series plot of earthquake magnitudes over time (Plotly).
  - Interactive map showing earthquake locations and impact levels (Folium).
- **Environment**: Designed to run in Jupyter Notebook for in-notebook visualizations, with no reliance on HTML files or external dashboards.

---

## Dataset

The project uses two datasets from Kaggle (e.g., USGS Earthquake Catalog):
- **usgs_main.csv**: Historical earthquake data for training (larger dataset).
- **usgs_current.csv**: Recent earthquake data for testing (smaller dataset).

**Columns**:
- `time`: Date and time of the earthquake (DateTime).
- `latitude`, `longitude`: Coordinates of the earthquake (Float).
- `depth`: Depth in kilometers (Float).
- `mag`: Magnitude of the earthquake (Float).
- `place`: Descriptive location (String).
- `nst`, `gap`: Seismic station data (Integer, Float).
- And more (e.g., `magType`, `dmin`, etc.).

**Note**: You’ll need to download the dataset from Kaggle and place it in the `Earthquakes Dataset` folder. Update the `folder_path` in the code to match your local path.

---

## Installation

### Prerequisites
- Python 3.11 (recommended, as TensorFlow may not fully support Python 3.12 as of March 2025).
- Jupyter Notebook (for in-notebook visualizations).
- Anaconda (optional, for managing environments).

### Steps
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/earthquake-prediction.git
   cd earthquake-prediction
