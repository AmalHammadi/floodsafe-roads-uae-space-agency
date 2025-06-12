# FloodSafe Roads – UAE Space Agency Project 

**FloodSafe Roads** is a satellite-powered flood risk mapping system designed to identify and visualize flood-prone areas across the UAE. It helps support disaster response, infrastructure planning, and long-term climate resilience.  
This project was developed as part of the **Space Hackathon 2024**, where it won in the **Space for Sustainability** category.

---

## Project Overview

Extreme rainfall events in the UAE can cause sudden flooding, damaging infrastructure and disrupting transportation. FloodSafe Roads analyzes satellite data to:

- Detect and monitor flooded areas using remote sensing
- Generate flood risk maps using NDWI (Normalized Difference Water Index)
- Support proactive urban planning and emergency response

---

## Tools & Technologies Used

### Collected Data

The project utilizes a combination of satellite imagery and historical flood data to detect, map, and analyze flood-prone areas in the UAE.

| Data Source | Description |
|-------------|-------------|
| **Sentinel-2 Satellite Imagery** | Used to compute NDWI (Normalized Difference Water Index) for detecting surface water before and after rainfall events. |
| **Sentinel-1 SAR Imagery** | Used for radar-based flood detection, especially useful in cloud-covered conditions. |
| **Historical Flood Records** | Ground-truth data from previous flood events in the UAE to validate remote sensing results and improve flood risk modeling. |
| **Rainfall Event Data (April 16, 2024)** | Focused analysis of an extreme rainfall event for evaluating flood impact using time-series imagery. |
| **Topographic & Infrastructure Layers** | Roads, urban boundaries, and land use maps used for overlay and impact assessment. |

###  Remote Sensing Software Used

| Software | Purpose |
|----------|---------|
| **SNAP (Sentinel Application Platform)** by ESA | Used to preprocess Sentinel-1 and Sentinel-2 imagery, including atmospheric correction, band extraction, and calibration for NDWI and SAR analysis. |
| **Google Earth Engine (GEE)** | Used for large-scale NDWI processing, water body detection, and time-series visualization directly in the cloud without downloading full datasets. |
| **QGIS** | Used for visualizing NDWI results, overlaying flood risk zones with roads, infrastructure, and agricultural land, and generating final flood maps. Also supports exporting GeoTIFF and shapefile outputs. |

### 🛰️ Remote Sensing & Image Processing
- **Sentinel-1** and **Sentinel-2** satellite imagery
- **NDWI Index** for water detection
- **Google Earth Engine** (optional for large-scale processing)
- **QGIS** for spatial visualization

### Programming
- **Python** (main language)
  - Libraries: `numpy`, `matplotlib`, `rasterio`, `geopandas`, `earthpy`, `GDAL`
- **Jupyter Notebook** for data exploration and visualization
  
### 🤖 AI & Machine Learning

- **Machine Learning Models**: Trained on historical flood data and NDWI outputs to classify flood-prone zones.
- **Supervised Classification**: Applied to Sentinel imagery to distinguish between water and non-water surfaces.
- **Python-based notebooks** used for feature extraction, model training, and accuracy evaluation.

  
## Features

- NDWI calculation from Sentinel-2 data
- Visualization of flooded areas before and after rainfall events
- Support for zooming into infrastructure (e.g., roads, agriculture zones)
- Exportable maps for disaster management use


## Achievements

-  **Winner** – Space Hackathon 2024, Space for Sustainability category  
-  Recognized for innovative use of satellite data in flood risk mapping  
-  Successfully integrated Sentinel-1 and Sentinel-2 data for accurate flood detection  
-  Improved flood risk predictions by combining historical flood records with remote sensing analysis  


