# Climate Alpha AI – Environmental Financial Intelligence Platform

**Production-grade satellite-driven climate risk analytics & AI-powered financial intelligence using Google Earth Engine and Yahoo Finance**

![Dashboard Preview](climate_alpha_ai_dashboard.png)

---

# Overview

Climate Alpha AI is an advanced **Climate + ESG + Financial Intelligence Platform** that combines:

- Satellite environmental monitoring
- AI-based forecasting
- Geospatial analytics
- ESG risk assessment
- Financial market intelligence

The platform uses **Google Earth Engine satellite datasets** and **Yahoo Finance market data** to analyze how environmental conditions influence stock performance, sector volatility, urban economic activity, and long-term climate risk.

The system provides:

- Environmental risk scoring
- Climate-financial correlation analysis
- Stock trend forecasting
- ESG-style analytics
- Pollution and temperature monitoring
- AI-driven forecasting models
- Interactive dashboards and geospatial insights

The methodology is inspired by real-world environmental intelligence systems used by companies like MSCI, Bloomberg, and climate-tech ESG platforms.

---

# Key Features

| Feature | Description |
|---|---|
| **Satellite environmental analysis** | NO₂, SO₂, CH₄, Aerosol Index, NDVI, and Land Surface Temperature using Google Earth Engine |
| **Financial intelligence integration** | Real-time and historical stock market analysis using Yahoo Finance |
| **Climate-financial correlation engine** | Detects relationships between environmental conditions and stock performance |
| **AI forecasting models** | Random Forest, XGBoost, Gradient Boosting, Ridge, and Lasso Regression |
| **ESG-style risk scoring** | Composite environmental risk scoring inspired by MSCI methodologies |
| **Geospatial analytics** | City-level and regional environmental monitoring |
| **Production-grade pipeline** | Automated extraction, validation, preprocessing, logging, and visualization |
| **Interactive dashboards** | Heatmaps, trend analysis, clustering, and forecasting visualizations |
| **Sector-level intelligence** | Environmental impact analysis across Energy, IT, Manufacturing, Transportation, and Automotive sectors |

---

# Data Sources

All environmental datasets are accessed using Google Earth Engine.

Financial market data is accessed using Yahoo Finance.

---

## Environmental Datasets

| Variable | Satellite / Product | Band | Resolution |
|---|---|---|---|
| NO₂ | Sentinel-5P TROPOMI | `tropospheric_NO2_column_number_density` | ~7 km |
| SO₂ | Sentinel-5P | `SO2_column_number_density` | ~7 km |
| CH₄ | Sentinel-5P | `CH4_column_volume_mixing_ratio_dry_air` | ~7 km |
| Aerosol Index (AER) | Sentinel-5P | `absorbing_aerosol_index` | ~7 km |
| Land Surface Temperature (LST) | MODIS MOD11A1 | `LST_Day_1km` | 1 km |
| NDVI | MODIS Vegetation Index | `NDVI` | 250 m |

---

## Financial Datasets

| Source | Data |
|---|---|
| Yahoo Finance | Historical stock prices |
| Yahoo Finance | Volume analysis |
| Yahoo Finance | Sector-based performance |
| Yahoo Finance | Volatility and returns |

---

## Example Stocks Used

| Company | Sector |
|---|---|
| RELIANCE.NS | Energy |
| TCS.NS | IT |
| INFY.NS | Technology |
| WIPRO.NS | Technology |
| NTPC.NS | Power |
| TATASTEEL.NS | Manufacturing |
| MARUTI.NS | Automotive |
| HEROMOTOCO.NS | Automotive |

---

# Methodology

## 1. Environmental Risk Scoring Framework

The platform generates ESG-style environmental risk scores using:

- Pollution intensity
- Climate trend analysis
- Exposure analysis
- Temperature anomalies
- Environmental volatility

---

## Risk Score Components

| Component | Weight |
|---|---|
| Current Environmental Risk | 55% |
| Trend Risk | 25% |
| Climate Exposure | 20% |

---

## Pollutant Weight Distribution

| Pollutant | Weight |
|---|---|
| NO₂ | 30% |
| Aerosol Index | 25% |
| SO₂ | 20% |
| CH₄ | 15% |
| LST | 10% |

---

# Climate-Financial Correlation Analysis

The platform analyzes relationships between:

| Environmental Variable | Financial Variable |
|---|---|
| NO₂ | Industrial stock performance |
| SO₂ | Manufacturing volatility |
| LST | Energy demand and utility stocks |
| NDVI | Agricultural performance |
| Aerosol Index | Urban economic activity |

Techniques used:

- Pearson Correlation
- Spearman Correlation
- Linear Regression
- Rolling Correlation Windows
- Trend Decomposition

---

# AI & Machine Learning Pipeline

## Data Pipeline

1. Satellite data extraction from Google Earth Engine
2. Financial market data acquisition from Yahoo Finance
3. Data synchronization and preprocessing
4. Feature engineering
5. Model training and validation
6. Forecast generation
7. Dashboard visualization

---

## Models Used

| Model | Purpose |
|---|---|
| Random Forest | Non-linear prediction |
| XGBoost | High-performance forecasting |
| Gradient Boosting | Ensemble prediction |
| Ridge Regression | Trend modeling |
| Lasso Regression | Feature selection |

---

## Feature Engineering

Generated features include:

- Rolling averages
- Moving volatility
- Lag-based climate indicators
- Pollution spike detection
- Heatwave indicators
- Momentum indicators
- Climate anomaly scores

---

## Forecasting Framework

### Inputs

- Environmental indicators
- Climate trends
- Stock returns
- Volatility metrics
- Sector exposure

### Outputs

- Risk forecasts
- Climate-sensitive stock predictions
- Sector vulnerability analysis
- ESG-style intelligence scores

---

# Geospatial Analytics

The system performs regional environmental analysis for major Indian cities including:

- Mumbai
- Delhi
- Bengaluru
- Hyderabad
- Chennai
- Kolkata
- Ahmedabad
- Pune

---

# Clustering & Risk Profiling

The platform uses K-Means clustering to classify cities and sectors into:

- High Risk / Worsening
- Moderate Risk / Stable
- Low Risk / Improving

Optimization techniques:

- Silhouette score analysis
- PCA dimensionality reduction
- Cluster validation

---

# Installation & Setup

## Prerequisites

- Python 3.9+
- Google Earth Engine account
- Yahoo Finance API access
- Jupyter Notebook / Google Colab

---

## Install Dependencies

```bash
pip install earthengine-api pandas numpy matplotlib seaborn plotly scikit-learn scipy xgboost yfinance geopandas
```

---

## Authenticate Google Earth Engine

```python
import ee

ee.Authenticate()
ee.Initialize(project='your-project-id')
```

---

# Project Structure

```text
Climate-Alpha-AI/
│
├── data/
│   ├── raw/
│   ├── processed/
│   └── financial/
│
├── notebooks/
│   ├── environmental_analysis.ipynb
│   ├── stock_analysis.ipynb
│   └── forecasting_models.ipynb
│
├── visualizations/
│   ├── dashboards/
│   ├── heatmaps/
│   └── reports/
│
├── models/
│   ├── trained_models/
│   └── evaluation/
│
├── src/
│   ├── gee_data_extraction.py
│   ├── yahoo_finance_loader.py
│   ├── feature_engineering.py
│   ├── forecasting.py
│   ├── visualization.py
│   └── utils.py
│
├── outputs/
│   ├── climate_risk_scores.csv
│   ├── stock_forecasts.csv
│   ├── sector_analysis.csv
│   ├── clustering_results.csv
│   ├── correlation_analysis.csv
│   └── executive_summary.txt
│
├── requirements.txt
├── README.md
└── main.py
```

---

# Dashboard & Visualization

The platform includes:

## Interactive Dashboards

- Environmental monitoring dashboard
- ESG risk dashboard
- Climate-financial correlation dashboard
- Forecasting dashboard

---

## Visual Analytics

| Visualization | Purpose |
|---|---|
| Heatmaps | Correlation analysis |
| Time-series charts | Trend monitoring |
| Geospatial maps | Pollution visualization |
| Cluster plots | Risk profiling |
| Forecast graphs | Future predictions |

---

# Business Value

Climate Alpha AI introduces a new category of:

> Satellite-driven financial intelligence.

Potential applications:

- ESG investing
- Hedge fund research
- Climate risk analytics
- Sustainable finance
- Smart city monitoring
- Environmental intelligence systems

Potential enterprise users:

- MSCI
- Bloomberg
- BlackRock
- S&P Global

---

# Performance & Optimization

## Optimization Techniques

- Vectorized processing
- Efficient satellite querying
- Parallel data extraction
- Feature caching
- PCA dimensionality reduction

---

# Future Enhancements

## Planned Improvements

### Deep Learning

- LSTM forecasting
- Transformer-based prediction
- Graph Neural Networks

### Real-Time Intelligence

- Live environmental monitoring
- Streaming stock forecasts
- Real-time anomaly detection

### Enterprise Deployment

- FastAPI backend
- Streamlit dashboards
- Docker deployment
- Cloud deployment

### ESG Expansion

- Carbon footprint scoring
- Sustainability ranking engine
- Climate stress testing

---

# Research Potential

This project has strong research applications in:

- Climate Finance
- ESG Analytics
- Environmental Economics
- Financial Machine Learning
- Geospatial AI
- Climate Risk Forecasting

---

# License

This project is licensed under the MIT License.

---

# Author

## Ansh Kambli

Data Science | Climate AI | ESG Analytics | Financial Intelligence

### Areas of Interest

- Climate Intelligence
- ESG Analytics
- Financial AI
- Geospatial Data Science
- Satellite Data Analytics
- Machine Learning

---

# Final Vision

Climate Alpha AI aims to become:

> “Bloomberg Terminal + Satellite Intelligence + AI-powered Climate Risk Forecasting.”

By combining satellite observations, AI forecasting, and financial intelligence, the platform creates a next-generation environmental analytics ecosystem for the future of sustainable finance.
