## CS 224W Final Project

**2013 US flight delay prediction with SkyNet: Graph Neural Networks for Edge Regression.**

### Built with
<img src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54" height="20" /> <img src="https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white" height="20" /> <img src="https://img.shields.io/badge/PyG-%233C2179.svg?style=for-the-badge&logo=pytorch&logoColor=white" height="20" /> <img src="https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white" height="20" /> <img src="https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white" height="20" /> <img src="https://img.shields.io/badge/Google%20Earth%20Engine-4285F4?style=for-the-badge&logo=googleearth&logoColor=white" height="20" />

### About
SkyNet predicts flight delays by modeling the US air traffic network as a graph. Unlike standard regression, we treat delay prediction as an **edge-regression task**, integrating flight schedules with high-resolution **ERA5 weather data** to capture cascading delays and spatial dependencies.

### Repository Files

| Notebook | Description |
| :--- | :--- |
| **`gcn_solution.ipynb`** | **Main Solution:** Static GCN + Edge MLP. Best performing model. |
| **`T_GCN.ipynb`** | **Temporal GCN:** Experimental GCN + GRU model for time-series updates. |
| **`naive_regression.ipynb`** | **Baseline:** Standard Ridge Regression on tabular flight data. |
| **`no_weather_gcn.ipynb`** | **Ablation:** GCN trained without weather features. |
| **`no_tail_number_gcn.ipynb`** | **Ablation:** GCN trained without aircraft tail numbers. |
| **`224_project_data_exploration.ipynb`** | **Data Prep:** Processing Kaggle flights and Google Earth Engine weather data. |
