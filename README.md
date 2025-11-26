# AI-Based Soil Moisture & Drought Risk Prediction System

This project develops a small AI system that predicts short-term soil-moisture anomalies and classifies drought risk by region using satellite-based soil moisture, rainfall, and vegetation indices. The system is designed as an end-to-end pipeline that includes geospatial data extraction, feature engineering, machine learning, and a simple interactive web dashboard.

The goal is to demonstrate how AI can support drought monitoring and early warning in data-scarce regions using open satellite data.

---

## 1. Project Objectives

- Build a regional, monthly soil moisture anomaly prediction system  
- Classify drought risk into interpretable categories  
- Integrate multi-source satellite datasets  
- Train a machine learning model using engineered geospatial features  
- Deploy a simple web-based dashboard for visualization and decision support  

---

## 2. Study Area

The system is designed to operate at the regional level for selected administrative regions. Initial implementation focuses on a limited number of regions for prototyping and validation.

---

## 3. Data Sources

All datasets are based on open satellite and reanalysis products accessed through Google Earth Engine.

- Soil Moisture: SMAP / ERA5-Land  
- Rainfall: GPM / CHIRPS  
- Vegetation Index: MODIS NDVI  
- Optional: Land Surface Temperature, PET

All datasets are aggregated to monthly resolution at the regional level.

---

## 4. System Overview

The pipeline consists of four main stages:

1. Data extraction from Google Earth Engine  
2. Feature engineering and drought label creation  
3. Machine learning model training and evaluation  
4. Interactive web application for prediction and visualization  

---

## 5. Machine Learning Approach

Two prediction tasks are supported:

- Soil moisture anomaly prediction (regression)
- Drought risk classification (classification)

In the initial implementation, a Random Forest classifier is used to predict drought class using:

- Lagged soil moisture
- Cumulative rainfall
- Vegetation index
- Seasonal indicators

---

## 6. Web Application

A Streamlit-based web dashboard provides:

- Regional drought risk prediction  
- Soil moisture anomaly visualization  
- Historical time series analysis  
- Model interpretation and feature importance 

---

## 7. Results

Model performance metrics, drought classification accuracy, and regional analysis maps will be added upon completion of model training.

---

## 8. Future Work

Integration of additional climate drivers (temperature, PET, ENSO)

Use of time-series deep learning models

Cloud deployment on Google Cloud Platform

Extension to near-real-time drought monitoring

---

## 9. Author

Name: Shraddha Gourishetty
Background: Geomatics, GIS, Remote Sensing
Focus: AI for environmental and climate applications