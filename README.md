# Renewable-Energy-Potential-Analyzer

 🌍 Renewable Energy Potential Analyzer

## 🧭 Project Overview

This project aims to accelerate renewable energy adoption by identifying high-potential locations and predicting project success through geospatial and financial analysis.

---

## 📦 Key Deliverables

- ✅ Renewable energy potential maps (solar/wind/hydro)

- ✅ Site suitability classification model

- ✅ Cost-benefit analysis tool (NPV, IRR)

- ✅ Investment opportunity ranker

---

## 👥 Team Roles

We are a team of 3 data fellows working collaboratively to achieve the core deliverables under a tight timeline. Tasks are distributed and aligned with each phase of the project.

---

## 🔧 Action Plan

### Phase 1: Discovery & Setup *(1–2 days)*

- [ ] Set up project folder structure (`data/`, `notebooks/`, `scripts/`, etc.)

- [ ] Install dependencies: `rasterio`, `geopandas`, `pandas`, `matplotlib`, `xgboost`, etc.

- [ ] Download and document data:

- [ ] Global Solar/Wind Atlas GeoTIFFs

- [ ] NASA POWER weather data (via API)

- [ ] World Bank electricity access data (CSV or API)

- [ ] Digital Elevation Model (DEM) from SRTM

- [ ] Create a `data_catalog.yaml` or spreadsheet with metadata

---

### Phase 2: Data Processing & Mapping *(2–3 days)*

- [ ] Clip GeoTIFFs to region of interest (e.g., Kenya)

- [ ] Reproject all rasters to the same CRS

- [ ] Extract and visualize:

- [ ] Solar potential (GHI)

- [ ] Wind potential (100m)

- [ ] Elevation, land cover, population (if used)

- [ ] Generate static or interactive maps (`matplotlib`, `folium`)

---

### Phase 3: Site Suitability Classification Model *(3–4 days)*

- [ ] Prepare a modeling dataset from raster + tabular features

- [ ] Engineer features: solar, wind, elevation, temperature, etc.

- [ ] Label sites based on suitability (rules or synthetic labels)

- [ ] Train and evaluate a Gradient Boosting model (XGBoost)

- [ ] Visualize feature importance and classification results

---

### Phase 4: Cost-Benefit Analysis *(2–3 days)*

- [ ] Estimate energy output per site (e.g., GHI × efficiency × size)

- [ ] Apply financial formulas:

- [ ] NPV (Net Present Value)

- [ ] IRR (Internal Rate of Return)

- [ ] Payback Period

- [ ] Define economic assumptions (installation cost, tariffs, etc.)

- [ ] Build a cost-benefit table per site

---

### Phase 5: Investment Opportunity Ranker *(1–2 days)*

- [ ] Define ranking formula using key indicators:

- NPV, IRR, energy output, access gap, distance to grid, etc.

- [ ] Normalize and weight each component

- [ ] Generate a ranked list of top candidate locations

---

### Phase 6 (Optional): Dashboard *(1–2 days)*

- [ ] Build an interactive dashboard using Streamlit or Plotly Dash

- [ ] Include:

- [ ] Potential maps

- [ ] Suitability predictions

- [ ] Ranked investment table

- [ ] Filters and download options

---

## 🗂️ Project Structure (Suggested)

├── README.md

├── data/

│ ├── raw/

│ ├── processed/

├── notebooks/

│ ├── 01_exploration.ipynb

│ ├── 02_mapping.ipynb

│ ├── 03_modeling.ipynb

├── scripts/

│ ├── data_download.py

│ ├── preprocessing.py

│ ├── model.py

│ ├── financials.py

├── outputs/

│ ├── maps/

│ ├── reports/

├── requirements.txt

---

## ✅ Dependencies

- Python 3.8+

- rasterio

- geopandas

- pandas

- numpy

- matplotlib

- scikit-learn

- xgboost

- folium or plotly

- streamlit (optional)

---

## 🚀 Getting Started

1. Clone this repository

2. Create a virtual environment and install dependencies

3. Begin with `notebooks/01_exploration.ipynb` to explore data

4. Proceed through each notebook in sequence or divide work among team

---

## 📅 Timeline Summary

| Phase | Duration |

|-------|----------|

| Phase 1: Setup | 1–2 days |

| Phase 2: Mapping | 2–3 days |

| Phase 3: Modeling | 3–4 days |

| Phase 4: Financials | 2–3 days |

| Phase 5: Ranking | 1 day |

| Phase 6: Dashboard (Optional) | 1–2 days |
	

