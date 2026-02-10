# 🌆 Big Data Urban Heat Island (UHI) Prediction

## Overview
This project builds a machine-learning model to predict **Urban Heat Island (UHI) intensity** at micro-scale resolution across **New York City** using **satellite imagery, geospatial data, and ground-level temperature measurements**.  
It was developed as part of the **2025 EY Open Science AI & Data Challenge**.

## Problem
Urban Heat Islands cause certain city areas to experience significantly higher temperatures, leading to health risks, increased energy demand, and greater impact on vulnerable populations.  
Traditional UHI models rely on coarse satellite data; this project improves accuracy by integrating **ground measurements with high-resolution satellite features**.

## Repository Structure
├── Big_Data_UHI_Prediction.ipynb # Final model & results
├── Sentinel2_GeoTIFF.ipynb # NDVI & satellite feature extraction
├── Landsat_LST.ipynb # Land Surface Temperature processing
├── data/ # Processed datasets
├── outputs/ # Predictions & maps
└── README.md


## Data Sources
- Ground-level air temperature data (CAPA Strategies – Heat Watch)
- Sentinel-2 multispectral satellite imagery (NDVI, water, urban density)
- NASA Landsat thermal imagery (Land Surface Temperature)
- Building footprint and urban density data
- Local weather data (NY State Mesonet)

## Feature Engineering
- Normalized Difference Vegetation Index (NDVI)
- Land Surface Temperature (LST)
- Building density proximity metrics
- Vegetation and water proximity indicators
- Spatial joins between satellite pixels and ground observations

## Modeling Approach
- **Target:** UHI Index (local temperature relative to city mean)
- **Split:** 70/30 train–test
- **Models:** Tree-based and ensemble regression
- **Metric:** R² (Coefficient of Determination)

## Results
- Identified urban heat hotspots and cooler zones at meter-level resolution
- Strong correlation between low vegetation, high building density, and elevated temperatures
- Results support urban planning, climate resilience, and heat-mitigation strategies  
**Final outputs are available in `Big_Data_UHI_Prediction.ipynb`.**

## Tech Stack
Python · Pandas · NumPy · GeoPandas · Rasterio · Scikit-learn · Jupyter Notebook

## How to Run
```bash
pip install -r requirements.txt
jupyter notebook

Run notebooks in this order:

Sentinel2_GeoTIFF.ipynb

Landsat_LST.ipynb

Big_Data_UHI_Prediction.ipynb

Applications

Urban planning · Climate adaptation · Public health risk analysis · Scalable to other cities

Author

Aman Jhagta
Portfolio: https://amanjhagta.github.io/Portfolio

GitHub: https://github.com/Amanjhagta
