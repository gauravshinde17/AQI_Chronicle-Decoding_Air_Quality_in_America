# AQI Chronicle: Decoding Air Quality in America (2000–2016)

This project analyzes **U.S. EPA ambient air quality data (2000–2016)** for **O₃, NO₂, SO₂, and CO** across **47 states and ~1.7M measurements**, rebuilding the **Air Quality Index (AQI)** from raw concentrations and assessing **regulatory compliance**.

---

## 🔗 Project Link

Notebook: [AQI Chronicle: Decoding Air Quality in America](https://www.kaggle.com/code/gauravshinde017/aqi-chronicle-decoding-air-quality-in-america)  
Report: `AQI_Project_Report.md` (phase‑wise summary of results)

---

## 📌 Overview

The project answers three core questions:

1. **How has U.S. air quality changed from 2000–2016?**  
2. **Which regions and pollutants drive the worst AQI days?**  
3. **Are we meeting EPA NAAQS standards, and where are the gaps?**

To do this, the notebook:

- Cleans and standardizes multi‑year EPA monitoring data  
- Recomputes AQI using official EPA breakpoint formulas  
- Engineers regulatory design values and exceedance flags  
- Explores temporal, multi‑pollutant, and geospatial patterns  

---

## 📊 Dataset

- **Source**: U.S. EPA / Kaggle export `pollution_us_2000_2016.csv`  
- **Coverage**:  
  - 2000–2016 (17 years)  
  - 47 U.S. states  
  - ~1.7M daily site‑level observations  
- **Pollutants**: O₃, NO₂, SO₂, CO (means, max values, AQI)
- **Dataset Source**: [U.S. Pollution Dataset](https://www.kaggle.com/datasets/sogun3/uspollution)

---

## 🧪 What This Project Does

**Phase 1 – Data Preparation**

- Load and inspect EPA pollution data  
- Perform QA/QC and unit standardization (ppb → ppm)  
- Recompute **AQI** for all four pollutants using EPA methodology  
- Engineer:
  - Temporal features (Year, Season, Weekend)  
  - O₃ **design values** (4th‑highest, 3‑year)  
  - NAAQS **exceedance flags** for each pollutant  

**Phase 2 – Exploratory Analysis**

- Long‑term trends for O₃, NO₂, SO₂, CO  
- Multi‑pollutant correlations (e.g., NO₂–CO as traffic signature)  
- Geospatial hot‑spots and regional profiles  
- NAAQS compliance status and non‑attainment areas  
- AQI category distribution and extreme‑event days  

---

## 📌 Key Insights

**🌟 SO₂ Success Story: −80.5% decline** (2000–2016)  
Coal plant scrubbers and fuel desulfurization worked ✓

**⚠️ O₃ Stubborn Pollutant: −7.7% improvement only**  
12.5% of sites exceed NAAQS (0.075 ppm design value)

**🗺️ Hot Spots:**  
- **Meigs County, TN** (AQI 70.2)  
- **Riverside, CA** (AQI 66.3, chronic O₃ violation)  
- **Forsyth, NC** (AQI 68.5)  

**🔗 Traffic Signature:** NO₂–CO correlation (0.61) confirms shared vehicle sources

**📅 Seasonal:** O₃ peaks summer (+55% vs winter), NO₂/CO peak winter inversions

**🏆 Compliance:** SO₂ 99% attainment ✓, O₃ 87% attainment ✗

---

## 🧱 Tech Stack

- Python, Jupyter Notebook  
- pandas, numpy  
- matplotlib, seaborn  

---



