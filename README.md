🌆 Big Data Urban Heat Island (UHI) Prediction
📌 Project Overview

This project develops a machine learning–based Urban Heat Island (UHI) prediction model using big geospatial and satellite datasets to identify and quantify heat hotspots at a micro-scale (meter-level) across New York City.

The work was completed as part of the 2025 EY Open Science AI & Data Challenge, which focuses on leveraging AI, satellite imagery, and open data to address climate and sustainability challenges.

The primary goal is to predict UHI Index values and understand the key drivers of urban heat, supporting data-driven decision-making for urban planning and climate resilience.

🎯 Problem Statement

Urban Heat Islands (UHIs) cause certain city regions to experience significantly higher temperatures than surrounding areas, leading to:

Increased health risks

Higher energy consumption

Greater impact on vulnerable populations

Traditional UHI models often rely on coarse satellite surface temperatures. This project improves upon that by combining ground-level temperature data with high-resolution satellite and urban features.

🗂️ Repository Structure
├── Big_Data_UHI_Prediction.ipynb     # Final model, analysis & results
├── Sentinel2_GeoTIFF.ipynb           # Sentinel-2 processing & NDVI features
├── Landsat_LST.ipynb                 # Landsat Land Surface Temperature extraction
├── data/                             # Processed & intermediate datasets
├── outputs/                          # Predictions, maps, and results
└── README.md

📊 Data Sources

The model integrates multiple open datasets:

Ground-level air temperature data (CAPA Strategies – Heat Watch Program)

Sentinel-2 satellite imagery

NDVI (vegetation index)

Water and urban density indicators

NASA Landsat thermal imagery

Land Surface Temperature (LST)

Building footprint & urban density data

Local weather data (New York State Mesonet)

All datasets are open-access and aligned with challenge guidelines 

2025 EY Open Science AI Data Ch…

🧠 Feature Engineering

Key features engineered include:

NDVI (Normalized Difference Vegetation Index)

Land Surface Temperature (LST)

Building density proximity metrics

Urban vs vegetation coverage indicators

Spatial joins between satellite pixels and ground data points

🤖 Modeling Approach

Target Variable: UHI Index

UHI Index = Local Temperature / Mean City Temperature


Train/Test Split: 70/30

Algorithms Used:

Tree-based regression models

Ensemble learning techniques

Evaluation Metric: R² (Coefficient of Determination)

The final model improves spatial interpretability and highlights key environmental drivers of heat intensity.

📈 Results

Successfully identified UHI hotspots and cool zones

Demonstrated strong correlation between:

Low vegetation density

High building density

Elevated surface temperatures

Outputs can support urban planning, heat mitigation, and climate policy decisions

📌 Final predictions and visualizations are available in:
Big_Data_UHI_Prediction.ipynb

🛠️ Tech Stack

Python

Jupyter Notebook

NumPy, Pandas

GeoPandas, Rasterio

Scikit-learn

Satellite & Geospatial Data Processing

🚀 How to Run
pip install -r requirements.txt
jupyter notebook


Run notebooks in the following order:

Sentinel2_GeoTIFF.ipynb

Landsat_LST.ipynb

Big_Data_UHI_Prediction.ipynb

🌍 Impact & Applications

Urban heat mitigation planning

Climate resilience strategies

Public health risk assessment

Scalable to other global cities

📚 References

EY Open Science AI & Data Challenge (2025)

NASA Landsat Mission

ESA Sentinel-2 Program

CAPA Strategies – Heat Watch Program 

2025 EY Open Science AI Data Ch…

👤 Author

Aman Jhagta
📌 MS in Business Analytics
🔗 Portfolio: https://amanjhagta.github.io/Portfolio

🔗 GitHub: https://github.com/Amanjhagta
