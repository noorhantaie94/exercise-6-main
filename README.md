#  Raster Data Processing & NDVI Satellite Imagery Mapping

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg)](https://www.python.org/)
[![xarray](https://img.shields.io/badge/Library-xarray-orange.svg)](https://docs.xarray.dev/)
[![rioxarray](https://img.shields.io/badge/Library-rioxarray-green.svg)](https://corteva.github.io/rioxarray/)
[![License](https://img.shields.io/badge/License-MIT-brightgreen.svg)](LICENSE)

## Project Overview
This repository contains the complete spatial raster processing workflow for **Exercise 6** of the *Automating GIS Processes* course. The project applies advanced multi-dimensional raster analysis using Python (`xarray` and `rioxarray`) on climatic datasets and Sentinel-2 satellite imagery.

---

## 📂 Core Features & Workflow

### 🌡️ Problem 1: Finland Temperature Analysis & Raster Mapping
- Processed daily $10\text{ km} \times 10\text{ km}$ spatial temperature grids across Finland.
- Converted raw raster units and extracted spatial temperature statistics.
- Visualized spatial temperature distributions with customized map layouts and colormaps.

### 🌲 Problem 2: Sentinel-2 Satellite Imagery Analysis & NDVI Mapping
Analysis focused on **Nuuksio National Park, Finland**:
1. **Metadata Extraction:** Extracted Spatial Reference System (CRS), spatial resolution, raster dimensions, and NoData values.
2. **Band Mapping:** Selected Red (Band 4) and Near-Infrared / NIR (Band 8) spectral bands.
3. **NDVI Calculation:** Applied the Normalized Difference Vegetation Index formula:
   $$\text{NDVI} = \frac{\text{NIR} - \text{Red}}{\text{NIR} + \text{Red}}$$
4. **Reclassification:** Categorized vegetation health into distinct zones (Non-vegetated, Sparse/Moderate, and Dense Vegetation).
5. **Visualization:** Plotted spatial NDVI classification maps and raster pixel distribution histograms.
6. **Data Export:** Exported processed vegetation raster data to `NDVI.tif`.

---

## Tools & Libraries
- **Python 3.10+**
- **xarray** & **rioxarray** (Multi-dimensional raster array manipulation)
- **matplotlib** (Data visualization & geospatial plotting)
- **numpy** (Array numerical computing)

---

## How to Run

1. Clone this repository:
   ```bash
   git clone [https://github.com/noorhantaie94/exercise-6-main.git](https://github.com/noorhantaie94/exercise-6-main.git)
   cd exercise-6-main
