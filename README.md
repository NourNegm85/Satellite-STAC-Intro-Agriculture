# Satellite Data Analysis with Python  
## Introduction to STAC (SpatioTemporal Asset Catalog) & NDVI Time-Series

[![YouTube](https://img.shields.io/badge/YouTube-dr.nour%20negm-red?style=flat&logo=youtube)](https://youtube.com/@dr.nournegm)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Profile-blue?style=flat&logo=linkedin)](https://www.linkedin.com/in/nour-ibrahim/)
[![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://www.python.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## 🌍 Project Overview

This repository accompanies an educational video from the  
**“Satellite Data with STAC & Python”** playlist on my YouTube channel.

The project demonstrates how to **discover, access, and analyze satellite imagery using STAC APIs and cloud-native Python tools**, without relying on Google Earth Engine (GEE).

In this tutorial, we:
- Query **Sentinel-2 Level-2A** imagery via a STAC catalog  
- Load cloud-optimized satellite data efficiently  
- Compute and visualize **NDVI time series**
- Work with fully **open, reproducible Python workflows**

---

## 🎯 Why STAC?

STAC (SpatioTemporal Asset Catalog) provides a standardized way to organize and access geospatial data stored in the cloud.

Learning STAC allows you to:
- Access satellite data directly from cloud providers
- Build scalable and reproducible workflows
- Avoid platform lock-in
- Use the same methodology across AWS, Microsoft Planetary Computer, and other STAC providers

---

## 🚀 What This Project Covers

- Searching satellite data using a **STAC API**
- Filtering imagery by:
  - Area of Interest (AOI)
  - Date range
  - Cloud cover
- Loading Sentinel-2 imagery as an **xarray data cube**
- Calculating **NDVI**
- Generating **time-series visualizations**
- Exporting results for further analysis

---

## 🛠️ Technology Stack

### Data
- **Sentinel-2 Level-2A Surface Reflectance**
- Accessed via **Element 84 / AWS STAC**

### Core Python Libraries
- `pystac-client`
- `odc-stac`
- `xarray`
- `rioxarray`
- `numpy`
- `matplotlib`
- `shapely`
- `geopandas`
- `netCDF4`
  
All required packages are listed in `requirements.txt`.

---

## 📂 Repository Structure

This repository is organized to keep data, code, and results separate and easy to find:

```text
.
├── aoi/
│   └── study_area.geojson      # Area of Interest: Spatial bounds for the query
│
├── notebooks/
│   └── 01_stac_ndvi_intro.ipynb # Main Tutorial: Step-by-step STAC & NDVI code
│
├── outputs/
│   ├── ndvi_timeseries.csv      # Extracted data for statistical analysis
│   ├── ndvi_plot.png            # Final NDVI growth curve visualization
│   └── ndvi_composite.tif       # Sample processed satellite image (NetCDF/GeoTIFF)
│
├── requirements.txt             # List of Python dependencies
└── README.md                    # Project documentation (this file)
```
---

## 📖 How to Use This Repository

### 1️⃣ Watch the Tutorial Video
📺 **YouTube:**  
👉 *[LINK]*

The notebook follows the video step by step.

---

### 2️⃣ Set Up the Environment

Clone the repository:

```bash
git clone https://github.com/NourNegm85/Satellite-STAC-Intro-Agriculture.git
```

Install dependencies:

```bash
pip install -r requirements.txt
```
---
3️⃣ Run the Notebook
jupyter notebook

---
You can modify:

AOI

Date range

Cloud cover threshold

Vegetation index calculation
---
Data & Documentation References

STAC Specification: https://stacspec.org

Element 84 STAC Catalog

Sentinel-2 Product Description (ESA)

---

## 👤 About the Author

**Dr. Nour Negm**  
PhD in Crop Genetics & Breeding  

Applying satellite data and open-source geospatial tools for agricultural and environmental analysis.

This repository is part of an ongoing effort to document practical, reproducible workflows that bridge academic research and real-world applications.

---
⭐ Support

If you find this repository useful:

⭐ Star the project

📺 Subscribe to the YouTube channel

🔁 Share it with others interested in satellite data & Python
