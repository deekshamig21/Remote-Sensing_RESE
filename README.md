# RESE
# Evaluation of Recent Changes Using Multi-Satellite Remote Sensing Data for Indus River Basin

This project evaluates recent environmental and hydrological changes in the **Indus River Basin** using multi-satellite remote sensing datasets. By combining data from different sensors and platforms, we analyze spatial and temporal trends in water bodies, vegetation, and land use over recent years.

---

## Overview

The Indus River Basin spans across Pakistan, India, China, and Afghanistan and supports hundreds of millions of people. Understanding its recent changes is critical for:

- Water resource management 
- Agricultural planning 
- Climate adaptation 

This project uses **multi-source satellite imagery** to detect and assess these changes, particularly focusing on:

- Surface water extent
- Vegetation health (NDVI, EVI)
- Land use/land cover shifts
- Snow and glacier retreat

---

## Data Sources

We use open-access data from the following satellite missions:

| Satellite     | Sensors        | Use Case                |
|---------------|----------------|-------------------------|
| **Landsat 8/9**   | OLI, TIRS       | Land cover, NDVI         |
| **Sentinel-2**    | MSI             | High-res vegetation, LULC |
| **MODIS**         | MOD13Q1, MOD10A2| Long-term NDVI/Snow Cover|
| **GRACE/GRACE-FO**| Mass Anomaly    | Groundwater trends       |
| **SRTM/DEM**      | Elevation       | Terrain and basin modeling|

---

## Methodology

1. **Data Acquisition**  
   Earth Engine / AWS / Google Cloud Public Datasets

2. **Preprocessing**  
   - Cloud masking  
   - Atmospheric correction  
   - Image compositing

3. **Indices Computation**  
   - NDVI, EVI, NDSI, NDWI

4. **Trend Analysis**  
   - Time series modeling  
   - Anomaly detection  
   - Seasonal decomposition

5. **Visualization & Mapping**  
   - Interactive maps  
   - Temporal charts  
   - Comparative layouts



## Results 

- Vegetation trends from 2000–2024
- Retreat of glaciated areas in the upper basin
- Seasonal and inter-annual snow cover variation
- Long-term changes in surface water extent
- GRACE-based groundwater mass anomalies



## Tools & Libraries

- Google Earth Engine (GEE)
- Python (geemap, rasterio, numpy, matplotlib)
- QGIS / ArcGIS Pro
- Jupyter Notebooks
- Git & GitHub






