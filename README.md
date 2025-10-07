# climate-change-bird-migration-analysis
Data-driven analysis of how climate change affects bird migration patterns using multi-decade datasets from eBird, NOAA, and MODIS — includes spatial clustering, correlation studies, and predictive modeling with Random Forest &amp; Gradient Boosting.
  

**Website:** [Project Site ↗](https://sites.google.com/view/analysisofclimatechangebird/home)

---

## 🌍 Executive Summary
This project explores how **climate change impacts bird migration patterns** across decades of global data.  
Migratory species rely heavily on environmental cues like temperature and habitat conditions; climate shifts can disrupt timing and routes.  
I integrated large-scale datasets from **eBird (bird observations)**, **NOAA (climate)**, and **MODIS (land cover)** to analyze temporal, spatial, and environmental correlations.

The project was executed in three milestones:

1. **Data Collection & Integration** – acquired, cleaned, and merged multi-source datasets.  
2. **Analytical Modeling** – conducted statistical, temporal, and spatial analyses.  
3. **Predictive Modeling** – applied ML (Random Forest & Gradient Boosting) to forecast migration timing.  

Key findings:  
- Clear species-specific timing shifts (e.g., Green Kingfisher arriving earlier).  
- Weak yet consistent climate correlations (mainly wind speed and temperature).  
- Random Forest outperformed Gradient Boosting in prediction accuracy but with low R² ≈ 0.005.  

These insights highlight the potential of **machine learning + environmental data analytics** for biodiversity and conservation planning.

---

## 🎯 Project Goal & Scope
- Investigate long-term relationships between **climate variables and bird migration timing**.  
- Map **migration hotspots** and habitat stress zones.  
- Quantify **climate correlations** using statistical analysis.  
- Build **predictive models** to estimate future migration behavior.  

---

## 🧰 Tools & Technologies
| Category | Tools / Libraries |
|-----------|------------------|
| **Languages** | Python |
| **Libraries** | Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Plotly, Folium |
| **Statistical Methods** | Linear Regression, Pearson Correlation |
| **ML Models** | Random Forest, Gradient Boosting |
| **Clustering** | DBSCAN (Spatial Hotspot Detection) |
| **Environment** | Google Colab |
| **Data Sources** | eBird API, NOAA GHCN, MODIS Land Cover |

---

## 🧩 Methodology Overview

### 🪶 Milestone 1 – Data Collection & Integration
- Acquired datasets from **eBird**, **NOAA**, and **MODIS**.  
- Cleaned duplicates, filled missing values, and normalized formats.  
- Merged datasets on date & geo-coordinates for spatiotemporal alignment.  
- Created a master dataset for analysis and model training.  

**Challenges:** large files, inconsistent formats, and temporal misalignment.

---

### 📊 Milestone 2 – Analytical Modeling
- **Temporal Analysis:** Detected earlier arrivals for some species via linear regression on Day-of-Year (DOY).  
- **Correlation Analysis:** Computed Pearson r between climate variables and DOY. Wind speed showed the most consistent inverse relationship.  
- **Spatial Analysis:** Used DBSCAN clustering and Folium maps to visualize migration hotspots and habitat loss.  


---

### 🤖 Milestone 3 – Predictive Modeling & Visualization
- **Algorithms:** Random Forest & Gradient Boosting.  
- **Features:** TMAX, TMIN, Precipitation, Wind Speed, Humidity, Year.  
- **Performance:**  
  - Random Forest → MSE ≈ 189.29, MAE ≈ 7.88 days, R² ≈ 0.005  
  - Gradient Boosting → MSE ≈ 195.04, MAE ≈ 8.2 days  
- **Feature Importance:** Temperature most influential, followed by wind speed.  
- **Visualization:** Scatter (Actual vs Predicted DOY), Feature Importance Bars, Interactive Dashboard.  

---

## 🗺️ Sample Visual Outputs
- <img width="487" height="503" alt="image" src="https://github.com/user-attachments/assets/bdfe5067-7f45-4eb5-b19e-d14c75cbd8cb" />
- <img width="381" height="179" alt="image" src="https://github.com/user-attachments/assets/a2bd51fe-493e-490c-9cfc-df35269bb1af" />
- <img width="380" height="179" alt="image" src="https://github.com/user-attachments/assets/ec4d044d-29ca-4367-a44b-a5afa358faff" />
- <img width="403" height="261" alt="image" src="https://github.com/user-attachments/assets/fb869c72-b0a5-48c7-bff8-828481c27a1b" />
- <img width="365" height="259" alt="image" src="https://github.com/user-attachments/assets/6c9bb203-fdbf-431b-9ea0-6c88cd4e6ab5" />
 

---

## 📈 Key Results
| Metric | Random Forest | Gradient Boosting |
|--------|----------------|-------------------|
| MSE | 189.29 | 195.04 |
| MAE (days) | 7.88 | 8.20 |
| R² | 0.005 | – 0.002 |

> **Observation:** Random Forest performed better but further feature engineering and data scaling could improve accuracy.

---

## 🧠 Insights & Conclusions
- Temperature and wind speed are key drivers of migration timing.  
- Species show heterogeneous responses to climate variability.  
- Spatial hotspots highlight regions with increasing habitat loss.  
- Demonstrates how data analytics + ML can enhance climate ecology studies.  

---

## 🔮 Future Work
- Integrate additional environmental indices (e.g., NDVI).  
- Experiment with LSTM and XGBoost models for time-series forecasting.  
- Enhance dashboard with real-time API data streams.  
- Expand dataset to global migration records for higher model generalization.  



