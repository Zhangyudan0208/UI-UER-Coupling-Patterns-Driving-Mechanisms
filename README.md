# UI-UER-Coupling-Patterns-Driving-Mechanisms

This repository contains the data and code used in the paper:

> **GeoAI-Based Spatiotemporal Evolution of Coupling Patterns and Driving Mechanisms between Urbanization and Ecological Resilience: Evidence from 278 Chinese Cities**

The repository is organised into three main folders:

---

## 1. `DATA`

- `All_indi_Year.csv`  
  - Annual base indicators for all cities.

- `df_Year_result.xlsx`  
  - Yearly city-level results of **Urbanization Intensity (UI)**, **Urban Ecological Resilience (UER)** and their **Coupling Coordination Degree (CCD)**.

- `DATA_processing/`  
  - Code used to calculate UI, UER and CCD from the raw indicators.

---

## 2. `Clustering`

- `CCD_06_22.csv`  
  - Input CCD time-series matrix for clustering (cities × years, 2006–2022).

- `cluster.ipynb`  
  - Soft-DTW K-means time-series clustering code.

- `labels_noprovin0911.csv`  
  - Resulting cluster labels for each city.

---

## 3. `SHAP`

- `shap.ipynb`  
  - Code for training the XGBClassifier and performing TreeSHAP analysis to interpret the drivers of the CCD clusters.
