# 🌿 Air Quality Analysis – Probability Distributions & Outlier Detection

This project was developed as part of **Course 3** of the **Google Advanced Data Analytics Certificate**. It simulates the role of a data analyst at the **United States Environmental Protection Agency (EPA)**, tasked with identifying regions that may need support to improve air quality.

---

## 📌 Project Overview

The activity focuses on analyzing **Air Quality Index (AQI)** values for **carbon monoxide** across over 200 monitoring sites. The main objectives are to understand the distribution of data, calculate **z-scores**, and detect **outliers** that may indicate critical pollution levels.

---

## 🧪 Development Process

### Initial Setup
- Defined the problem: Identify regions with unusual AQI behavior  
- Imported libraries: `numpy`, `pandas`, `matplotlib`, `scipy`, `statsmodels`  

### Data Exploration & Preparation
- Loaded EPA dataset containing air quality metrics by site, city, state, and county  
- Focused analysis on the `AQI` values for **carbon monoxide**  
- Reviewed distribution shape, calculated summary statistics, and evaluated data quality  

### Distribution Analysis
- Plotted histograms and density plots  
- Measured **skewness** and **kurtosis** to assess distribution symmetry and tail behavior  
- Used **z-scores** to identify statistical outliers  

---

## 📊 Key Insights

- Most AQI values for carbon monoxide followed a near-normal distribution  
- Right-skewed data patterns were observed in some locations, indicating possible pollution spikes  
- Z-score analysis revealed high outliers in specific monitoring sites that may require further investigation  
- Distribution insights support decisions on where to prioritize environmental intervention  

---

## 📁 Project Files

- `Activity_Explore probability distributions.ipynb`  
  → Jupyter Notebook with full analysis, charts, and summary statistics  

---

## 🛠 Tools Used

- Google colab
- Python  
- pandas  
- matplotlib  
- scipy  
- statsmodels  

---

This project demonstrates key statistical techniques for exploring real-world environmental data. It reflects core data analyst responsibilities in public sector contexts—**data cleaning, distribution analysis, anomaly detection, and actionable insight generation**.

---
