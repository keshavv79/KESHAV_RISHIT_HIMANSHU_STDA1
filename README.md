# Spatio-Temporal Data Analysis (STDA)

This repository contains the assignments and project reports for the Spatio-Temporal Data Analysis (STDA) course. The projects focus on applying spatial, temporal, and spatio-temporal statistical techniques and machine learning models to real-world datasets, specifically the Global Terrorism Database (GTD) and Urban Bike-Sharing networks.

**Team Members (IIIT Bangalore):**
* Keshav Goyal
* Rishit Mane
* Himanshu Khatri

---

## 📁 Repository Structure


KESHAV_RISHIT_HIMANSHU_STDA1/
│
├── A1/
│   ├── EDA_1.ipynb
│   │   # Data preprocessing, EDA, and spatial modeling code
│   │
│   └── IMT2022560_564_584_A1 (2).pdf
│       # Spatial Autocorrelation and Regression Analysis Report
│
├── A2/
│   ├── EDA2.ipynb
│   │   # Time-series decomposition, ACF/PACF, and ARIMA forecasting code
│   │
│   └── imt2022560_564_584_a2 (2).pdf
│       # Temporal Analysis and Short-Term Forecasting Report
│
└── A3/
    ├── london_clean.ipynb
    │   # Spatio-temporal analysis and modeling for London bike-share
    │
    ├── taipei.ipynb
    │   # Temporal analysis and modeling for Taipei bike-share
    │
    └── IMT2022560_564_584_A3.pdf
        # Bike-Sharing Systems Spatio-Temporal Analysis Report


---

## 📝 Assignment Descriptions

### **A1: Spatial Autocorrelation and Regression Analysis of Global Terrorism Incidents**
**Folder:** `A1/`

**Objective:** To investigate the spatial structure of global terrorism incidents using country-level aggregation of the Global Terrorism Database (GTD).

**Key Highlights:**
* **Spatial Autocorrelation:** Evaluated whether terrorist attack counts exhibit systematic spatial clustering using Global Moran's I.
* **LISA Analysis:** Identified localized spatial patterns, mapping specific high-high (hotspots) and low-low (coldspots) regions of terrorist activity.
* **Spatial Regression:** Built an Ordinary Least Squares (OLS) regression model using fatalities as a predictor of attack counts. Upon detecting residual spatial autocorrelation, a spatial lag model was fitted to assess spatial spillover effects across neighboring borders.

---

### **A2: Temporal Analysis and Short-Term Forecasting of Global Terrorism Incidents (1970–2017)**
**Folder:** `A2/`

**Objective:** To analyze long-term trends, temporal variability, and potential seasonal patterns in global terrorist activity, and to forecast short-term future activity.

**Key Highlights:**
* **Time-Series Decomposition:** Separated the monthly attack count series into trend, seasonal, and residual components using classical decomposition.
* **Stationarity & Autocorrelation:** Utilized Augmented Dickey-Fuller (ADF) tests, alongside ACF and PACF plots, to examine temporal dependence and stabilize variance using log transformations.
* **Forecasting:** Developed and compared ARIMA(0,1,1) models against baseline linear regression models using a holdout validation strategy. The ARIMA model successfully captured short-term temporal dependencies and significantly outperformed the baseline.

---

### **A3: Spatio-Temporal Analysis and Modeling of Bike-Sharing Systems in London and Taipei**
**Folder:** `A3/`

**Objective:** A comprehensive spatio-temporal analysis comparing large-scale bike-sharing data from two distinct urban environments: London and Taipei.

**Key Highlights:**
* **Temporal Dynamics:** Analyzed hourly demand and daily seasonality, highlighting distinct peak-hour commuting patterns in London versus smoother, more uniformly distributed usage in Taipei.
* **Spatial Structure:** Examined station-level demand in London using Moran's I, Geary's C, and LISA to identify geographic hotspots and dominant origin-destination flows. K-means clustering was also applied to group stations based on activity and location.
* **Predictive Modeling:** Engineered lag-based, calendar-based, and rolling-statistic features to forecast demand. Utilized Linear Regression for spatial prediction and non-linear tree-based models (Random Forest, XGBoost) to capture complex temporal interactions.
